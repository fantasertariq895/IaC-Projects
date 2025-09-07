
---

## ✅ Project 2: `static_website_amplify/`

**README Path:** `/IaC-Projects/static_website_amplify/README.md`

```md
# Host Static React Website with AWS Amplify Gen 2

This project deploys a static frontend React website using AWS Amplify Gen 2 with full CI/CD from GitHub.

## 🧠 Concepts Covered

- Amplify Gen 2 sandbox & CLI (`ampx`)
- SSO authentication setup with AWS CLI
- GitHub → Amplify hosting integration
- Frontend app bootstrapped with `Vite + React`

## 📁 Project Structure

- `static_website_amplify/`  
  └── Contains all frontend code and `.ampx` config
- AWS Amplify environment connected to GitHub repo
- Profile created via `aws configure sso`

## 🛠️ Technologies Used

- React + Vite
- AWS Amplify Gen 2 (sandbox & CLI)
- AWS IAM Identity Center (SSO)
- GitHub Actions (CI/CD optional)
- AWS CLI v2

## ⚙️ SSO Setup Steps Done

- SSO URL: `https://d-9066252cb5.awsapps.com/start`
- Region: `us-east-1`
- Created SSO user: `amplify-admin`
- Attached `AmplifyBackendDeployFullAccess` policy
- Configured SSO profile using `aws configure sso`

## 🚀 Deployment Instructions

```bash
# Configure profile
aws configure sso

# Start Amplify sandbox (from project root)
npx ampx sandbox --profile fantaser
