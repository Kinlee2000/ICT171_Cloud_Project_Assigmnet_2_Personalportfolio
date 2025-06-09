# Server Setup Guide

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
```
---

## 3. Update System and Install Apache2

```bash
sudo apt update
sudo apt install apache2 -y
sudo systemctl enable apache2
sudo systemctl start apache2
```
---
## 4. upload and deploy Website Files 
1. Install unzip
  ```bash
  sudo apt install unzip
  ```
2. upload cloud_html.zip using SCP
3. Unzip and move files.
  ```bash
  unzip cloud_html.zip
  sudo cp -r cloud_html/* /var/www/html/
  sudo chown -R www-data:www-data /var/www/html/
  ```
---
## 5. configure Apache Virtual Host
create Virtual host config
``bash
sudo nano /etc/apache2/sites-available/gyeltshen.net.conf
```

