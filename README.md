# Ansible-VM-Monitor

# Infrastructure as Code – Automated VM Provisioning & Configuration

## 📌 Project Overview
This project demonstrates an **Infrastructure as Code (IaC)** solution to automate **virtual machine provisioning and configuration** using **Terraform** and **Ansible**.  
It enables users to request VMs with custom specifications while ensuring security, consistency, and compliance within the internal infrastructure.

The entire VM lifecycle—from provisioning to software installation and OS hardening—is fully automated, reducing manual effort and setup time.

---

## 🛠 Tools & Technologies
- **Terraform** – VM provisioning and infrastructure automation  
- **Ansible** – Post-provisioning configuration management  
- **VMware / Cloud Provider API** – VM creation and management  
- **Linux & Windows Server** – Target operating systems  
- **Git** – Version control for IaC  
- **YAML** – Ansible playbooks and configurations  
- **Bash / Python** – Optional scripting for automation tasks  

---

## 🚀 Features
- Automated VM provisioning using Terraform templates
- Parameterized deployments for creating multiple VMs with a single configuration change
- Automated OS and software configuration using Ansible
- Pre-installed development, monitoring, and security tools
- OS-level hardening based on company security policies
- Centralized, version-controlled IaC repository
- Faster provisioning time (from days to under **1 hour**)

---

## 🧩 Architecture Workflow
1. User defines VM requirements (CPU, RAM, storage, OS type)
2. Terraform provisions VMs using reusable templates
3. Ansible configures newly created VMs:
   - Installs required software
   - Applies security hardening
   - Manages users, groups, and permissions
4. Infrastructure remains within internal network for security compliance

---

## 📂 Project Structure
```bash
.
├── terraform/
│   ├── main.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── terraform.tfvars
├── ansible/
│   ├── playbooks/
│   │   ├── setup.yml
│   │   ├── security.yml
│   └── roles/
├── scripts/
│   └── helper.sh
├── README.md
