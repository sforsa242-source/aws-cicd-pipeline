# 🔄 AWS CI/CD Pipeline

Production-grade CI/CD pipeline templates for deploying applications to AWS using GitHub Actions, CodePipeline, and CodeBuild. Supports Lambda, ECS, and static site deployments.

## 🎯 Pipeline Templates

### 1. Serverless Deployment (Lambda + SAM)
Automated build, test, and deploy for serverless applications.

### 2. Container Deployment (ECS Fargate)
Docker build, ECR push, and ECS service update with blue/green deployments.

### 3. Static Site (S3 + CloudFront)
Build, deploy to S3, and invalidate CloudFront cache.

### 4. Infrastructure (Terraform)
Plan, validate, and apply Terraform changes with state management.

## 📁 Pipeline Files

```
.github/workflows/
├── serverless-deploy.yml    # Lambda/SAM deployment
├── ecs-deploy.yml           # Container deployment
├── static-site.yml          # S3/CloudFront deployment
└── terraform.yml            # Infrastructure changes
```

## 🔒 Security

- OIDC authentication (no long-lived AWS credentials)
- Environment-based approvals for production
- Automated security scanning (Trivy, Bandit)
- Dependency vulnerability checks (Dependabot)
- Least-privilege IAM roles per pipeline

## 📄 License

MIT License
