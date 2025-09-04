# terraform-lab-02-ec2
Terraform Lab 2 — Launch an EC2 instance on AWS

Terraform Lab 2 — Launch an EC2 Instance on AWS
Overview
This lab demonstrates how to use Terraform to provision an EC2 instance on AWS. The goal is to showcase Infrastructure as Code (IaC) principles for automating cloud resource creation.
Prerequisites
- AWS account with programmatic access enabled
- Terraform installed (v1.13+)
- AWS CLI installed and configured
- Visual Studio Code (or any code editor)
- GitHub account to store project files

Lab Execution Steps
Step 1: Initialize Terraform
Run the following command to initialize Terraform and download necessary provider plugins:
terraform init
Screenshot: [images/1.png]
Step 2: Validate Configuration
Validate the Terraform configuration to ensure there are no syntax errors:
terraform validate
Screenshot: [images/2.png]
Step 3: Plan Execution
Generate an execution plan to preview the resources that will be created:
terraform plan
Screenshot: [images/3.png]
Step 4: Apply and Launch EC2 Instance
Apply the configuration to provision the EC2 instance. When prompted, type 'yes' to confirm.
terraform apply
Screenshot: [images/4.png]
Step 5: Verify EC2 Instance
Once Terraform has finished, verify that the EC2 instance has been launched successfully by checking the AWS Management Console under EC2 → Instances.
Terraform Output Example:
instance_public_ip = 34.243.xxx.xxx
Screenshot: [images/5.png]
Configuration Details
- Region: eu-west-1 (Ireland)
- Instance Type: t2.micro (Free Tier eligible)
- AMI: Amazon Linux 2
- Resource Name: Terraform-Lab-02-EC2

Cleanup
To prevent unnecessary AWS charges, destroy the resources when you are finished with the lab:
terraform destroy
# type 'yes' when prompted
Screenshot: [images/6.png]
Skills Demonstrated
- Provisioning AWS resources with Terraform
- Terraform workflow: init → validate → plan → apply → destroy
- Managing EC2 instances declaratively
- GitHub documentation with evidence (screenshots + project files)

Author
Ime Ben
Cloud Security Engineer | AWS & Azure Specialist
GitHub: https://github.com/ime-cloud-sec-analyst
LinkedIn: https://www.linkedin.com/in/imeben
Email: imegcu55@gmail.com

