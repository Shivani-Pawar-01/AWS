# 🌐 Route Table Creation (AWS Practical)

This document explains the step-by-step process of creating and associating Route Tables in AWS.

---

##  Step 1: Click on "Create Route Table"
<img width="940" height="206" alt="image" src="https://github.com/user-attachments/assets/988cfc9a-5687-4337-9d6d-2a49f7885f34" />


---

##  Step 2: Give Name to Route Table
Provide a meaningful name for the route table  
<img width="940" height="147" alt="image" src="https://github.com/user-attachments/assets/34a1b4c3-f477-45dc-824e-7b64e7760719" />


---

##  Step 3: Select VPC
Choose the VPC to control traffic for that specific VPC only  
<img width="940" height="121" alt="image" src="https://github.com/user-attachments/assets/12f33cd6-ada7-4316-b114-c7271ac618b9" />


---

## ✅ Step 4: Route Table Created
<img width="940" height="196" alt="image" src="https://github.com/user-attachments/assets/718fed47-e528-4e40-abaa-fcd6eec8385b" />


---

## 🔁 Repeat for Private Route Table
Follow the same steps to create a Private Route Table

---

## 🔗 Step 5: Edit Subnet Association
This decides which route table a subnet will follow  
<img width="940" height="275" alt="image" src="https://github.com/user-attachments/assets/1a7759a8-34ed-47ca-a8ba-f3445188fe1f" />


---

## 🌍 Step 6: Associate Public Subnet
Select the public subnet and click **Save associations**  
<img width="940" height="261" alt="image" src="https://github.com/user-attachments/assets/b90950b1-e2cf-4796-bb6f-b8f393904278" />


---

## 🔒 Step 7: Associate Private Subnet
Select the private subnet and click **Save associations**  
<img width="940" height="268" alt="image" src="https://github.com/user-attachments/assets/b1150c26-3cdb-4920-aea7-95a45bf64f41" />


---

## 🧠 Important Notes
- Route Table controls traffic routing within a VPC  
- Each subnet must be associated with a route table  
- Public subnet → associated with route table having Internet Gateway route  
- Private subnet → associated with route table without Internet access  

---
