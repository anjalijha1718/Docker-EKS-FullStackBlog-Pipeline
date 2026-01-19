# Docker-EKS-FullStackBlog-Pipeline

![DevOps Banner](https://miro.medium.com/v2/resize:fit:720/format:webp/0*LdTGlxSTQHnTl9uy.gif)

**DevOps Project: End-to-End CI/CD Pipeline for Full-Stack Blogging Application**

*A Spring Boot Application Deployed on AWS EKS with Terraform, Jenkins, SonarQube, Nexus, Trivy & Prometheus/Grafana*

## 📋 Project Overview

Production-ready **Full-Stack Blogging Application** with complete **CI/CD pipeline**:

- Spring Boot REST API
- Docker containerization
- AWS EKS Kubernetes deployment
- Jenkins automated pipeline
- Terraform Infrastructure as Code
- Production monitoring with Prometheus + Grafana

## ✨ Features

- ✅ Create/Edit/Delete Blog Posts
- ✅ RESTful API (Spring Boot)
- ✅ SonarQube Code Analysis
- ✅ Trivy Vulnerability Scanning
- ✅ Jenkins CI/CD Pipeline
- ✅ AWS EKS Deployment
- ✅ Nexus Artifact Repository
- ✅ Email Notifications
- ✅ Prometheus + Grafana Monitoring

## 📱 Screenshots

**Login Page**  
![Login](https://miro.medium.com/v2/resize:fit:700/0*1TkD_l1YWmE6CPwz.png)

**Home Page**  
![Home](https://miro.medium.com/v2/resize:fit:700/0*pFYg1X3ZAZ0STgcS.png)

**Blog Post**  
![Post](https://miro.medium.com/v2/resize:fit:700/0*6156xWhmbdVtlxYj.png)


## 🏗️ Infrastructure

**7 AWS EC2 Instances:**
- Jenkins Server (t2.large)
- EKS Master + 2 Worker Nodes (t2.medium)
- SonarQube, Nexus, Monitoring (t2.medium)

![Infra](https://miro.medium.com/v2/resize:fit:700/0*HiK2H1lqLBR0Fs8r.png)

## 🚀 Quick Setup

### 1. AWS CLI + Terraform
```bash
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip && sudo ./aws/install
aws configure

sudo apt install terraform -y
# SonarQube
docker run -d -p 9000:9000 sonarqube:lts-community

# Nexus  
docker run -d -p 8081:8081 sonatype/nexus3


