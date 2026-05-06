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

### AWS EKS Application Deployment Pipeline
Production-grade AWS infrastructure and CI/CD pipeline for deploying a containerized application to Kubernetes:

- VPC with public/private subnets across 3 availability zones, NAT Gateway and routing, provisioned via Terraform modules
- EKS cluster with managed node group in private subnets, ECR repository with lifecycle policy
- GitHub Actions CI/CD pipeline with OIDC authentication, no long-lived credentials stored anywhere
- Docker image built and pushed to ECR on every push to main, tagged with git commit SHA
- Helm chart with liveness/readiness probes, deployed to EKS via helm upgrade --install
- IAM roles with least-privilege S3 access for pods via IRSA
- Infrastructure is ephemeral, spun up with terraform apply and torn down with terraform destroy after each session

Repository: https://github.com/selimcelem/aws-eks-pipeline

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

---

Currently preparing for AWS Solutions Architect Associate and actively building a hands-on cloud engineering portfolio.
