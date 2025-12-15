# DevOps / Cloud Engineering Portfolio Project

> **Important:** This repository is a **personal DevOps learning & portfolio project**.  
> It is **not a production system** and **not an official fork maintained by the OpenTelemetry project**.

---

## 📌 Project Purpose

This repository is a **DevOps-focused portfolio project** created to demonstrate my practical skills in:

- Infrastructure as Code (Terraform)
- AWS Cloud (VPC, EKS, IAM, networking)
- Kubernetes (EKS-based deployments)
- CI/CD pipelines
- Observability & cloud-native tooling (based on OpenTelemetry Demo)

The application layer is based on the **OpenTelemetry Astronomy Shop Demo**, which provides a realistic microservices environment.  
My **main focus is the infrastructure, automation, and deployment**, not application development.

---

## 🧠 Why this project exists

Recruitment processes for **DevOps / Cloud / Platform Engineer** roles often require:

- Real-world infrastructure examples
- Terraform modules and state management
- Kubernetes cluster provisioning
- CI/CD automation
- Clear, reproducible setup

This repository exists **only to showcase these skills** in a realistic cloud scenario.

---

## 🏗️ Current State

### ✅ Implemented

- **Terraform-based AWS infrastructure**
  - Remote Terraform state (S3 + DynamoDB locking)
  - Custom VPC (public & private subnets, NAT Gateways)
  - Amazon EKS cluster
  - Managed node groups
  - Modular Terraform structure (`vpc`, `eks`)

- Clean separation of:
  - backend state configuration
  - reusable Terraform modules
  - environment variables

---

### 🚧 Planned / In Progress

- Kubernetes manifests deployment to EKS
- Helm-based installation
- CI/CD pipeline (GitHub Actions)
  - Terraform validation & plan
  - Infrastructure deployment
  - Kubernetes rollout
- Observability stack integration
  - OpenTelemetry Collector
  - Metrics / logs / traces
- Security best practices
  - IAM least privilege
  - Kubernetes RBAC

---

## 🧰 Tech Stack

- **Cloud:** AWS
- **IaC:** Terraform
- **Container Orchestration:** Kubernetes (EKS)
- **CI/CD:** GitHub Actions (planned)
- **Observability:** OpenTelemetry
- **Networking:** VPC, Subnets, NAT, IGW

---

## 📁 Repository Structure (DevOps part)

```
eks-install/
├── backend/          # Remote Terraform state (S3 + DynamoDB)
├── modules/
│   ├── vpc/          # Custom VPC module
│   └── eks/          # EKS cluster & node groups
├── main.tf           # Infrastructure composition
├── variables.tf      # Input variables
├── outputs.tf        # Outputs
```

---

## ⚠️ Disclaimer

- This project is **for educational and recruitment purposes only**.
- Resource names, defaults, and configurations are simplified.
- Costs are not optimized for production usage.
- No SLA, security hardening, or enterprise governance is implied.

---

## 📎 Credits

- Application layer based on: **OpenTelemetry Astronomy Shop Demo**
- Original project: https://opentelemetry.io/docs/demo/


