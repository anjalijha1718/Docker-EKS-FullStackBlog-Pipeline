# Docker-EKS-FullStackBlog-Pipeline

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

## 🏗️ Infrastructure

**7 AWS EC2 Instances:**
- Jenkins Server (t2.large)
- EKS Master + 2 Worker Nodes (t2.medium)
- SonarQube, Nexus, Monitoring (t2.medium)

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


