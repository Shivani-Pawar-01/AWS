# IAM User Creation Guide (AWS)

## 📌 Overview
This guide explains the step-by-step process to create an IAM User in AWS and grant appropriate permissions.

---

## 🛠️ Steps to Create an IAM User

### 1. Go to IAM Dashboard
- Open AWS Management Console
- Navigate to **IAM (Identity and Access Management)**
- Click on **Users**
- Click **Create User**
<img width="940" height="189" alt="image" src="https://github.com/user-attachments/assets/0310efe2-28ed-4b7b-85b1-2c24c93b01d3" />


---

### 2. Specify User Details
- Enter a **User Name**
- (Optional) Add tags for identification
<img width="940" height="167" alt="image" src="https://github.com/user-attachments/assets/2d62a5d7-b0f3-4a53-87ea-420f9272884e" />


---

### 3. Enable Console Access
- Enable **AWS Management Console access**
- This allows the user to log in using a username and password
<img width="940" height="74" alt="image" src="https://github.com/user-attachments/assets/88ed483e-435f-40c1-a399-7d083e64648a" />


---

### 4. Set Password Options
Choose one of the following:
- **Auto-generated password**
- **Custom password**
<img width="940" height="319" alt="image" src="https://github.com/user-attachments/assets/76dc7959-137f-4b9f-ba5a-4f084535fa48" />


✔ Ensure secure login by enforcing password policies

---

### 5. Set Permissions
Choose how to assign permissions:

- Attach policies directly
- Add user to a group
- Copy permissions from an existing user
<img width="940" height="378" alt="image" src="https://github.com/user-attachments/assets/5529ff34-f216-4005-b509-d73834505eb5" />


✔ Customize permissions based on requirements (least privilege principle)

---

### 6. Review Configuration
- Carefully review all settings
- Ensure correct permissions and details are assigned
<img width="940" height="376" alt="image" src="https://github.com/user-attachments/assets/e910794a-66ef-42ab-a7e7-75e7ef08005c" />


---

### 7. Check Console Sign-In Details
- Review login URL and credentials
- Download or copy details for the user
<img width="940" height="373" alt="image" src="https://github.com/user-attachments/assets/3e430404-0568-45ad-b3ea-83bb921762e1" />


---

### 8. Create User
- Click **Create User**
- Click **Return to User List**
<img width="940" height="202" alt="image" src="https://github.com/user-attachments/assets/30698a05-648c-439f-aba1-d8a45d409a87" />


✔ IAM User is successfully created 🎉

---

## 🔐 Best Practices
- Follow **least privilege principle**
- Use **MFA (Multi-Factor Authentication)**
- Avoid using root account for daily tasks
- Regularly review permissions

---

## 📎 Summary
Creating an IAM user involves:
1. Defining user details
2. Setting login access
3. Assigning permissions
4. Reviewing and creating the user

---
