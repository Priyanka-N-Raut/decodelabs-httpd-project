**🚀 DecodeLabs Landing Page Deployment on AWS EC2**

A modern and responsive DecodeLabs technical landing page deployed on an AWS EC2 instance using Apache HTTPD Web Server.

This project demonstrates real-world cloud deployment of a static website using Infrastructure as a Service (IaaS).


📌**Project Overview**

This project includes:

✅ Creation of an AWS EC2 instance (Linux)

✅ Installation and configuration of Apache HTTPD

✅ Deployment of a static HTML/CSS landing page

✅ Hosting the website using a public IP address

✅ Security Group configuration for HTTP access (Port 80)


🛠 **Technologies Used**

AWS EC2 (Amazon Linux / Ubuntu)

Apache HTTPD

HTML5

CSS3

Linux Commands

SSH


☁️ **Deployment Steps**
1️⃣ Launch EC2 Instance

Select Amazon Linux / Ubuntu AMI

Choose instance type (t2.micro)

Configure Security Group:

Allow HTTP (Port 80)

Allow SSH (Port 22)


2️⃣ Connect to EC2 via SSH
ssh -i your-key.pem ec2-user@your-public-ip

3️⃣ Install Apache


For Amazon Linux:

sudo yum update -y
sudo yum install httpd -y
sudo systemctl start httpd
sudo systemctl enable httpd


For Ubuntu:

sudo apt update
sudo apt install apache2 -y
sudo systemctl start apache2

4️⃣ Deploy Website Files

Move your index.html file to:

/var/www/html/


Example:

sudo nano /var/www/html/index.html


Paste your website code and save.


5️⃣ Access the Website

Open in browser:

http://your-public-ip


Your DecodeLabs landing page will be live 🎉

📂 **Project Structure**
decodelabs-ec2-deployment/
│
├── index.html
└── README.md


✨ Features

Responsive design

Modern tech UI

Smooth scroll functionality

Apache Web Server hosting

Public cloud deployment


🎯 Learning Outcomes

Through this project, I learned:

How to launch and configure EC2 instances

How Apache serves static content

Security Group configuration

Linux server management

Real-world cloud deployment process


👩‍💻 **Author**

**Priyanka Raut**
Cloud & DevOps Enthusiast
Aspiring Cloud Engineer
