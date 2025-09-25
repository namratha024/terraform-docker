# Terraform Docker IaC Project

## Objective
This project demonstrates **Infrastructure as Code (IaC)** using Terraform to provision a local Docker container.  
The goal is to automate container creation and management using Terraform on a Windows machine.

---

## Project Overview
- **Tool:** Terraform  
- **Container:** Docker (Nginx web server)  
- **OS:** Windows 10/11  
- **Outcome:** Provision an Nginx container running on a local port.

---

## Steps to Run the Project

1. **Clone the Repository**
```bash
git clone https://github.com/namratha024/terraform-docker.git
cd terraform-docker
Initialize Terraform

terraform init


Plan the Infrastructure

terraform plan


Apply Configuration

terraform apply -auto-approve


Verify the Container

docker ps


Open a browser and go to http://localhost:8081 (or the port defined in main.tf)

You should see the Nginx welcome page.

Check Terraform State

terraform state list


Destroy the Infrastructure

terraform destroy -auto-approve

Repo Structure
terraform-docker/
│── main.tf             # Terraform configuration file
│── .gitignore          # Ignores local Terraform state and temporary files
│── README.md           # Project documentation

Screenshots / Logs

Include:

terraform init

terraform plan

terraform apply

docker ps output

Nginx page in browser

terraform state list

terraform destroy
