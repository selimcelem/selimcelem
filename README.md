# Selim Çelem

AWS Certified Cloud Practitioner with a background in BIM engineering, now focused on cloud infrastructure, automation, and reproducible deployment workflows.

## Core Focus

- AWS infrastructure and automation
- Infrastructure as Code with Terraform
- CI/CD with GitHub Actions
- Container deployments with Docker, ECR, and ECS Fargate
- Serverless architectures on AWS
- Production-minded IAM, logging, and operational workflows

## Featured Projects

### Q-Atelier — Production AWS Website & Booking System
Full-stack serverless AWS platform for a live bridal atelier in the Netherlands:
- S3 + CloudFront CDN with custom domain (q-atelier.nl) and ACM SSL
- API Gateway + Lambda (Node.js) for booking management
- DynamoDB for appointment storage with token-based confirmation flow
- Resend API for transactional email with .ics calendar attachments
- Terraform IaC with remote state, modular structure, GitHub Actions CI/CD
- PENDING → ACCEPT / REJECT / RESCHEDULE booking flow with secure email links

Live: https://www.q-atelier.nl
Repository: https://github.com/selimcelem/q-atelier

### AWS SAA-C03 Practice App

Cross-platform Android/Windows quiz app for AWS exam preparation, backed by a full serverless AWS infrastructure:

* Cognito (Google OAuth, PKCE, Identity Pools with per-user IAM scoping)
* S3 for score sync and question reporting
* Lambda + EventBridge for scheduled digest email notifications via SNS
* Terraform IaC, GitHub Actions CI/CD
* .NET MAUI (Android + Windows)

Repository: https://github.com/selimcelem/aws-saa-c03-practice-app

### Mini Cloud Deployment Platform

Small AWS deployment platform for a containerized FastAPI application, built to demonstrate a production-style cloud workflow:

- Terraform with separated bootstrap and platform layers
- Remote state in S3 with DynamoDB locking
- Docker image build and push to Amazon ECR
- GitHub Actions push-to-deploy workflow
- Amazon ECS Fargate behind an Application Load Balancer
- CloudWatch logging, least-privilege CI/CD IAM, and ECR lifecycle cleanup

Repository: https://github.com/selimcelem/mini-cloud-deployment-platform

### Cloud Resume Challenge (AWS)

Production-ready serverless AWS platform built with:

- S3 + CloudFront + Route 53
- API Gateway + Lambda + DynamoDB
- Terraform (Infrastructure as Code)
- GitHub Actions CI/CD

Live: https://selimcelem.com  
Backend: https://github.com/selimcelem/cloud-resume-challenge  
Frontend: https://github.com/selimcelem/cloud-resume-frontend  

---

Currently preparing for AWS Solutions Architect Associate and building hands-on cloud engineering portfolio projects.
