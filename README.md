#  DevSecOps on AWS EKS — SecureBank Project

> **End-to-End DevSecOps Pipeline:** Deploying a Production-Grade Banking Application on AWS EKS using Jenkins, Docker, Kubernetes, and Modern Security Tools

[![AWS](https://img.shields.io/badge/AWS-EKS-orange?logo=amazon-aws)](https://aws.amazon.com/eks/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-1.28-blue?logo=kubernetes)](https://kubernetes.io/)
[![Jenkins](https://img.shields.io/badge/Jenkins-CI%2FCD-red?logo=jenkins)](https://www.jenkins.io/)
[![Docker](https://img.shields.io/badge/Docker-Containerized-blue?logo=docker)](https://www.docker.com/)
[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

##  About The Project

**SecureBank** is a cloud-native banking application built to demonstrate a **complete real-world DevSecOps pipeline** on AWS. This project takes you from **zero to production**, deploying a 3-tier microservices application on Amazon EKS with full CI/CD automation, security scanning, and observability.

This is **not just a demo** — it's a hands-on, step-by-step learning journey covering every tool, command, and decision a Principal DevOps Architect would make in real production environments.

---

##  Architecture

![SecureBank Architecture](docs/architecture-diagram.png)

###  Three-Tier Application Design

| Tier | Technology | Purpose | Port |
|------|------------|---------|------|
| **Frontend** | React.js 18 | User Interface | 3000 |
| **Backend** | Spring Boot 3 + Java 17 | REST APIs & Business Logic | 8080 |
| **Database** | MySQL 8.0 (AWS RDS) | Data Persistence | 3306 |

---

##  Tech Stack

###  **Cloud & Infrastructure**
- **AWS EKS** — Managed Kubernetes Cluster
- **AWS EC2** — Jenkins, SonarQube Servers
- **AWS RDS** — MySQL Database
- **AWS ALB** — Application Load Balancer
- **AWS IAM** — Identity & Access Management

###  **CI/CD & Automation**
- **Jenkins** — Continuous Integration / Continuous Deployment
- **GitHub** — Source Code Management & Webhooks
- **DockerHub** — Container Image Registry

###  **Container Orchestration**
- **Docker** — Containerization
- **Kubernetes** — Container Orchestration
- **Helm** — Kubernetes Package Manager
- **NGINX Ingress Controller** — Traffic Routing

###  **DevSecOps Tools**
- **SonarQube** — Static Code Analysis
- **Trivy** — Container & Filesystem Vulnerability Scanning
- **OWASP Dependency Check** — Software Composition Analysis

###  **Monitoring & Observability**
- **Prometheus** — Metrics Collection
- **Grafana** — Dashboards & Visualization

###  **Application Stack**
- **React.js** — Frontend Framework
- **Spring Boot** — Backend Framework
- **MySQL** — Relational Database
- **Maven** — Build Tool

---

##  Project Roadmap

This project is organized into **12 phases**, each in its own folder. See [Table of Contents](ToC.md) for the complete structure.

| Phase | Topic | Status |
|-------|-------|--------|
| [Phase 1](phase-01-prerequisites/) | Foundation & Prerequisites |  In Progress |
| [Phase 2](phase-02-source-code/) | Source Code Management |  Upcoming |
| [Phase 3](phase-03-jenkins-setup/) | Jenkins Server Setup on EC2 |  Upcoming |
| [Phase 4](phase-04-security-tools/) | Code Quality & Security Tools |  Upcoming |
| [Phase 5](phase-05-eks-cluster/) | AWS EKS Cluster Provisioning |  Upcoming |
| [Phase 6](phase-06-docker/) | Containerization |  Upcoming |
| [Phase 7](phase-07-k8s-manifests/) | Kubernetes Manifests & Helm |  Upcoming |
| [Phase 8](phase-08-cicd-pipeline/) | Full CI/CD Pipeline |  Upcoming |
| [Phase 9](phase-09-monitoring/) | Monitoring & Observability |  Upcoming |
| [Phase 10](phase-10-testing/) | Testing & Validation |  Upcoming |
| [Phase 11](phase-11-cleanup/) | Cleanup & Cost Management |  Upcoming |
| [Phase 12](phase-12-bonus-argocd/) | Bonus: ArgoCD GitOps |  Upcoming |

---

##  What You'll Learn

By following this project end-to-end, you'll gain hands-on expertise in:

-  Designing **3-tier microservices architecture** on AWS
-  Provisioning **EKS clusters** using `eksctl` and Terraform
-  Building **multi-stage Docker images** for production
-  Writing **declarative Jenkinsfiles** with security gates
-  Implementing **DevSecOps best practices** (SAST, SCA, image scanning)
-  Deploying applications using **Kubernetes manifests & Helm charts**
-  Setting up **monitoring stacks** with Prometheus & Grafana
-  Managing **secrets, RBAC, and ingress** in production K8s
-  Automating **end-to-end deployments** with GitHub Webhooks

---

##  Quick Start

### Prerequisites

Before starting, ensure you have:

-  A laptop with **Git Bash** (Windows) / Terminal (Mac/Linux)
-  A **GitHub account**
-  An **AWS account** (Free Tier eligible)
-  A **DockerHub account**
-  **VS Code** installed

### Clone This Repository

```bash
git clone git@github.com:chrahul/devsecops-eks-microservices-project.git
cd devsecops-eks-microservices-project
```

### Follow the Phases

Start with [Phase 1](phase-01-prerequisites/README.md) and progress sequentially. Each phase has its own README with step-by-step instructions.

---

##  Repository Structure

devsecops-eks-microservices-project/
├── docs/                          # Architecture diagrams & screenshots
├── application-source-code/       # React frontend + Spring Boot backend
├── phase-01 to phase-12/          # 12 sequential learning phases
├── scripts/                       # Reusable shell scripts
├── README.md                      # You are here!
├── ToC.md                         # Detailed Table of Contents
├── .gitignore                     # Git ignore rules (DevSecOps grade)
└── LICENSE                        # MIT License

---

##  Contributing

This is a learning project — contributions, suggestions, and feedback are warmly welcomed!

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add: improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

##  Author

**Rahul Chaubey**  
*DevSecOps Architect & Trainer*

-  Email: rahulch.unix@gmail.com
-  GitHub: [@chrahul](https://github.com/chrahul)

---

##  License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## ⭐ Show Your Support

If this project helps you learn DevSecOps, please **star ⭐ the repository** — it motivates further updates and helps other learners discover it!

---

##  For Students

This repository is designed as a **complete learning resource**. Each phase is self-contained but builds on previous ones. **Don't skip phases** — every step teaches something fundamental!

>  **Mantra:** *"Slow is smooth, smooth is fast. Build right, build once."*

---

**Happy Learning! **