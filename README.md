# ICT171_Assigmnet_2_Personalportfolio
personalPortfolio 

# ICT171 Cloud Server Project - Kinley Gyeltshen | student ID: 35459148 

## 🌐 Live Server
- http://www.gyeltshen.net

## 🎥 Video Explainer
https://drive.google.com/file/d/1p6N11vPp4qQIYXKYo6fP72vZNDkr-Crb/view?usp=drive_link 

## About the Project
This project is part of ICT171 - Introduction to Server Environments and Architectures.  
It demonstrates how to set up a personal portfolio website using an EC2 Ubuntu server, Apache2, and a domain name.

## Technologies Used
- AWS EC2 (t2.micro)
- Ubuntu 22.04 LTS
- Apache2
- GitHub
- Cloudflare (for DNS)

## Setup Instructions (Short Summary)
1. Create an EC2 instance
2. Install Apache2: `sudo apt update && sudo apt install apache2`
3. Upload your portfolio html.zip to `/var/www/html`
4. Configure DNS via Cloudflare to point your domain to the EC2 public IP
5. Add SSL with Certbot

Detailed documentation can be found in `35459148_kinley_gyeltshen_ICT171cloudproject.pdf`.

## License
MIT License 
