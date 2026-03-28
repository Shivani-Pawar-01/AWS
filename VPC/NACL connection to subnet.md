# 🔐 NACL Connection to Subnet (AWS Practical)

This document explains the step-by-step process of creating a Network ACL (NACL) and associating it with subnets in AWS.

---

##  Step 1: Create NACL
Go to **VPC Dashboard → Network ACLs → Create Network ACL**  
<img width="940" height="214" alt="image" src="https://github.com/user-attachments/assets/311c8779-77fe-4440-98f6-a28d5c10ddc8" />


---

##  Step 2: Give Name to NACL
Provide a meaningful name for the NACL  
<img width="940" height="123" alt="image" src="https://github.com/user-attachments/assets/95c0c8ee-cd9a-4b9d-af60-0e556853ec7b" />


---
## 📌 Step 3: Select VPC
Select the VPC where the NACL will be created  
- Every Network ACL must belong to a specific VPC
<img width="940" height="236" alt="image" src="https://github.com/user-attachments/assets/a7ba117d-1dc5-4d6a-a6c9-eab7a3e84caa" />


---

## ✅ Step 4: NACL Created
The Network ACL is successfully created  
<img width="940" height="220" alt="image" src="https://github.com/user-attachments/assets/e0c24044-d3d0-4586-9551-73ab23bb69e7" />


---

## 🔗 Step 5: Edit Subnet Association
- Select the NACL
- Click on **Actions → Edit Subnet Associations**  
<img width="940" height="216" alt="image" src="https://github.com/user-attachments/assets/aa393894-b8aa-415d-9699-4200dd4df1c2" />


---

## 🌐 Step 6: Associate Subnets
- Select **Public Subnet**
- Select **Private Subnet**
- Click **Save changes**

👉 Now the NACL is attached to both subnets  
<img width="940" height="264" alt="image" src="https://github.com/user-attachments/assets/d0d79725-7cca-4489-bb3b-9e3ca04b2f93" />


---

## 📥 Step 7: Configure Inbound Rules
- Click on **Edit Inbound Rules**
- Add rules to allow incoming traffic  
<img width="940" height="238" alt="image" src="https://github.com/user-attachments/assets/518d6099-b016-4a5a-a925-1533b76d7127" />


---

## 📤 Step 8: Configure Outbound Rules
- Click on **Edit Outbound Rules**
- Add rules to allow outgoing traffic  
<img width="940" height="221" alt="image" src="https://github.com/user-attachments/assets/043cf2c7-6012-42a9-910a-be6438f346b2" />


---

## 💾 Step 9: Save Rules
- Save both inbound and outbound rules  
<img width="940" height="237" alt="image" src="https://github.com/user-attachments/assets/6518b2d1-7034-4de4-8dbe-333256f45ec5" />


---

## 🧠 Important Notes
- NACL operates at the **subnet level**
- It is **stateless** (inbound and outbound rules are separate)
- One NACL can be associated with multiple subnets
- Default NACL allows all traffic, custom NACL must be configured manually

---
