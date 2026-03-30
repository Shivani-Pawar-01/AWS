# Attaching Policy to User / Role / User Group (AWS)

## 📌 Overview
This guide explains how to attach an IAM Policy to a User, Role, or User Group in AWS to grant permissions.

---

## 🛠️ Steps to Attach a Policy

### 1. Go to Policies Section
- Open **AWS Management Console**
- Navigate to **IAM (Identity and Access Management)**
- Click on **Policies**

---

### 2. Select Policy
- Choose the policy you want to attach
<img width="940" height="426" alt="image" src="https://github.com/user-attachments/assets/6d220cf4-b720-44d7-92de-83ef7d5b2cba" />


---

### 3. Open Attach Option
- Click on **Actions**
- Select **Attach**
<img width="940" height="445" alt="image" src="https://github.com/user-attachments/assets/90c4660b-5c66-4ec7-97e6-03d22869404d" />


---

### 4. Select Target Entity
- Choose where you want to attach the policy:
  - **User**
  - **Role**
  - **User Group**
  <img width="940" height="444" alt="image" src="https://github.com/user-attachments/assets/798bbd1b-f98f-46ea-a944-a0ec70a52b57" />


✔ Select the appropriate entity based on your requirement

---

### 5. Attach Policy
- Click **Attach Policy**
<img width="940" height="449" alt="image" src="https://github.com/user-attachments/assets/62b9c59f-a361-4996-8394-e589d7d3f801" />


✔ Policy is successfully attached 🎉

---

## 🔐 Best Practices
- Prefer attaching policies to **groups** instead of individual users
- Use **roles for services** (e.g., EC2, Lambda)
- Follow the **least privilege principle**
- Regularly review attached policies

---

## 📎 Summary
Attaching a policy involves:
1. Selecting the policy
2. Choosing the target (User / Role / Group)
3. Attaching the policy

---
