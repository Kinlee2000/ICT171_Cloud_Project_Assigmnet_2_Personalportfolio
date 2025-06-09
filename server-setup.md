# Server ssetup guide
This document provides all the steps required to build the Personal Portfolio website hosted on AWS EC2.

---
## 1. Launch EC2 Instance

- Provider: AWS
- Instance Type: t2.micro (Free Tier eligible)
- OS: Ubuntu Server 22.04 LTS
- Security Group: Open ports 22 (SSH), 80 (HTTP), and 443 (HTTPS)

---

## 2. SSH Into the Server

```bash
ssh -i "your-key.pem" ubuntu@<EC2_PUBLIC_IP>
---
## 3.Update system and install Apache

```bash 
sudo apt update
sudo apt install apache2 -y
sudo systemctl enable apache2
sudo systemctl start apache2
---
Check Apache:

```bash
sudo systemctl status apache2

