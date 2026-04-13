# 🌐 CloudFront CDN Practical (AWS)

This document explains how to host a website using Amazon S3 and deliver it via CloudFront CDN, including custom domain setup with Route 53.

---

# 🚀 Part 1: Web Hosting using S3

## 📌 Step 1: Create S3 Bucket
1. Click on **Create Bucket**  
2. Select bucket type:
   - General → Multi-AZ storage  
   - Directory → Single AZ storage  
3. Select namespace and give bucket name:
   - Global → Unique globally  
   - Account regional → Region-based  
4. Object ownership:
   - Enable → Public hosting  
   - Disable → Private  
5. Public access:
   - Enable for web hosting  
6. Enable/Disable versioning  
7. Default encryption (SSE-S3 / SSE-KMS)  
8. Click **Create Bucket**  

✅ Bucket created successfully

---

## 📂 Step 2: Upload Website Files
1. Open bucket  
2. Click **Upload**  
3. Click **Add files** or drag & drop  
4. Upload HTML, CSS, JS files  
5. Click **Upload**  

---

## 🌐 Step 3: Enable Static Website Hosting
1. Go to **Properties**  
2. Scroll to **Static Website Hosting**  
3. Click **Edit**  
4. Enable it  
5. Enter:
   - Index document → `index.html`  
6. Click **Save changes**  

---

## 🔐 Step 4: Add Bucket Policy
1. Go to **Permissions**  
2. Scroll to **Bucket Policy**  
3. Add policy to allow public access  

---

## 🌍 Step 5: Make Files Public
1. Select all files  
2. Click **Actions**  
3. Click **Make public using ACL**  
4. Confirm  

---

# 🌍 Part 2: Create CloudFront Distribution

## 📌 Step 1: Create Distribution
1. Go to CDN dashboard  
2. Click **Create Distribution**  
3. Give name (optional)  
4. Distribution type → as required  
5. Domain name → auto-generated  

---

## 🔗 Step 2: Origin Settings
6. Origin type → S3  
7. Select your S3 bucket  

---

## ⚙️ Step 3: Settings
8. Private access:
   - Enable → if S3 is private  
   - Disable → if S3 is public  
9. Cost settings:
   - Enable → production  
   - Disable → practice  

---

## ✅ Step 4: Create Distribution
10. Review settings  
11. Click **Create Distribution**  

---

## ⏳ Step 5: Deployment
- Status → Deploying  
- Wait until deployed  

---

## 🏠 Step 6: Configure Default Root Object
1. Go to distribution → **General settings**  
2. Click **Edit**  
3. Add:
   - `index.html`  
4. Save changes  

---

## 🌐 Step 7: Access Website
1. Copy CDN domain name  
2. Paste in browser  

🎉 Website is now served via CDN

---

# 🌐 Part 3: CDN with Custom Domain

## 📌 Step 1: Create Distribution
1. Go to CDN dashboard  
2. Click **Create Distribution**  
3. Enter custom domain name  

---

## 🔗 Step 2: Origin Setup
4. Origin type → S3  
5. Select bucket  

---

## ⚙️ Step 3: Settings
6. Configure private access  
7. Configure cost settings  

---

## 🔒 Step 4: TLS Certificate
8. Create TLS certificate (HTTPS)  
   - Enables secure communication  

---

## ✅ Step 5: Create Distribution
9. Review settings  
10. Click **Create Distribution**  
11. Wait for deployment  

---

## 🏠 Step 6: Default Root Object
1. Go to settings  
2. Add `index.html`  
3. Save  

---

# 🌐 Part 4: Route 53 Setup

## 📌 Step 1: Create Hosted Zone
1. Go to Route 53  
2. Click **Create Hosted Zone**  
3. Enter domain name  
4. Create  

---

## 📌 Step 2: Update Name Servers
1. Copy NS records  
2. Go to domain provider  
3. Replace existing NS records  

⏳ Propagation time: up to 24 hours  

---

## 📌 Step 3: Create DNS Record
1. Go to hosted zone  
2. Click **Create Record**  
3. Leave subdomain empty  
4. Record type → A  
5. Enable alias  
6. Select CloudFront distribution  
7. Routing policy → Simple  
8. Evaluate target health → Yes  
9. Create record  

---

## 📌 Step 4: Verify
- Check CDN URL  
- Check custom domain  
- Verify HTTPS  

---

# 🎉 Final Output

- Website hosted on S3  
- Delivered via CloudFront CDN  
- Custom domain connected (optional)  
- HTTPS enabled (secure access)  

---

# 🧠 Important Notes
- CloudFront improves performance using caching  
- Always set `index.html` as default root object  
- Use HTTPS for secure communication  
- Route 53 connects domain with CDN  
- S3 can be private when using CloudFront  

---
