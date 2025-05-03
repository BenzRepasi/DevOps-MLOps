# Use a pinned Alpine version for reproducibility (like v1) but with LTS Node (like v2)
ARG NODE_VERSION=23.3.0
FROM node:${NODE_VERSION}-alpine

# Set production environment early (both versions)
ENV NODE_ENV=production

# Create and set working directory (like both versions)
WORKDIR /usr/src/app

# Copy only lockfiles first (wildcard handling from v2, but stricter like v1)
COPY package.json package-lock.json* ./

# Install dependencies with npm ci + cache mount (best of v1 + v2)
RUN --mount=type=cache,target=/root/.npm \
    if [ -f package-lock.json ]; then npm ci --omit=dev; \
    else npm install --production --silent; fi

# Switch to non-root user early (security best practice from v1)
USER node

# Copy app files (after npm install for better layer caching)
COPY --chown=node:node . .

# Expose port (same in both)
EXPOSE 8080

# Run application (CMD as array, best practice)
CMD ["node", "app.js"]