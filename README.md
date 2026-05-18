# AWS DevOps CI/CD Reference Architecture Project

##  Project Purpose
This repository documents a **reference AWS DevOps architecture and CI/CD pipeline design**
for a scalable 3-tier application.  
This project is created for **learning, understanding system design, and interview preparation**.

 Note: This is a **design & documentation-focused project**, not a fully implemented live deployment.

---

##  Architecture Overview
The architecture demonstrates:
- Frontend & Backend CI/CD pipelines
- Multi-AZ 3-tier AWS architecture
- Secure networking using public & private subnets
- Scalable application and database layers


<img width="1258" height="657" alt="3" src="https://github.com/user-attachments/assets/41e73c44-5e13-4b8d-a1f0-773405290171" />

##  CI/CD Pipeline Design
- Source Control: GitHub
- CI: AWS CodeBuild
- CD: AWS CodeDeploy
- Orchestration: AWS CodePipeline

<img width="1264" height="652" alt="2" src="https://github.com/user-attachments/assets/052f7ffa-4bd1-44ad-b509-0c9021602064" />

##  Frontend CI/CD Flow
- GitHub → CodeBuild → CodeDeploy → Presentation Tier EC2
- React frontend served via NGINX

##  Backend CI/CD Flow
- GitHub → CodeBuild → CodeDeploy → Application Tier EC2
- Node.js backend managed using PM2

 <img width="1248" height="640" alt="1" src="https://github.com/user-attachments/assets/b67947c7-accd-48a7-afaf-91fdc72e3799" />

 ## Security Considerations
- Bastion host for SSH access
- Private subnets for App & DB tiers
- HTTPS using ACM
- Security Groups with least privilege

## Learning Outcomes
- Understanding AWS CI/CD services
- Designing highly available architectures
- Separation of frontend & backend pipelines
- Secure cloud networking concepts

## how i implement this project don't worry i have created file checkout this :)  (step-by-step-implementation.md)


