# aws-cli-workstation-cft
AWS Cloudformation templates that creates a Linux CLI workstation with common devops tools pre-installed

This project aims to create a simple CLI Linux environment that you can spin up quickly with Cloudformation,
use to deploy some code with Ansible/Terraform/CDK/etc and then delete it again when you no longer need it.

The EC2 instance this creates is setup to use AWS Session Manager Connect for console access. Simply select the 
instance, click 'Connect' in the upper right, choose the 'Session Manager' tab, and click 'Connect' to get a 
CLI console. 

The EC2 instance is currently setup with an Admin IAM role to simplify use. In corporate environments this should 
be scoped down to the minimum required permissions.  

### Installed tools aws-cli-al2023-x86-64-cft.yaml
- git
- htop
- wget and curl (these come by default with AL2023)
- Docker
- Ansible
- Terraform
- Python3 (comes by default with AL2023)
- NPM
- NodeJS
- Typescript
- AWS CDK

### Installed tools aws-cli-al2023-arm64-cft.yaml
- git
- htop
- wget and curl (these come by default with AL2023)
- Docker
- Ansible
- Terraform
- Python3 (comes by default with AL2023)
- NPM
- NodeJS
- Typescript
- AWS CDK