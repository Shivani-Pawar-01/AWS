# Static Website Hosting using S3 (AWS)

## 📌 Overview
This guide explains how to host a static website using an Amazon S3 bucket by uploading files and enabling static website hosting.

---

## 🛠️ Steps to Host a Static Website in S3

### 1. Open S3 Bucket
- Go to **AWS Management Console**
- Navigate to **S3**
- Select your **Bucket**
<img width="940" height="222" alt="image" src="https://github.com/user-attachments/assets/79773e3f-12ab-4a79-9e63-d50e264f0366" />


---

### 2. Upload Website Files
- Click on **Upload**
- Click **Add Files**
- Select files (HTML, CSS, JS, images)  
  OR use **Drag & Drop**
<img width="940" height="294" alt="image" src="https://github.com/user-attachments/assets/ec6bf542-21c5-4ca1-a646-e4b59c8ae6a7" />
<img width="940" height="268" alt="image" src="https://github.com/user-attachments/assets/770caebf-f255-4646-a14e-b4abff9a5d85" />


---

### 3. Upload Objects
- Review selected files
- Click **Upload**
<img width="940" height="303" alt="image" src="https://github.com/user-attachments/assets/ebb88050-046f-43d2-9c03-a063c63c2bee" />
<img width="940" height="359" alt="image" src="https://github.com/user-attachments/assets/3900dfbd-5892-46dd-9d57-01dbc37a93d3" />


✔ Files are now stored in the S3 bucket

---

### 4. Enable Static Website Hosting
- Go to **Properties** tab of the bucket
- Scroll to **Static Website Hosting**
- Click **Edit**
- Select **Enable**
<img width="940" height="334" alt="image" src="https://github.com/user-attachments/assets/17db6793-005f-41a6-b48f-7de084724f5d" />
<img width="940" height="324" alt="image" src="https://github.com/user-attachments/assets/ae75486d-7671-4d9e-8978-f9b4f3555850" />
<img width="940" height="180" alt="image" src="https://github.com/user-attachments/assets/247e9c70-846d-4d5b-bc64-5aeb05299911" />

---

### 5. Configure Hosting Settings
- Enter:
  - **Index Document** → `index.html`
  <img width="940" height="199" alt="image" src="https://github.com/user-attachments/assets/5b58b8f1-4be6-4c15-a23b-a5b653931a02" />


✔ This tells S3 which file to load as the homepage

- Save changes

---

### 6. Make Files Public
- Select all uploaded files
- Click **Actions**
- Choose **Make Public (using ACL)**
<img width="940" height="348" alt="image" src="https://github.com/user-attachments/assets/f00440b1-a55c-4995-b1ab-4cdb2fceb2c0" />
<img width="940" height="333" alt="image" src="https://github.com/user-attachments/assets/63db2a8c-55f2-480d-a4dc-1d5ba6c97474" />


✔ Required so users can access the website

---

### 7. Access Website Endpoint
- Go to **Properties**
- Scroll to **Static Website Hosting**
- Copy the **Bucket Website Endpoint**
<img width="940" height="408" alt="image" src="https://github.com/user-attachments/assets/0a8321ed-e83f-452f-94a2-ed65a6131751" />
<img width="940" height="203" alt="image" src="https://github.com/user-attachments/assets/0fe53355-cf76-4677-8f1f-8cbec790ef3d" />


---

### 8. Open Website
- Paste the endpoint URL in your browser
<img width="940" height="504" alt="image" src="https://github.com/user-attachments/assets/a2053485-9fcc-4806-9a74-fff6c388bcd8" />


✔ Your static website is now live 🎉

---

## Important Note
- Refer this for free template for web hosting


## 🔐 Best Practices
- Avoid using ACLs; prefer **Bucket Policies** for public access
- Enable **Block Public Access** only when needed
- Use **CloudFront + HTTPS** for production websites
- Organize files properly (index.html, assets folder, etc.)

---

## 📎 Summary
Hosting a static website involves:
1. Uploading files
2. Enabling static hosting
3. Making files public
4. Accessing via endpoint URL

---
