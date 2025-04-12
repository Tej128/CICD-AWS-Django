# 🚀 Django CI/CD Deployment with AWS CodePipeline & CodeDeploy

This project demonstrates how to automate the deployment of a Django application using a complete CI/CD pipeline powered by **AWS CodePipeline**, **CodeDeploy**, and **EC2**. It showcases modern DevOps practices and AWS infrastructure for streamlined delivery.

---

## 🔧 Tech Stack

- **Django**
- **AWS EC2**, **IAM**, **CodePipeline**, **CodeDeploy**
- **Ubuntu Server**
- **Gunicorn**, **Nginx**
- **GitHub Integration**

---

## 🌟 Highlights

- 📦 **Automated CI/CD**: Build, test, and deploy stages triggered by code pushes.
- 🔐 **IAM Roles**: Secure, role-based access for CodeDeploy and EC2 instances.
- 🌐 **Live Deployment**: Public IP access to Django app after successful deploy.
- 🛠️ **Configuration Driven**: Uses `buildspec.yml`, `appspec.yml`, and `gunicorn.service`.

---

## ⚙️ How It Works

1. **Code Commit → GitHub**
2. **CodePipeline** detects push → triggers build via `buildspec.yml`
3. **CodeDeploy** deploys to EC2 using `appspec.yml`
4. EC2 runs `gunicorn` + `nginx` for serving Django

---

## 🚀 Getting Started

### 🔑 Prerequisites

- AWS account
- EC2 instance (Ubuntu)
- Proper IAM roles for CodeDeploy, EC2
- A Django project ready to deploy

### 🧩 Clone the Repo

```bash
git clone https://github.com/Tej128/CICD-AWS-Django.git
cd CICD-AWS-Django
