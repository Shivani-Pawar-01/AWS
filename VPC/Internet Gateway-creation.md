# 🌐 Internet Gateway Creation (AWS Practical)

This document explains the step-by-step process of creating and attaching an Internet Gateway in AWS.

---

##  Step 1: Click on "Create Internet Gateway"
<img width="940" height="219" alt="image" src="https://github.com/user-attachments/assets/a7dc9fe4-5adf-4e49-b19d-e0d55969fba0" />


---

##  Step 2: Give Name to Internet Gateway
Provide a name and click on **Create Internet Gateway**  
<img width="940" height="273" alt="image" src="https://github.com/user-attachments/assets/f63f4d13-4fb7-415a-8972-b1d9aa09f299" />


---

## ✅ Step 3: Internet Gateway Created
<img width="940" height="191" alt="image" src="https://github.com/user-attachments/assets/e4757c12-b448-4509-8b78-06dae08509b5" />


---

## 🔗 Step 4: Attach Internet Gateway to VPC
Click on **Actions → Attach to VPC**  
<img width="940" height="197" alt="image" src="https://github.com/user-attachments/assets/9b56f8cd-194c-473c-b125-8d54d83f72c2" />


---

## 🌍 Step 5: Select VPC
Choose the VPC to provide internet access and click **Attach Internet Gateway**  
<img width="940" height="211" alt="image" src="https://github.com/user-attachments/assets/b8da7231-1d7b-4613-a75e-c0c893466270" />


---

## 🔁 Step 6: Update Route Table
Go to Route Table → Click **Actions → Edit Routes**  
<img width="940" height="263" alt="image" src="https://github.com/user-attachments/assets/253a49f5-da4b-4c57-8a34-3d4a2ef67690" />


---

## 📡 Step 7: Add Route (Destination & Target)
Specify:
- **Destination** → `0.0.0.0/0` (for internet access)  
- **Target** → Internet Gateway  

Click **Save changes**  
<img width="940" height="238" alt="image" src="https://github.com/user-attachments/assets/472157a7-4a4c-4acc-ad20-566093558efb" />


---

## 🧠 Important Notes
- Internet Gateway enables communication between VPC and the internet  
- Must be attached to a VPC before use  
- Route table must have route (`0.0.0.0/0`) pointing to IGW for public access  
- Only public subnets should use Internet Gateway  

---
