# EC2 Instance with Custom VPC using Terraform

This project provisions an EC2 instance inside a custom VPC using Terraform. It includes setup for internet access via an Internet Gateway and public subnet routing.

## 📁 Files Included

- `main.tf` – Contains provider, VPC, subnet, EC2 instance definitions
- `variables.tf` – All input variables (e.g., CIDR blocks, instance type)
- `outputs.tf` – Output IP address or resource IDs
- `terraform.tfvars` – Custom variable values (optional)

## ☁️ AWS Resources Created

- VPC with defined CIDR block
- Public Subnet
- Internet Gateway
- Route Table with default route to IGW
- EC2 Instance (Amazon Linux 2 or Ubuntu)
- Security Group allowing SSH (port 22)

## 🛠️ Technologies Used

- Terraform v1.7+
- AWS EC2, VPC, IGW
- AWS CLI (optional)
- Git/GitHub for version control

## 🚀 How to Deploy

```bash
terraform init
terraform plan
terraform apply
