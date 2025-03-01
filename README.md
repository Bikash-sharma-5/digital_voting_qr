# Voter QR Code Verification System  

A **secure web-based system** for generating, scanning, and managing voter information using **QR codes** with AES encryption. This system ensures **voting integrity** by preventing multiple votes from the same voter.

## 📌 Features  

✔️ **Generate QR Codes** for voter verification.  
✔️ **Encrypt voter details** (Voter ID & Name) using **AES encryption**.  
✔️ **Scan QR Codes** and verify voter details.  
✔️ **Track voting status** – prevents multiple votes.  
✔️ **Search voters** in a dynamically updated database.  

## 🛠️ Technologies Used  

- **HTML, CSS, JavaScript** (Frontend)  
- **CryptoJS** (AES encryption for voter data)  
- **QRCode.js** (QR code generation)  
- **html5-qrcode** (QR code scanning)  

## 🚀 How It Works  

1. **Add Voter to Database**  
   - Enter **Voter ID** and **Name**.  
   - Click **"Add to Database"** (Name is stored **encrypted**).  

2. **Generate QR Code**  
   - Select an existing **Voter ID** from the database.  
   - Click **"Generate QR Code"** – the QR contains **encrypted** voter details.  

3. **Scan QR Code**  
   - Click **"Start Scanner"** and scan the **QR code**.  
   - The system **decrypts** and verifies the voter.  
   - If the voter hasn't voted yet, they are **marked as voted** ✅.  
   - If already voted, an **alert prevents multiple votes** ❌.  

4. **View Voter Database**  
   - Check voter status (**✅ Voted / ❌ Not Voted**).  
   - Use the **search bar** to find voters.  

## 🏗️ Setup & Usage  

### 🔹 1. Clone Repository  
```sh
git clone https://github.com/yourusername/voter-qr-system.git
cd voter-qr-system
