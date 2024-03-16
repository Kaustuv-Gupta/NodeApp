# Problem Description
Creating a CICD pipeline dor deploying a NodeJs App using jenkins building the infrastructure using IaaC (Terraform) in AWS.

## Steps
- VPC setup on AWS which includes public & private subnets (multi-AZ) using Terraform
- Use Ansible for configuration management, for instance, installing ‘Docker’ on the hosts
- Use Jenkins to build the CICD pipeline for the deployment of node applications
- App - For running the containerized version of the app
- Bastion - In a public subnet for accessing private instances
- ALB for accessing App and Jenkins
- A Jenkins pipeline to build nodejs app image & deploy it on the app instance
- Use Github as a codebase repository and ECR for docker image repository