# 🚀 End-to-End DevOps Projects

A curated collection of DevOps projects demonstrating cloud deployments, automation, monitoring, CI/CD pipelines, and Kubernetes orchestration using top tools like AWS, Jenkins, Docker, Terraform, and Ansible.

---

## 📁 VProfile App Setup – Manual & Automated

- Set up a multi-tier Java web app (VProfile) using Linux VMs via Vagrant
- Manually deployed Nginx, Tomcat, RabbitMQ, Memcached, and MySQL services
- Automated infrastructure using shell scripts and systemd unit files
- Configured service dependencies and application deployment for local R&D lab

---

## 📦 Containerization of VProfile App

- Containerized VProfile services using Docker with custom Dockerfiles
- Created Docker Compose file to manage multi-container deployment (Tomcat, MySQL, Nginx, etc.)
- Built and pushed Docker images to DockerHub
- Verified local deployment and established container-to-container networking

---

## 🧊 Containerizing Microservices (E-Mart App) [https://github.com/Akash1612-cryto/emartapp]

- Containerized Angular, Node.js, Java, MySQL, and MongoDB microservices
- Used multi-stage Dockerfiles for optimized builds
- Centralized routing via NGINX API Gateway using custom configuration
- Used Docker Compose to orchestrate 6 services in a mono-repo setup

---

## ☸️ Kubernetes Deployment of VProfile App

- Deployed containerized VProfile stack on AWS-hosted Kubernetes cluster via KOPS
- Defined Kubernetes Deployments, Services (ClusterIP), Secrets, PVCs for MySQL
- Used AWS EBS via dynamic PVC provisioning
- Managed external access via Ingress Controller + AWS ALB
- Applied labels & affinity for zone-based scheduling

---

## 🌩️ Lift & Shift VProfile App to AWS

- Migrated the locally running VProfile stack to AWS EC2 instances using the lift-and-shift strategy
- Configured ELB, Auto Scaling Groups, RDS, and Security Groups for scalable architecture
- Used Route 53 for private DNS and S3 for artifact storage
- Implemented TLS using ACM for secure access

---

## 🔁 Re-Architecting VProfile App using AWS PAAS & SAAS

- Refactored infrastructure using AWS managed services (Beanstalk, RDS, ElastiCache, AmazonMQ)
- Hosted the frontend on Elastic Beanstalk with HTTPS via ALB
- Utilized CloudFront + Route53 for global access and domain routing
- Simplified backend management using managed DB and caching layers

---

## 🧪 Jenkins CI/CD Pipeline (WAR Artifact)

- Installed and configured Jenkins on AWS EC2
- Set up multi-stage pipeline: Code Checkout ➝ Maven Build ➝ Unit Test ➝ Code Analysis ➝ Artifact Upload (Nexus)
- Integrated SonarQube and Checkstyle for code quality gate enforcement
- Used Jenkinsfile for pipeline-as-code and GitHub as SCM

---

## 🐳 CI Pipeline with Docker Image Creation

- Extended CI pipeline to include Docker image builds using Jenkins
- Built multi-stage Docker image from source and pushed to Amazon ECR
- Used Docker and AWS plugins in Jenkins with IAM credentials stored securely
- Versioned and tagged images using Jenkins build numbers

---

## 📦 Ansible for AWS Infrastructure

- Used Ansible modules to automate AWS EC2 instance creation and key pair management
- Managed credentials via IAM access keys securely exported via environment variables
- Created reusable playbooks for provisioning infrastructure
- Stored keys securely and handled EC2 provisioning idempotently

---

## ⚙️ AWS CI/CD Pipeline with CodePipeline & Bitbucket

- Built a CI/CD pipeline using AWS CodePipeline integrated with Bitbucket
- CodeBuild was configured using `buildspec.yml` for Maven-based Java build
- Elastic Beanstalk used for artifact deployment and environment hosting
- Implemented RDS for backend with secured parameter handling

--------------------------------------------------------------------------------------------------------------

📂 Project Code Repository
Explore complete source code, shell scripts, Dockerfiles, and Kubernetes YAMLs used across these projects:  
🔗 [github.com/Akash1612-cryto/vprofile-project](https://github.com/Akash1612-cryto/vprofile-project)
