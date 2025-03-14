# Phishing Simulation Using Gophish on Kali Linux

## 📌 Project Overview
This project demonstrates how to use **Gophish**, an open-source phishing toolkit, to **simulate phishing attacks** for cybersecurity awareness training. The objective is to understand **social engineering tactics** and implement **phishing defenses**.

By setting up **Gophish** on **Kali Linux**, we can launch controlled phishing campaigns to train users and analyze security awareness.

---

## 🛠 Tools Used
To perform phishing simulations, the following tools are used:

- **Kali Linux** (for ethical hacking)
- **Gophish** (phishing simulation toolkit)
- **Email Server** (for sending phishing emails)
- **Web Server** (to host fake phishing pages)

---

## ⚡ Key Tasks
The following penetration testing activities are performed:

1. **🛠 Setting up Gophish to launch phishing campaigns**
2. **📧 Creating custom phishing email templates**
3. **🌐 Designing fake login pages for credential harvesting**
4. **📊 Analyzing attack results to measure user awareness**
5. **🛡️ Implementing defensive strategies against phishing**

---

## 🚀 How to Run

### ✅ Step 1: Download Gophish
First, download the latest release of **Gophish**:

\`\`\`bash
wget https://github.com/gophish/gophish/releases/download/vX.X.X/gophish-vX.X.X-linux-64bit.tar.gz
\`\`\`

Replace `vX.X.X` with the latest version number from the [Gophish Releases](https://github.com/gophish/gophish/releases).

---

### ✅ Step 2: Extract and Set Up Gophish
Extract the Gophish archive:

\`\`\`bash
tar -xvzf gophish-vX.X.X-linux-64bit.tar.gz
\`\`\`

Navigate into the Gophish directory:

\`\`\`bash
cd gophish
\`\`\`

---

### ✅ Step 3: Run Gophish
Give execution permission and start Gophish:

\`\`\`bash
chmod +x gophish
./gophish
\`\`\`

Once started, Gophish will provide login details:Please login with the following credentials: Username: admin Password: randomly_generated_password
## 🕵️ Phishing Campaign Setup

### 🔹 1. Configure SMTP Settings (Email Server)
To send phishing emails, configure an SMTP server in **Gophish Settings**.

Example SMTP setup for Gmail (Less Secure Apps Enabled):

\`\`\`bash
SMTP Server: smtp.gmail.com
Port: 587
Username: your-email@gmail.com
Password: your-app-password
\`\`\`

---

### 🔹 2. Create a Phishing Email Template
Design a **realistic phishing email** in the Gophish interface.

Example Phishing Email:

\`\`\`
Subject: Urgent Security Update Required!
Body:
Dear User,

Your account requires immediate verification due to unusual login attempts.
Please confirm your identity by clicking the link below:

[Verify Now](http://your-phishing-site.com)

Thank you,
Security Team
\`\`\`

---

### 🔹 3. Design a Fake Login Page
Use **Gophish Landing Pages** to create a phishing site.

To clone a real login page:

\`\`\`bash
wget -r -k -p http://example-login-page.com
\`\`\`

Edit the cloned page to redirect credentials to **Gophish**.

---

### 🔹 4. Launch the Phishing Campaign
1. **Create a new campaign** in Gophish.
2. Select the **Email Template** and **Landing Page**.
3. Add **Target Users** (training group).
4. Start the campaign.

---

### 🔹 5. Analyze Results
Monitor campaign statistics in **Gophish Dashboard**:

- 📧 **Emails Sent**
- 📬 **Emails Opened**
- 🔗 **Links Clicked**
- 🔐 **Credentials Entered**

---

## 🛡️ Defensive Strategies
To protect against phishing attacks, implement:

- **Multi-Factor Authentication (MFA)** to prevent credential misuse.
- **Email Filtering** to block suspicious emails.
- **Security Awareness Training** for employees.
- **Domain Monitoring** to detect fake login pages.
- **Phishing-resistant Browsers** (Google Safe Browsing, Microsoft Defender).

---

## 🎯 Conclusion
This project demonstrates **ethical phishing simulations** to improve cybersecurity awareness. By using **Gophish**, organizations can safely test employees' security awareness and strengthen phishing defenses.

**🔹 Disclaimer:** This guide is for educational purposes only. Do not attempt phishing attacks without proper authorization.
