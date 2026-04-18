# 🚀 AWS DevOps Project – Production-Grade Django Deployment

![AWS](https://img.shields.io/badge/AWS-EC2%20%7C%20RDS%20%7C%20S3-orange?logo=amazonaws\&logoColor=white)
![Django](https://img.shields.io/badge/Django-4.x-green?logo=django)
![DevOps](https://img.shields.io/badge/DevOps-Project-blue?logo=githubactions)
![Cloud](https://img.shields.io/badge/Cloud-AWS-blue?logo=amazonaws)
![Status](https://img.shields.io/badge/Status-Completed-brightgreen)
![License](https://img.shields.io/badge/License-MIT-lightgrey)

A scalable and production-ready Django web application deployed on AWS using modern DevOps and cloud best practices.

This project demonstrates real-world architecture including high availability, monitoring, security, and automated scaling.

---

## 📌 Project Overview

This project focuses on building and deploying a highly available Django application on AWS with:

* Load balancing
* Auto scaling
* Centralized logging
* Monitoring & alerts
* Secure networking
* CDN acceleration

It reflects how real-world production systems are designed and deployed in cloud environments.

---

## 🛠 Tech Stack

### 💻 Application Layer

* Django (Python Framework)
* HTML / CSS / Bootstrap
* Gunicorn (WSGI Server)
* Nginx (Reverse Proxy)

### ☁️ Cloud & AWS Services

* Amazon EC2
* Application Load Balancer (ALB)
* Auto Scaling Group (ASG)
* Amazon RDS (MySQL)
* Amazon S3
* Amazon CloudFront
* Amazon CloudWatch
* Amazon SNS
* VPC, IAM, Security Groups

---

## 🏗 Architecture Overview

### 🔄 Request Flow

User
→ CloudFront (CDN)
→ Application Load Balancer (ALB)
→ Auto Scaling Group (EC2 Instances)
→ Nginx
→ Gunicorn
→ Django Application
→ Amazon RDS (MySQL)

### 📊 Logging & Monitoring Flow

Application Logs
→ CloudWatch
→ SNS Alerts
→ Amazon S3 (Storage)

---

## ✨ Key Features

* ✔ High availability using ALB & Auto Scaling
* ✔ Secure networking with VPC
* ✔ Managed database using RDS
* ✔ CDN acceleration via CloudFront
* ✔ Monitoring & alerts using CloudWatch + SNS
* ✔ Centralized logging stored in S3
* ✔ Production-ready deployment

---

## ⚙️ Deployment Workflow

### 1️⃣ Infrastructure Setup

* Created VPC with public/private subnets
* Configured route tables and internet gateway
* Set up security groups for ALB, EC2, and RDS
* Created IAM roles

### 2️⃣ Application Deployment

* Installed Python, Nginx, and Gunicorn
* Configured Nginx as reverse proxy
* Deployed Django application
* Connected application with RDS

### 3️⃣ Load Balancing & Scaling

* Configured Application Load Balancer
* Created Auto Scaling Group
* Enabled health checks
* Configured launch templates

### 4️⃣ Monitoring & Alerts

* Enabled CloudWatch metrics
* Created alarms for CPU and instance health
* Configured SNS notifications

### 5️⃣ CDN & Storage

* Integrated CloudFront
* Configured S3 for static files and logs
* Applied caching policies

---

## 💻 Local Development Setup

### Prerequisites

* Python 3.x
* MySQL
* Git
* AWS Account

### Installation

```bash
git clone https://github.com/m-rahees/AWS_project.git
cd AWS_project

python -m venv env
env\Scripts\activate   # For Windows

pip install -r requirements.txt

python manage.py migrate
python manage.py runserver
```

Open in browser:
http://127.0.0.1:8000

---

## 🔐 Security Implementation

* VPC network isolation
* Private RDS instance
* IAM role-based access control
* Security group restrictions
* HTTPS via CloudFront
* CSRF protection
* Secure cookies

---

## 📊 Monitoring & Logging

* CloudWatch metrics & dashboards
* ALB health checks
* Auto scaling based on load
* SNS alerts (email notifications)
* Centralized logs stored in S3

---

## 📸 Screenshots

> Add your screenshots inside `/screenshots` folder

* Architecture Diagram
* CloudWatch Dashboard
* Application UI
* Alerts & Logs

---

## 🚀 Future Enhancements

* Infrastructure as Code using Terraform
* CI/CD pipeline (GitHub Actions / Jenkins)
* Docker containerization
* Kubernetes (EKS) deployment
* AWS WAF integration

---

## 👨‍💻 Author

**Muhammed Rahees**
DevOps / Cloud Enthusiast

* GitHub: https://github.com/m-rahees
* LinkedIn: https://linkedin.com/in/muhammed-rahees-a6815b376

---

## ⭐ Support

If you found this project helpful, consider giving it a ⭐ on GitHub!
