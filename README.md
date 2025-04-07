# Infrastructure as Code (IaC) on AWS

![AWS](https://img.shields.io/badge/AWS-CloudFormation-orange) ![CI/CD](https://img.shields.io/badge/CI%2FCD-Jenkins-blue) ![License](https://img.shields.io/badge/license-MIT-green)

## 🚀 Project Overview
This project automates the provisioning and management of cloud infrastructure on AWS using Infrastructure as Code (IaC) principles. It includes modular CloudFormation templates, CI/CD pipelines, monitoring, auto-scaling, and security best practices.

## 📁 Folder Structure
```
repo-root/
├── templates/         # AWS CloudFormation templates
├── scripts/           # Shell scripts for deployment
├── jenkins/           # Jenkins pipeline
├── .github/workflows/ # GitHub Actions workflow
├── README.md          # Project overview and setup
├── DEPLOYMENT_GUIDE.md          # Step-by-step deployment guide
├── TROUBLESHOOTING.md           # Fixes for common errors
├── MAINTENANCE.md               # Long-term operations
```

## 🔧 Tech Stack
- **AWS CloudFormation** – Define and manage infrastructure
- **Jenkins / GitHub Actions** – CI/CD automation
- **AWS CloudWatch** – System monitoring and alerts
- **IAM** – Identity and access management
- **Auto Scaling & Load Balancing** – Resilient and scalable setup

## 🛠️ Getting Started
### Prerequisites
- AWS CLI installed and configured
- IAM credentials with CloudFormation and EC2 access
- Jenkins server or GitHub repository setup for automation

### Installation
```bash
git clone https://github.com/yourusername/iac-aws-infra.git
cd iac-aws-infra
./scripts/deploy.sh templates/vpc.yaml my-vpc-stack
```

## 🚦 CI/CD Pipeline
- Validates CloudFormation templates using `cfn-lint`
- Deploys templates automatically to AWS
- Monitors system status and supports rollback on failure

## 📊 Monitoring & Maintenance
- CloudWatch Alarms for EC2, auto-scaling, and cost tracking
- Routine IAM policy reviews
- Logs archiving and audit management

## 🧠 Lessons Learned
- Modular infrastructure improves reusability and clarity
- Security configurations require constant tuning
- CI/CD automation significantly reduces manual errors

## 📄 License
This project is licensed under the MIT License. See the LICENSE file for more details.
