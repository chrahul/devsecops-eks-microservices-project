#  Table of Contents — DevSecOps on AWS EKS

> **Project:** End-to-End DevSecOps Pipeline — Deploying SecureBank (React + Spring Boot + MySQL) on AWS EKS

---

##  PHASE 1: Foundation & Prerequisites
- 1.1 Architecture Overview & Workflow Diagram
- 1.2 AWS Account Setup, IAM User & Access Keys
- 1.3 Tools Installation on Local Laptop (AWS CLI, kubectl, eksctl, Terraform, Helm, Git)
- 1.4 GitHub Account Setup & SSH Key Configuration
- 1.5 DockerHub Account Setup & Access Token
- 1.6 VS Code + GitHub Integration (Source Control, Extensions)

---

##  PHASE 2: Source Code Management
- 2.1 Fork/Clone the Sample Application (React Frontend + Spring Boot Backend)
- 2.2 Repository Structure & Branching Strategy (main, dev, feature)
- 2.3 Push Code from VS Code → GitHub
- 2.4 GitHub Webhooks Setup (for Jenkins triggers)

---

##  PHASE 3: Jenkins Server Setup on AWS EC2
- 3.1 Launch EC2 Instance (t2.large, Ubuntu 22.04, Security Groups)
- 3.2 Install Java 17, Jenkins, Docker, kubectl, AWS CLI, Trivy
- 3.3 Initial Jenkins Configuration & Plugin Installation
- 3.4 Configure Global Tools (Maven, JDK, NodeJS, Docker, SonarQube Scanner)
- 3.5 Configure Credentials (GitHub, DockerHub, AWS, SonarQube, Kubeconfig)

---

##  PHASE 4: Code Quality & Security Tools
- 4.1 SonarQube Server Setup on EC2 (separate instance)
- 4.2 SonarQube + Jenkins Integration (Quality Gates, Webhook)
- 4.3 Trivy Installation (FS Scan + Image Scan)
- 4.4 Nexus Repository Setup (for Maven artifacts) — *Optional*
- 4.5 OWASP Dependency Check Plugin

---

##  PHASE 5: AWS EKS Cluster Provisioning
- 5.1 EKS Architecture Deep Dive (Control Plane, Worker Nodes, VPC)
- 5.2 IAM Roles for EKS (Cluster Role, Node Role)
- 5.3 EKS Cluster Creation using `eksctl` (or Terraform)
- 5.4 Configure `kubeconfig` & Verify Cluster
- 5.5 Install AWS Load Balancer Controller
- 5.6 Install NGINX Ingress Controller (alternative path)
- 5.7 Install Metrics Server & Cluster Autoscaler

---

##  PHASE 6: Containerization
- 6.1 Dockerfile for React Frontend (Multi-stage build)
- 6.2 Dockerfile for Spring Boot Backend (Multi-stage build)
- 6.3 Local Docker Build & Test
- 6.4 Push Images to DockerHub

---

##  PHASE 7: Kubernetes Manifests & Helm Charts
- 7.1 Namespace, ConfigMaps, Secrets
- 7.2 Deployment & Service YAMLs (Frontend, Backend)
- 7.3 Ingress Resource (Path-based routing)
- 7.4 HPA (Horizontal Pod Autoscaler)
- 7.5 Persistent Volumes for Database
- 7.6 Helm Chart Packaging — *Optional*

---

##  PHASE 8: The Full CI/CD Pipeline (Jenkinsfile)
- 8.1 Pipeline Architecture & Stages Walkthrough
- 8.2 **Stage 1:** Git Checkout
- 8.3 **Stage 2:** Compile & Unit Test (Maven / npm)
- 8.4 **Stage 3:** SonarQube Code Analysis + Quality Gate
- 8.5 **Stage 4:** OWASP Dependency Check
- 8.6 **Stage 5:** Trivy Filesystem Scan
- 8.7 **Stage 6:** Build & Tag Docker Image
- 8.8 **Stage 7:** Trivy Image Scan
- 8.9 **Stage 8:** Push Image to DockerHub
- 8.10 **Stage 9:** Update K8s Manifests (Image Tag)
- 8.11 **Stage 10:** Deploy to EKS via kubectl/Helm
- 8.12 **Stage 11:** Email/Slack Notifications

---

##  PHASE 9: Monitoring & Observability
- 9.1 Prometheus Installation via Helm
- 9.2 Grafana Setup & Dashboards
- 9.3 Node Exporter & Blackbox Exporter
- 9.4 Application & Cluster Monitoring Dashboards
- 9.5 Alerting (AlertManager → Email/Slack)

---

##  PHASE 10: Testing & Validation
- 10.1 End-to-End Pipeline Run
- 10.2 Access Application via Ingress URL / Route53
- 10.3 Trigger a Code Change → Auto Deploy Verification
- 10.4 Load Testing & HPA Validation

---

##  PHASE 11: Cleanup & Cost Management
- 11.1 Tear Down EKS Cluster
- 11.2 Terminate EC2 Instances
- 11.3 Delete IAM Roles, Load Balancers, EBS Volumes
- 11.4 AWS Cost Best Practices

---

##  BONUS PHASE 12 (Optional)
- 12.1 ArgoCD GitOps Setup
- 12.2 Migrating from Jenkins-Push to ArgoCD-Pull Deployment
- 12.3 HTTPS with Cert-Manager + Let's Encrypt
- 12.4 AWS Secrets Manager Integration

---

##  Learning Outcomes

By completing this project, you will master:

-  AWS Cloud (EC2, EKS, RDS, IAM, ALB)
-  Kubernetes (Pods, Deployments, Services, Ingress, HPA)
-  Docker (Multi-stage builds, image optimization)
-  Jenkins CI/CD (Pipeline as Code, Webhooks)
-  DevSecOps (SonarQube, Trivy, OWASP Dependency Check)
-  Monitoring (Prometheus, Grafana)
-  Infrastructure as Code (Terraform, Helm)

---

##  Author

**Rahul Chaubey** | DevSecOps Architect & Trainer  
 rahulch.unix@gmail.com  
 [GitHub: @chrahul](https://github.com/chrahul)

---

##  License

This project is licensed under the MIT License — see the [LICENSE](LICENSE) file for details.