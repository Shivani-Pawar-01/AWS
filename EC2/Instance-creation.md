# 💻 EC2 Instance Launching (AWS Practical)

This document explains the step-by-step process of launching an EC2 instance in AWS.

---

## 📌 Step 1: Click on "Launch Instance"
Go to EC2 Dashboard and click **Launch Instance**  
![Step 1 Screenshot](step1.png)

---

## 📌 Step 2: Give Instance Name
Provide a name tag for the instance  
![Step 2 Screenshot](step2.png)

---

## 📌 Step 3: Select AMI
Choose an operating system (Amazon Machine Image)  
![Step 3 Screenshot](step3.png)

---

## 📌 Step 4: Select Instance Type
- Example: `t3.micro` (Free tier eligible)  
![Step 4 Screenshot](step4.png)

---

## 📌 Step 5: Configure Key Pair
- Select existing or create new key pair  
- Used for secure login (SSH)  
![Step 5 Screenshot](step5.png)

---

## 📌 Step 6: Configure Security Group
- Define firewall rules (SSH, HTTP, etc.)  
- Controls inbound/outbound traffic  
![Step 6 Screenshot](step6.png)

---

## 📌 Step 7: Configure Storage
- Define storage size (EBS volume)  
- Option to launch multiple instances with same configuration  
![Step 7 Screenshot](step7.png)

---

## 🚀 Step 8: Launch Instance
Click **Launch Instance**

---

## ✅ Step 9: Instance Created
EC2 instance is successfully created and running  
![Step 8 Screenshot](step8.png)

---

## 🧠 Important Notes
- Use `t3.micro` for free tier usage  
- Always keep key pair secure (do not share)  
- Security group should allow required ports only  
- Monitor instance usage to avoid extra cost  

---
