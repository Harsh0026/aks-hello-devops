# aks-hello-devops

# 🚀 Automated Kubernetes Deployment on Azure AKS

## 📌 Overview
This project demonstrates an end-to-end DevOps automation workflow for deploying a containerized web application on **Azure Kubernetes Service (AKS)** using **Terraform, Docker, Helm, and GitHub Actions**.

The solution follows modern DevOps best practices such as Infrastructure as Code (IaC), CI/CD automation, container security scanning, and Kubernetes-native deployments. A simple **Hello World web application** is automatically built, pushed, and deployed whenever code is pushed to the `main` branch.

---

## 🛠️ Tech Stack

- **Cloud Provider:** Azure  
- **Kubernetes:** Azure Kubernetes Service (AKS)  
- **Infrastructure as Code:** Terraform  
- **Containerization:** Docker  
- **Container Registry:** Azure Container Registry (ACR)  
- **CI/CD:** GitHub Actions  
- **Kubernetes Packaging:** Helm  
- **Ingress:** NGINX Ingress Controller  
- **Security:** Trivy (container image scanning)  
- **Monitoring:** Prometheus & Grafana  

---

## 🔄 CI/CD Workflow

The CI/CD pipeline is implemented using **GitHub Actions** and is automatically triggered on every push to the `main` branch.

### Pipeline Steps:
1. Code is pushed to the `main` branch
2. GitHub Actions builds the Docker image
3. Image is scanned for vulnerabilities using **Trivy**
4. Image is pushed to **Azure Container Registry**
5. Application is deployed to **AKS using Helm**
6. Application is exposed publicly via **NGINX Ingress**

---

## 🌐 Live Application

**http://20.253.60.24/**  
