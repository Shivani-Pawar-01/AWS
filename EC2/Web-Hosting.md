# 🌐 Web Hosting using Terminal & Shell Scripting (AWS Practical)

This document explains how to host a website on an EC2 instance using:
1. Terminal (manual setup)  
2. Shell scripting (automated setup using User Data)

---

# 🚀 Part 1: Web Hosting using Terminal

## 📌 Step 1: Launch & Connect to Instance
- Launch EC2 instance  
- Connect using SSH  
![Step 1 Screenshot](step1.png)

---

## 📌 Step 2: Run Commands on Terminal

Execute the following commands:

```bash id="a1b2c3"
sudo -i
apt update -y
apt install nginx -y
cd /var/www/html
ls
vim index.html
