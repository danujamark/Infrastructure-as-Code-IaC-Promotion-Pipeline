# Infrastructure-as-Code-IaC-Promotion-Pipeline
Infrastructure as Code (IaC) project implementing Terraform, CloudFormation, CI/CD pipelines, environment promotion workflows, and automated AWS infrastructure deployment.
## Overview

This project demonstrates the implementation of an Infrastructure as Code (IaC) Promotion Pipeline using:

- AWS CloudFormation
- Terraform
- GitHub Actions
- Amazon S3
- Amazon CloudFront

The solution automates infrastructure deployment across development and production environments while applying governance controls such as approval gates and drift detection.

The project also demonstrates how Infrastructure as Code maintains infrastructure consistency by detecting and correcting manual configuration drift.

---

## Project Objectives

- Automate AWS infrastructure deployments
- Implement Infrastructure as Code practices
- Build CI/CD deployment pipelines
- Promote infrastructure safely between environments
- Implement approval-based production deployment
- Demonstrate infrastructure drift detection and recovery
- Apply DevOps automation concepts

---

## Technologies Used

- AWS CloudFormation
- Terraform
- GitHub Actions
- Amazon S3
- Amazon CloudFront
- GitHub Environments
- CI/CD Pipelines

---

## Architecture Components

- CloudFormation Templates
- Terraform Modules
- GitHub Actions Workflow
- S3 Static Website Hosting
- CloudFront Distribution
- Environment Promotion Pipeline
- Approval Gates
- Drift Detection Workflow

---

## Infrastructure Workflow

```text
Developer Commit
       ↓
GitHub Repository
       ↓
GitHub Actions Pipeline
       ↓
Development Deployment
       ↓
Approval Gate
       ↓
Production Deployment
       ↓
Drift Detection & Recovery
```

---

## Repository Structure

```text
.github/workflows/
cloudformation/
modules/
environments/dev/
environments/pro/
```

---

## Tasks Completed

### CloudFormation Deployment
- Created CloudFormation template
- Provisioned:
  - S3 Bucket
  - CloudFront Distribution
- Generated website output URL

### Static Website Hosting
- Uploaded index.html
- Configured S3 website hosting
- Verified CloudFront delivery

### Terraform Implementation
- Recreated infrastructure using Terraform
- Organized reusable modules
- Configured environment-based deployment structure

### GitHub Actions CI/CD Pipeline
- Configured automated deployment workflow
- Enabled environment promotion process
- Connected GitHub repository with AWS deployment

### GitHub Secrets Configuration
- Added AWS access credentials securely
- Configured GitHub repository secrets

### Approval Gate Implementation
- Configured GitHub Environments
- Enabled required reviewer approval
- Protected production deployment workflow

### Drift Detection Demonstration
- Manually modified website content from AWS Console
- Simulated infrastructure drift condition

### Drift Recovery
- Restored correct infrastructure state using IaC
- Triggered pipeline redeployment
- Verified infrastructure consistency restoration

---

## Deployment Features

### Development Environment
- Automatic deployment enabled
- Fast testing workflow

### Production Environment
- Manual approval required
- Controlled promotion workflow

### Drift Management
- Manual change detection
- Infrastructure reconciliation through IaC

---

## Example Use Case

### Initial Deployment
```text
Version v1 deployed successfully
```

### Manual Drift
```text
Website manually changed from AWS Console
"HACKED FROM CONSOLE"
```

### Drift Fix
```text
Git commit: Fix drift
Pipeline redeployed infrastructure
Website restored to intended state
```

---

## Security & Governance Features

- Environment separation
- Approval-based production deployment
- Version-controlled infrastructure
- Automated deployment pipeline
- Drift correction process
- Infrastructure consistency enforcement

---

## Validation Performed

- Verified CloudFormation deployment
- Tested Terraform provisioning
- Confirmed GitHub Actions execution
- Verified approval gate functionality
- Tested S3 website hosting
- Verified CloudFront access
- Simulated infrastructure drift
- Verified drift recovery process

---

## Learning Outcome

This project demonstrates practical knowledge of:

- Infrastructure as Code principles
- CloudFormation and Terraform usage
- CI/CD pipeline implementation
- GitHub Actions automation
- Environment promotion workflows
- Drift detection and reconciliation
- DevOps governance practices
- AWS infrastructure automation
- Production deployment control
