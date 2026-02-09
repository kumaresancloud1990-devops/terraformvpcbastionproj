# Terraform VPC with Bastion Host

This project creates an AWS VPC using Terraform with:
- Public subnet
- Private subnet
- Internet Gateway
- NAT Gateway
- Bastion EC2 instance (Ubuntu, t3.micro)

## Architecture
- Bastion host in public subnet
- Private subnet has internet access via NAT
- SSH access to bastion allowed only from my public IP

## Prerequisites
- Terraform >= 1.3
- AWS CLI configured
- An existing EC2 key pair

## How to use

```bash
terraform init
terraform plan
terraform apply
