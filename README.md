No problem! Here’s a **lean, hyper-focused 90-day DevOps/MLOps roadmap** that combines **Docker, AWS, Kubernetes, and Andrew Ng’s MLOps**—designed for maximum job relevance in 3 months.  

---

## **🚀 90-Day DevOps/MLOps Sprint**  
*(Priority Order: Docker → AWS → Kubernetes → MLOps)*  

### **📌 Month 1: Docker & AWS Core (Days 1-30)**  
**Goal:** Master containerization and AWS basics.  
| **Week** | **Focus**                    | **Key Tasks**                                                                 |
|----------|------------------------------|-------------------------------------------------------------------------------|
| **1**    | Docker Fundamentals          | - Dockerize Python/ML apps (FastAPI + PyTorch). <br>- Optimize images (multi-stage builds). |
| **2**    | AWS EC2, ECR, IAM            | - Deploy Docker containers on EC2. <br>- Set up ECR and CI/CD with GitHub Actions. |
| **3**    | AWS ECS & Terraform          | - Run containers on ECS Fargate. <br>- Automate infra with Terraform.          |
| **4**    | AWS Networking (VPC, S3)     | - Build a secure VPC. <br>- Create an S3-backed app with IAM roles.            |

**Andrew Ng Tie-In:**  
- Use Week 1’s Docker skills to containerize his **Week 3 model deployment examples**.  

---

### **📌 Month 2: Kubernetes & CI/CD (Days 31-60)**  
**Goal:** Orchestrate containers and automate pipelines.  
| **Week** | **Focus**                    | **Key Tasks**                                                                 |
|----------|------------------------------|-------------------------------------------------------------------------------|
| **5**    | Kubernetes Basics            | - Deploy apps on **local K8s (Minikube)**. <br>- Learn Pods, Deployments, Services. |
| **6**    | AWS EKS                      | - Migrate apps to **EKS**. <br>- Configure ALB Ingress.                        |
| **7**    | CI/CD for K8s (GitOps)       | - Set up **ArgoCD** for GitOps. <br>- Helm charts for packaging.               |
| **8**    | Monitoring (Prometheus)      | - Monitor EKS with **Prometheus/Grafana**. <br>- Logging with CloudWatch.     |

**Andrew Ng Tie-In:**  
- Deploy his **model serving lab** on EKS (replace local K8s).  

---

### **📌 Month 3: MLOps & Capstone (Days 61-90)**  
**Goal:** Build production-ready ML systems.  
| **Week** | **Focus**                    | **Key Tasks**                                                                 |
|----------|------------------------------|-------------------------------------------------------------------------------|
| **9**    | **Andrew Ng’s MLOps**        | - Complete Weeks 1-2 (ML pipelines). <br>- Integrate **MLflow** for tracking. |
| **10**   | Model Deployment (SageMaker) | - Deploy his Week 3 labs on **SageMaker**. <br>- Custom Docker containers.    |
| **11**   | End-to-End Project           | - Build a **herbarium classifier pipeline**: <br>  - Train → Dockerize → Deploy on EKS. |
| **12**   | Job Prep & Polish            | - Record demos. <br>- Optimize LinkedIn/GitHub. <br>- Mock interviews.        |

---

### **🎯 Capstone Project**  
**"MLOps Pipeline on AWS"**  
1. **Data:** Herbarium images in S3.  
2. **Training:** SageMaker (custom Docker container).  
3. **Orchestration:** Kubernetes (EKS) + ArgoCD.  
4. **Monitoring:** SageMaker Model Monitor + Prometheus.  

**Result:** A **portfolio-ready project** covering Docker, AWS, K8s, and MLOps.  

---

### **⚡ Efficiency Hacks**  
1. **Focus on AWS Only** (skip GCP unless needed).  
2. **Use Pre-Builds** (e.g., SageMaker built-in algorithms for quick wins).  
3. **Reuse Code** (adapt Andrew Ng’s labs for AWS).  
4. **Daily 2-3 Hours** (prioritize hands-on over theory).  

---

### **📚 Resource Plan**  
| **Topic**       | **Resource**                                  | **Time**  |  
|-----------------|-----------------------------------------------|-----------|  
| Docker          | Docker Deep Dive (Nigel Poulton)              | Week 1    |  
| AWS             | AWS DevOps Pro Udemy Course                   | Weeks 2-4 |  
| Kubernetes      | K8s Documentation + EKS Workshop              | Weeks 5-8 |  
| MLOps           | Andrew Ng’s Course + AWS SageMaker Labs       | Weeks 9-10|  

---

### **🔧 Tools You’ll Master**  
- **Containers:** Docker, ECR  
- **Orchestration:** EKS, Helm  
- **MLOps:** SageMaker, MLflow  
- **CI/CD:** GitHub Actions, ArgoCD  

---

## **⏱️ Weekly Time Commitment**  
- **Weekdays:** 2 hours/day (hands-on labs).  
- **Weekends:** 4 hours (projects).  


## Journal
### 27.04.2025 - Day 1
- Created GH account
- Downloaded and installed Docker
- Book Docker Deep Dive (2025) pg. 64
### 28.04.2025 - Day 2
- Continue Docker Deep Dive (2025) until pg. 156
- docker run, kill, exec, 
- Manifest files
- Entrypoint and Cmd in manifest
- image vs container: 1:N relationship
- docker pull: opinionated, defaults to dockerhub and latest tag
- docker layers: docker -> containerd -> shim -> runc
- added lazydocker and grepy utilities
### 29-30.04 and 02.05.2025 - Day 3-5
- Continue Docker Deep Dive (2025) until pg. 218
- Pulled GitHub repo and containerised it via docker image
- Connected to DockerHub
- vulnerability scan with grype
- FROM, RUN, COPY, WORKDIR -> layers
- EXPOSE, ENV, CMD, ENTRYPOINT -> metadata
- VS extension to create Dockerfile, then run Deepseek for review
- MULTI-STAGE builds: Big image for compiling then copy it to slim-image
- Dockerfile can have multiple target, need to specify it with docker build --target

