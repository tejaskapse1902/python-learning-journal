# 📧 SMTP - Email Sending Protocol in Python

### 🔹 What is SMTP?
SMTP stands for *Simple Mail Transfer Protocol*. It is a protocol used for sending emails from a client to a server and between mail servers.

### 🔹 Ports
- Port 587: TLS encryption (recommended)
- Port 465: SSL encryption

### 🔹 Python SMTP Flow
1. Connect to SMTP Server (e.g., smtp.gmail.com)
2. Login using app-password
3. Construct message (MIME format)
4. Send using `sendmail()` or `send_message()`
5. Close the connection

### 🔹 Real Use Cases
- OTP verification systems
- Automatic reminders & notifications
- Newsletter / bulk mailing
- Contact forms
- Password reset

### ✨ Next Goal:
Build **Account Verification Using OTP**
with Python + SMTP + Streamlit.
