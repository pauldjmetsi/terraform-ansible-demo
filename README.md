# terraform-ansible-demo
CI/CD pipeline example with Terraform and Ansible

## Architecture Overview
GitHub (Source + CI/CD)
   │
   ├── Terraform Plan → Apply  (provisions AWS infrastructure)
   │       │
   │       └── AWS (EC2, VPC, SGs, etc.)
   │
   └── Ansible Playbook (configures EC2 instances post-deployment)
           │
           └── Connects via SSH to AWS EC2 instances

