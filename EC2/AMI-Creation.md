# 📀 AMI Creation (AWS Practical)

This document explains how to create an AMI (Amazon Machine Image) from an EC2 instance and launch a new instance from it.

---

# 🚀 Part 1: Create AMI from EC2 Instance

## 📌 Step 1: Connect to Instance
- Connect to EC2 instance using **SSH**  
- Install required packages/software  
![Step 1 Screenshot](step1.png)

---

## 📌 Step 2: Create Image
1. Select the instance  
2. Click **Actions → Image and templates → Create image**  
![Step 2 Screenshot](step2.png)

---

## 📌 Step 3: Configure AMI
- Give **Name tag**  
- Add description (optional)  

### Reboot Options:
- Checked → **No reboot** (faster, less consistent)  
- Unchecked → **Instance reboots** (recommended for consistency)  
![Step 3 Screenshot](step3.png)

---

## 📌 Step 4: Configure Storage
- Root volume is added by default  
- Add additional volumes if required  
![Step 4 Screenshot](step4.png)

---

## 📌 Step 5: Add Tags
- Add tags for both AMI and snapshot  

---

## 🚀 Step 6: Create Image
Click **Create Image**

---

## ✅ Output
AMI Image created successfully 🎉  
![Step 5 Screenshot](step5.png)

---

# 🚀 Part 2: Launch Instance from AMI

## 📌 Step 1: Select AMI
- Choose the created AMI to launch instance  
![Step 6 Screenshot](step6.png)

---

## 📌 Step 2: Configure Instance
- Give name tag  
- OS and instance type are pre-configured from AMI  
![Step 7 Screenshot](step7.png)

---

## 📌 Step 3: Key Pair
- Select or create key pair  
![Step 8 Screenshot](step8.png)

---

## 📌 Step 4: Security Group
- Select appropriate security group  
![Step 9 Screenshot](step9.png)

---

## 📌 Step 5: Storage
- Use default volume or add extra if required  

---

## 🚀 Step 6: Launch Instance
Click **Launch Instance**

---

## 🔐 Step 7: Connect to Instance
- Connect via SSH  

---

## 🔍 Step 8: Verify Packages
- Check installed packages/software  

---

## ✅ Output
Instance launched successfully with pre-installed packages 🎉  

---

# 🧠 Important Notes
- AMI stores OS + installed software + configuration  
- Use reboot option for consistency  
- AMI helps in fast deployment of identical instances  
- Useful for backup, scaling, and automation  

---
