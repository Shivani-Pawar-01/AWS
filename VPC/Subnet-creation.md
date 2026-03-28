# 🌐 Subnet Creation (AWS Practical)

This document explains the step-by-step process of creating Public and Private Subnets in AWS.

---

##  Step 1: Click on "Create Subnet" (Public Subnet)
<img width="940" height="220" alt="image" src="https://github.com/user-attachments/assets/ddecf1e1-0ef0-4242-ab87-7bcc0ce76e17" />


---

##  Step 2: Select VPC
Choose the VPC in which you want to create the subnet  
<img width="940" height="232" alt="image" src="https://github.com/user-attachments/assets/b1f64052-2540-450e-93b6-d0b987209ef8" />


---

##  Step 3: Give Subnet Name Tag
Provide a meaningful name for the subnet  
<img width="940" height="109" alt="image" src="https://github.com/user-attachments/assets/4abb7d00-3468-43d0-aa87-ae13997d7ece" />


---

##  Step 4: Select Availability Zone (AZ)
Choose the desired Availability Zone  
<img width="940" height="179" alt="image" src="https://github.com/user-attachments/assets/2e77ed26-d1c1-482a-878e-019c1574f920" />


---

##  Step 5: Define CIDR Block
Provide the IP range for the subnet  
Example: `10.0.1.0/24`  
<img width="940" height="117" alt="image" src="https://github.com/user-attachments/assets/ba94bfab-20b6-4833-ad18-3aba8224c06d" />


---

## 🔁 Repeat Steps for Private Subnet
Follow the same steps to create a Private Subnet

---

## ✅ Step 6: Public and Private Subnets Created
<img width="940" height="197" alt="image" src="https://github.com/user-attachments/assets/49a8c6e3-884a-47e3-bb72-455e8eec2b4c" />


---

## 🌍 Step 7: Enable Auto-Assign Public IP (for Public Subnet)

To allow instances to interact with the internet:

### Steps:
1. Select the subnet  
2. Click on **Actions → Edit subnet settings**  
3. Enable **Auto-assign public IPv4 address** (checkbox) and save

<img width="940" height="303" alt="image" src="https://github.com/user-attachments/assets/2e637d52-fc57-4d70-bcbc-044d0cef3996" />
<img width="940" height="120" alt="image" src="https://github.com/user-attachments/assets/99b03698-c263-4e9f-a4f6-bd23a30c3d19" />



---

## 🧠 Notes
- Public subnet → used for internet-facing resources  
- Private subnet → used for secure internal resources  
- CIDR block must not overlap with other subnets
-  ✅ Enable **Auto-assign Public IP** for public subnet to allow internet interaction  


---
