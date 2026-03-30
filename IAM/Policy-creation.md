# IAM Policy Creation Guide (AWS)

## 📌 Overview
This guide explains how to create an IAM Policy in AWS to define permissions for users, groups, or roles.

---

## 🛠️ Steps to Create an IAM Policy

### 1. Go to IAM Dashboard
- Open **AWS Management Console**
- Navigate to **IAM (Identity and Access Management)**
- Click on **Policies**
- Click **Create Policy**
<img width="940" height="298" alt="image" src="https://github.com/user-attachments/assets/ee5a1b41-0fd3-47e0-93e5-09f30bb0fc1e" />


---

### 2. Select Service
- Choose the **AWS service** for which you want to create the policy
<img width="940" height="429" alt="image" src="https://github.com/user-attachments/assets/29bf66e3-e7d3-4b3c-a357-06b43d23ed6f" />

Examples:
- S3
- EC2
- VPC

---

### 3. Define Actions
- Specify the actions you want to allow
Example:
- Enable **All Actions** (Full Access)
<img width="940" height="466" alt="image" src="https://github.com/user-attachments/assets/d31f6011-4194-4e48-990d-24a84d2237d9" />

  
✔ Actions define **what operations you can perform**

---

### 4. Specify Resources
- Select **All Resources** or define specific resources
✔ Important:
- **Action → What you can do**
- **Resource → Where you can do it**
<img width="940" height="376" alt="image" src="https://github.com/user-attachments/assets/3773ac9b-d324-4d4a-aa28-b35a158515d0" />


---

### 5. Name and Describe Policy
- Enter a **Policy Name**
- Add a **Description**
- (Optional) Add tags
<img width="940" height="296" alt="image" src="https://github.com/user-attachments/assets/a3fcde67-6b35-46d4-8a17-b29eeec23065" />


---

### 6. Review Policy
- Check all configurations:
  - Service
  - Actions
  - Resources
<img width="940" height="376" alt="image" src="https://github.com/user-attachments/assets/ded6e139-2da2-454e-b352-8447d7668767" />

✔ Ensure permissions are correct before creating

---

### 7. Create Policy
- Click **Create Policy**
<img width="940" height="380" alt="image" src="https://github.com/user-attachments/assets/22a2a37a-55ca-4cd4-b934-8b87d18f30a3" />


✔ IAM Policy is successfully created 🎉

---

## 🔐 Best Practices
- Follow **least privilege principle**
- Avoid giving full access unless required
- Use **specific resource-level permissions**
- Regularly review and update policies

---

## 📎 Summary
Creating an IAM Policy involves:
1. Selecting service
2. Defining actions
3. Specifying resources
4. Reviewing and creating the policy

---
