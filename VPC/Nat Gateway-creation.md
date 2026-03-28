# 🌐 NAT Gateway Creation (AWS Practical)

This document explains the step-by-step process of creating and configuring a NAT Gateway in AWS.

---

## 📌 Step 1: Click on "Create NAT Gateway"
Go to **VPC Dashboard → NAT Gateways → Create NAT Gateway**  
<img width="940" height="214" alt="image" src="https://github.com/user-attachments/assets/139c18d1-1b6d-4cc1-a74d-ad4dcf6252e1" />


---

## 📌 Step 2: Give Name to NAT Gateway
Provide a meaningful name for the NAT Gateway  
<img width="940" height="87" alt="image" src="https://github.com/user-attachments/assets/b3eef20d-e78f-4bce-9014-2a06a4a43ffd" />


---

## 📌 Step 3: Choose Availability Mode
Select one of the following:
- Zonal (Recommended)
- Regional  
<img width="940" height="90" alt="image" src="https://github.com/user-attachments/assets/e56d87ce-80b9-4c9d-930f-d627b5462dd4" />


---

## 📌 Step 4: Select VPC
Choose the VPC where NAT Gateway will operate  
<img width="940" height="117" alt="image" src="https://github.com/user-attachments/assets/48358df8-3ef7-4ba6-b5e0-046da4f28f9d" />


---

## 📌 Step 5: Choose Connectivity Type
Select **Public NAT Gateway**  
- Used to provide outbound internet access for private subnets  
<img width="940" height="65" alt="image" src="https://github.com/user-attachments/assets/a3b68bdf-efed-4a45-8b2c-2c70f31b9ebc" />


---

## 📌 Step 6: Allocate Elastic IP
Select **Automatic allocation**  
- Provides a static public IP for outbound traffic
<img width="940" height="103" alt="image" src="https://github.com/user-attachments/assets/d7dfa7ca-d6f4-496a-ba90-a3e815f575a2" />


---

## ✅ Step 7: NAT Gateway Created
Wait until status shows **Available**  
<img width="940" height="215" alt="image" src="https://github.com/user-attachments/assets/fb7c6667-0799-402c-adbb-56ce659f1934" />


---

## 🔁 Step 8: Edit Route Table
Go to **Route Tables → Select Private Route Table → Edit Routes**  
<img width="940" height="212" alt="image" src="https://github.com/user-attachments/assets/55e8f146-fbe1-494c-86ab-875d3ffbc0b4" />


---

## 🔗 Step 9: Add Route
Add the following route:

- **Destination:** `0.0.0.0/0`  
- **Target:** NAT Gateway  

<img width="940" height="262" alt="image" src="https://github.com/user-attachments/assets/b253434d-69e8-4a3c-8b5c-1b4b9bd7403e" />


---

## 💾 Step 10: Save Changes
Click **Save Routes** to apply configuration  

---

## 🧠 Important Notes
- NAT Gateway allows **private subnet instances to access the internet**
- It supports **outbound traffic only**
- Requires:
  - Public Subnet
  - Elastic IP
  - Internet Gateway attached to VPC
- Must update **Private Route Table** to use NAT Gateway

---

## 🔁 Traffic Flow
- Private Subnet → Route Table → NAT Gateway → Internet Gateway → Internet

---  
