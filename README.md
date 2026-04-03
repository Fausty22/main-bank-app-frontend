# Banking App — Frontend

![Docker](https://img.shields.io/badge/Container-Docker-blue)
![Nginx](https://img.shields.io/badge/Server-Nginx-green)
![ECR](https://img.shields.io/badge/Registry-Amazon_ECR-orange)

## Overview
Frontend service for the three-tier banking application. Built with HTML/CSS, served via Nginx, containerised with Docker and deployed to AWS EKS.

## Features
- Responsive banking dashboard UI
- Real-time infrastructure status display
- Payments, Analytics, Security and Global banking services
- Health check endpoint

## Tech Stack
- **Frontend:** HTML5, CSS3
- **Web Server:** Nginx Alpine
- **Container:** Docker
- **Registry:** Amazon ECR
- **Deployment:** Kubernetes on AWS EKS

## CI/CD Pipeline
Every push to main automatically:
1. Builds Docker image
2. Pushes to Amazon ECR
3. Argo CD detects change and deploys to EKS

## Local Development
```bash
# Build image
docker build -t faustina-frontend .

# Run locally
docker run -p 8080:80 faustina-frontend

# Open browser
http://localhost:8080
```

## Author
**Faustina Nwokolo** — Cloud & DevOps Engineer