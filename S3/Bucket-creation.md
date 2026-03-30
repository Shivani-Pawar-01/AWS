# S3 Bucket Creation Guide (AWS)

## 📌 Overview
This guide explains how to create an Amazon S3 bucket and configure its settings for storage, access, and security.

---

## 🛠️ Steps to Create an S3 Bucket

### 1. Create Bucket
- Open **AWS Management Console**
- Navigate to **S3 (Simple Storage Service)**
- Click **Create Bucket**
<img width="940" height="331" alt="image" src="https://github.com/user-attachments/assets/ddf8dc6b-9e4e-48ce-974e-ef4b796f7b59" />

---

### 2. Select Bucket Type
Choose the appropriate bucket type:

- **General Purpose Bucket**
  - Used for most workloads
  - Stores data across multiple Availability Zones (Multi-AZ)

- **Directory Bucket**
  - Used for specific use cases
  - Stores data in a single Availability Zone (Single-AZ)
  <img width="940" height="198" alt="image" src="https://github.com/user-attachments/assets/d01516a3-59ea-4acd-8f9e-5b6b3b966aad" />


---

### 3. Bucket Naming & Namespace
- Enter a **Bucket Name**
✔ Important:
- Bucket name must be **globally unique**
- Naming is not limited to a single account or region
<img width="940" height="135" alt="image" src="https://github.com/user-attachments/assets/9727a943-702e-446c-90a3-ff0086b762ed" />


---

### 4. Object Ownership
- Configure object ownership settings
Options:
- **ACLs Enabled**
- **ACLs Disabled (Recommended)**
<img width="940" height="181" alt="image" src="https://github.com/user-attachments/assets/905da316-4f26-4d0a-8840-859847755031" />


✔ Use:
- Enable (ACLs) → For special use cases like public hosting
- Disable → For private and secure access (recommended)

---

### 5. Public Access Settings
- Configure **Block Public Access**

Options:
- **Enable Block Public Access** → For private buckets (recommended)
- **Disable Block Public Access** → Required for public websites
<img width="940" height="328" alt="image" src="https://github.com/user-attachments/assets/4a96e8a2-6536-49b4-a923-009a83a358f0" />


---

### 6. Bucket Versioning
- Enable or disable **Versioning**

✔ Benefits:
- Keeps multiple versions of objects
- Helps in data recovery and protection
<img width="940" height="125" alt="image" src="https://github.com/user-attachments/assets/57ef0bb3-9336-4b1c-ba0a-b969150a15d1" />


---

### 7. Default Encryption
- Enable default encryption for bucket

Options:
- **SSE-S3** (Amazon managed keys)
- **SSE-KMS** (KMS managed keys)
<img width="940" height="213" alt="image" src="https://github.com/user-attachments/assets/5eff4646-74e5-49f0-9eb8-cd2643ddde5b" />


✔ Ensures all data is encrypted automatically

---

### 8. Create Bucket
- Click **Create Bucket**
<img width="940" height="399" alt="image" src="https://github.com/user-attachments/assets/9195bde3-55c8-4e4b-b908-14808c14bc90" />


---

### 9. Bucket Created
✔ Your S3 bucket is successfully created 🎉
<img width="940" height="344" alt="image" src="https://github.com/user-attachments/assets/b6b7ba04-1b2f-4299-bae5-1376e7f88db2" />


---

## 🔐 Best Practices
- Keep buckets **private by default**
- Enable **versioning** for critical data
- Use **encryption (SSE-S3 or SSE-KMS)**
- Follow **proper naming conventions**
- Avoid enabling public access unless required

---

## 📎 Summary
Creating an S3 bucket involves:
1. Choosing bucket type
2. Naming the bucket
3. Configuring access settings
4. Enabling security features
5. Creating the bucket

---
