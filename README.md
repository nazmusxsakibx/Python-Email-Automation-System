# Python-Email-Automation-System

Python Email Automation System

# 🐍 Python Email Automation System

> Automated email delivery using Python — featuring multi-receiver support, file attachments, and daily scheduling.

---

## ✨ Features

- 📨 Send emails to **multiple receivers** simultaneously
- 📎 Attach **any file type** (PDF, image, Excel, text)
- ⏰ **Daily scheduler** — auto-sends at a fixed time every day
- 🛡️ **SSL encrypted** Gmail SMTP connection
- ⚠️ **Error handling** — one failure never stops other receivers

---

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Python 3.11 | Core programming language |
| smtplib | SMTP email sending |
| email.mime.multipart | Multi-part email (body + attachment) |
| email.mime.base | File attachment handling |
| Base64 encoders | Binary to email-safe encoding |
| Gmail SMTP | smtp.gmail.com on Port 465 (SSL) |
| schedule | Daily task scheduling |
| os | File existence check |

---

## 🚀 Setup & Run

### 1. Install dependency
```bash
pip install schedule
```

### 2. Configure settings in send_email.py
```python
SENDER     = "your_email@gmail.com"
PASSWORD   = "your_app_password"      # Google App Password
RECEIVERS  = ["receiver1@gmail.com", "receiver2@gmail.com"]
ATTACHMENT = r"full\path\to\file.pdf"
SEND_TIME  = "09:00"                  # Daily send time
```

### 3. Run
```bash
python send_email.py
```

---

## 📸 Output

```
Scheduler started! Emails will send daily at 09:00
Sending emails...
Email sent to receiver1@gmail.com
Email sent to receiver2@gmail.com
```

---

## 🔐 Google Account Setup

1. Enable **2-Step Verification** at myaccount.google.com/security
2. Generate **App Password** at myaccount.google.com/apppasswords
3. Use the 16-digit App Password in the script — never your real password

---


## 📄 Documentation

Full project documentation included with:
- Full code 
- Explanation
- Output 
