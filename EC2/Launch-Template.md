# 📦 Launch Template (AWS Practical)

This document explains how to create a Launch Template and launch EC2 instances using it.

---

# 🚀 Part 1: Create Launch Template

## 📌 Step 1: Click on "Create Launch Template"
Go to EC2 Dashboard → Click **Launch Templates → Create launch template**  
![Step 1 Screenshot](step1.png)

---

## 📌 Step 2: Give Template Name
Provide a name tag for the launch template  
![Step 2 Screenshot](step2.png)

---

## 📌 Step 3: Specify Template Version
- Define version (useful for future updates)  
![Step 3 Screenshot](step3.png)

---

## 📌 Step 4: Auto Scaling Option
- Enable if you want to use with Auto Scaling  
![Step 4 Screenshot](step4.png)

---

## 📌 Step 5: Select AMI
Choose OS for instance environment  
![Step 5 Screenshot](step5.png)

---

## 📌 Step 6: Select Instance Type
Choose required instance type  
![Step 6 Screenshot](step6.png)

---

## 📌 Step 7: Configure Key Pair
Select or create key pair for authentication  
![Step 7 Screenshot](step7.png)

---

## 📌 Step 8: Network Settings
- Configure VPC, Subnet, and Security Group  
- Or leave default settings  
![Step 8 Screenshot](step8.png)

---

## ✅ Step 9: Launch Template Created
![Step 9 Screenshot](step9.png)

---

# 🚀 Part 2: Launch Instance from Launch Template

## 📌 Step 1: Select Template
- Choose the template  
- Click **Actions → Launch instance from template**  
![Step Screenshot](step10.png)

---

## 📌 Step 2: Select Version
- Choose template version  

---

## 📌 Step 3: Review Configuration
- Verify all settings  

---

## 🚀 Step 4: Launch Instance
Click **Launch Instance**

---

## ✅ Output
Instance launched successfully using Launch Template 🎉  

---

# 🔁 Alternative Method

## 📌 Create Template from Existing Instance
1. Select an existing EC2 instance  
2. Click **Actions → Image and templates → Create template from instance**  
3. Provide:
   - Name tag  
   - Version (optional)  
4. Template will inherit all instance configurations  

---

# 🧠 Important Notes
- Launch Templates help in reusing configurations  
- Useful for Auto Scaling and consistent deployments  
- Versioning allows easy updates  
- Reduces manual configuration errors  

---
