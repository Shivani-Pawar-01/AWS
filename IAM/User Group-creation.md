# IAM User Group Creation Guide (AWS)

## 📌 Overview
This guide explains how to create an IAM User Group in AWS and assign users and permissions.

---

## 🛠️ Steps to Create a User Group

### 1. Create User Group
- Go to **IAM Dashboard**
- Click on **User Groups**
- Click **Create Group**
<img width="940" height="241" alt="image" src="https://github.com/user-attachments/assets/13474f6b-5179-4a28-8338-23368d991284" />


---

### 2. Specify Group Name
- Enter a **User Group Name**
- (Optional) Add tags for better identification
<img width="940" height="215" alt="image" src="https://github.com/user-attachments/assets/eee4cdb1-28c5-4cee-b4d5-b6343fe29bab" />


---

### 3. Add Users to Group
- Select users you want to add to this group
- Users in this group will inherit the assigned permissions
<img width="940" height="178" alt="image" src="https://github.com/user-attachments/assets/0f78e600-26fe-4adc-9381-7be20a49885b" />


---

### 4. Assign Permissions
- Attach required policies to the group

Example permissions:
- **EC2 Full Access**
- **VPC Full Access**
- **S3 Full Access**
<img width="940" height="464" alt="image" src="https://github.com/user-attachments/assets/7c446ad9-207c-4b1d-a724-b88b8e177fd8" />


✔ Choose permissions based on requirements

---

### 5. Create User Group
- Click **Create Group**
<img width="940" height="253" alt="image" src="https://github.com/user-attachments/assets/b1f8f05f-69db-4da7-af8f-b6767a1cdfc7" />


✔ IAM User Group is successfully created 🎉

---

## 🔐 Best Practices
- Use **groups to manage permissions** instead of assigning directly to users
- Follow the **least privilege principle**
- Create different groups for different roles (e.g., Admin, Developer, Read-only)
- Regularly review group permissions

---

## 📎 Summary
Creating a User Group involves:
1. Naming the group
2. Adding users
3. Assigning permissions
4. Creating the group

---
