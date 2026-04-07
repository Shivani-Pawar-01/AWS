# 🌐 Web Hosting using S3 + Route 53 (AWS Practical)

This document explains the step-by-step process to host a static website using Amazon S3 and Route 53.

---

# 🪣 Part 1: Create S3 Bucket

## 📌 Step 1: Create Bucket
Click on **Create Bucket**  
<img width="940" height="331" alt="image" src="https://github.com/user-attachments/assets/d0490612-bc5b-4a3d-97ad-15ab6e207a10" />


---

## 📌 Step 2: Select Bucket Type
- General purpose → Single region  
- Multi-AZ → For higher availability  
<img width="940" height="198" alt="image" src="https://github.com/user-attachments/assets/4efbdb75-9fa0-4e90-8092-04f4221b3143" />


---

## 📌 Step 3: Bucket Name & Namespace
- Bucket name must be **globally unique**
- give name same as a domain name
- Add name tag  
<img width="940" height="223" alt="image" src="https://github.com/user-attachments/assets/0a1a0c92-f319-4a2f-8ef8-5ac1e934b69b" />


---

## 📌 Step 4: Object Ownership
- Enable → For public web hosting  
- Disable → For private use  
<img width="940" height="181" alt="image" src="https://github.com/user-attachments/assets/65b0c0a8-32d1-4596-be15-7aa14d5b5adf" />


---

## 📌 Step 5: Public Access Settings
- Enable public access for hosting
<img width="940" height="328" alt="image" src="https://github.com/user-attachments/assets/de20b856-b628-4ec1-9b1f-70463b5d0fcd" />


---

## 📌 Step 6: Versioning
- Enable/Disable as required
<img width="940" height="125" alt="image" src="https://github.com/user-attachments/assets/325365ec-9646-4f19-b226-41e3b312a631" />


---

## 📌 Step 7: Default Encryption
- Data is encrypted using SSE-S3 or SSE-KMS  
<img width="940" height="213" alt="image" src="https://github.com/user-attachments/assets/bd216084-b778-46a7-9bf8-63caa0279fae" />


---

## 📌 Step 8: Create Bucket
Click **Create Bucket**  
<img width="940" height="399" alt="image" src="https://github.com/user-attachments/assets/c97f06e4-b246-4313-b7b4-c42ef9bd63c6" />


---

## ✅ Step 9: Bucket Created
<img width="940" height="357" alt="image" src="https://github.com/user-attachments/assets/2f004552-1c68-4619-899f-adfe1ad351aa" />


---

# 📂 Part 2: Upload Website Files

## 📌 Step 1: Open Bucket
Click on your bucket  
<img width="940" height="357" alt="image" src="https://github.com/user-attachments/assets/f7f07cfb-8ce1-44ff-a149-2c229e81d03c" />


---

## 📌 Step 2: Upload Files
Click **Upload**  
<img width="940" height="294" alt="image" src="https://github.com/user-attachments/assets/8c0a4c5f-6385-4927-8f26-2dbc77c54673" />


---

## 📌 Step 3: Add Files
- Click **Add files** OR drag & drop
<img width="940" height="268" alt="image" src="https://github.com/user-attachments/assets/155d3ae9-bb09-481d-8147-b79785c43c5b" />
- And you will something like this
<img width="940" height="268" alt="image" src="https://github.com/user-attachments/assets/155d3ae9-bb09-481d-8147-b79785c43c5b" />


---

## 📌 Step 4: Upload Files
Click **Upload**  
<img width="940" height="359" alt="image" src="https://github.com/user-attachments/assets/082a32cb-4d4b-49c9-8850-fd1f84228f83" />


---

## 🌐 Step 5: Enable Static Website Hosting

1. Go to **Properties**  
2. Scroll to **Static Website Hosting**  
3. Click **Edit**  
4. Enable it  

---

## 📌 Step 6: Add Index Document
- Enter: `index.html`  
<img width="940" height="199" alt="image" src="https://github.com/user-attachments/assets/ca755085-9a8d-4765-88d3-4fc734196da6" />


---

## 📌 Step 7: Save Changes

---

## 🌍 Step 8: Make Files Public
1. Select all files  
2. Click **Actions → Make public using ACL**  
<img width="940" height="348" alt="image" src="https://github.com/user-attachments/assets/4276d96c-a976-4a43-a591-bebe366f5ead" />
<img width="940" height="333" alt="image" src="https://github.com/user-attachments/assets/701b40ac-26f9-469d-bfaf-e19f54390149" />


---

# 🌐 Part 3: Create Hosted Zone in Route 53

## 📌 Step 1: Create Hosted Zone
Click **Create Hosted Zone**  
<img width="940" height="453" alt="image" src="https://github.com/user-attachments/assets/700f8152-2c7f-42b5-91df-d331325e8c0a" />


---

## 📌 Step 2: Enter Domain Name
Add domain name and optional description  
<img width="940" height="243" alt="image" src="https://github.com/user-attachments/assets/3189b9b8-f055-463b-af86-ab520ed6ad0d" />
<img width="940" height="285" alt="image" src="https://github.com/user-attachments/assets/37b247f4-d8c8-4621-a7be-1b22bb973029" />


---

## 📌 Step 3: Hosted Zone Created


---

## 📌 Step 4: Copy NS Records
<img width="940" height="472" alt="image" src="https://github.com/user-attachments/assets/7b22f68e-70d1-43b5-b937-e5eeec873057" />


---

## 📌 Step 5: Update Domain Provider
- Go to domain provider website  
- Update **NS (Name Server) records**
<img width="940" height="479" alt="image" src="https://github.com/user-attachments/assets/fd4458c5-b2ce-4a17-9ed6-c630626b938e" />


---

## 📌 Step 6: DNS Settings
- Open domain → DNS/Nameserver  
- Replace with Route 53 NS records
<img width="940" height="443" alt="image" src="https://github.com/user-attachments/assets/e79712a2-154e-4c3b-9577-76c293123b0c" />
<img width="940" height="472" alt="image" src="https://github.com/user-attachments/assets/989b4814-ae21-4b29-9bbf-2f2ef40e6231" />


---

## ⏳ Step 7: Wait for Propagation
- Can take few minutes to 24 hours  

---

# 🌐 Part 4: Create Record in Hosted Zone

## 📌 Step 1: Create Record
Go to Hosted Zone → Click **Create Record**
<img width="940" height="447" alt="image" src="https://github.com/user-attachments/assets/0279d502-dd80-45fe-9c58-ff2b875c4789" />


---

## 📌 Step 2: Configure Record
- Leave subdomain empty  
- Record type → A  
- Enable Alias  

---

## 📌 Step 3: Routing
- Select region same as S3 bucket  
- Select bucket endpoint  

---

## 📌 Step 4: Routing Policy
- Simple routing  
- Evaluate target health → Yes


---

## 📌 Step 5: Create Record
<img width="940" height="311" alt="image" src="https://github.com/user-attachments/assets/647a202e-39cd-4ffb-bebd-aff41d346689" />

---

# ✅ Part 5: Test Website

Open in browser: Type the domain name eg: www.shivanipawar.online
<img width="940" height="482" alt="image" src="https://github.com/user-attachments/assets/6abb8323-b2a4-4a9b-a368-64be8a9c9027" />

🎉 Website hosted successfully!

---

# 🧠 Important Notes
- Bucket name must match domain name for static hosting  
- Public access must be enabled for website hosting  
- Always set `index.html` as default document  
- DNS propagation may take time  
- Route 53 + S3 is cost-effective for static websites  

---
