# IAM Role Creation Guide (AWS)

## 📌 Overview
This guide explains how to create an IAM Role in AWS and assign permissions for services or entities to securely access AWS resources.

---

## 🛠️ Steps to Create an IAM Role

### 1. Go to IAM Dashboard
- Open **AWS Management Console**
- Navigate to **IAM (Identity and Access Management)**
- Click on **Roles**
- Click **Create Role**
<img width="940" height="231" alt="image" src="https://github.com/user-attachments/assets/3a1c6d98-6ec2-4321-8e94-253b3a6ce8f3" />


---

### 2. Select Trusted Entity Type
- Choose **who will use this role**
<img width="940" height="267" alt="image" src="https://github.com/user-attachments/assets/521f4aa0-ed05-40c5-b80a-b2fed675970f" />


Examples:
- AWS Service (e.g., EC2, Lambda)
- Another AWS Account
- Web Identity (e.g., Google, Facebook)

✔ This defines *which entity can use the role*

---

### 3. Select Use Case
- Choose the specific service (e.g., **EC2**)
<img width="940" height="425" alt="image" src="https://github.com/user-attachments/assets/87eec50e-faf6-4110-bafa-747d390e287e" />


✔ This helps AWS suggest relevant policies  
✔ It does **NOT** restrict you to only those permissions

---

### 4. Assign Permissions
- Attach policies to the role
<img width="940" height="384" alt="image" src="https://github.com/user-attachments/assets/15e24cff-a5ba-4667-8ca2-7478dba573b5" />


✔ Important:
- Even if use case is **EC2**, you can assign:
  - S3 permissions
  - DynamoDB permissions
  - Any required permissions

---

### 5. Name and Describe Role
- Enter a **Role Name**
- Add a **Description** for clarity
- (Optional) Add tags
<img width="940" height="267" alt="image" src="https://github.com/user-attachments/assets/9b588048-2d13-45d5-8c8a-6f5a66aa7f0f" />


---

### 6. Review Configuration
- Check:
  - Trusted entity
  - Permissions attached
  - Role details
  <img width="940" height="379" alt="image" src="https://github.com/user-attachments/assets/f26355bb-9211-4631-b0c9-b2139c0fa42c" />

✔ Ensure everything is correct to avoid misconfiguration


---

### 7. Create Role
- Click **Create Role**
<img width="940" height="310" alt="image" src="https://github.com/user-attachments/assets/4cb9a587-8647-45bc-bab8-16955d2932fb" />

✔ IAM Role is successfully created 🎉

---

## 🔐 Best Practices
- Follow **least privilege principle**
- Use roles instead of storing credentials in applications
- Assign roles to services like **EC2, Lambda**
- Regularly review and update permissions

---

## 📎 Summary
Creating an IAM Role involves:
1. Selecting trusted entity
2. Choosing use case
3. Assigning permissions
4. Reviewing and creating the role

---
