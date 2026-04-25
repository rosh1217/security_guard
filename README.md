# security_guard
🛡️ SecureGuard – Security dashboard + encrypted vault with OpenCV face unlock. Password health, breach monitor, phishing detector, 2FA, security score.
# 🔐 SecureGuard – Core Security & Protection Platform

**Your personal cybersecurity command center.**  
SecureGuard is a full‑stack web application that helps individuals and small teams assess, monitor, and improve their digital security posture – all from one clean dashboard.

## ✨ Features

- **🔑 Password Health Checker** – Analyze password strength, detect reuse, and generate strong alternatives.
- **📡 Breach Monitor** – Check if your email appears in known data breaches (HaveIBeenPwned API).
- **🔗 Phishing URL Detector** – Scan suspicious links for malicious patterns and blacklists.
- **📝 Encrypted Secure Vault** – Store sensitive notes with client‑side AES‑256 encryption (zero‑knowledge).
- **🔢 TOTP 2FA Manager** – Generate time‑based one‑time passwords for your online accounts.
- - **📊 Security Score** – Dynamic score (0–100) that rewards secure behaviour.
- **👤 OpenCV Face Unlock** – *(Advanced)* Secure your vault with face recognition + liveness detection (blink & motion). Built with OpenCV and a Python microservice.

## 🧠 How It Works

- **Frontend:** React (Vite) + Tailwind CSS – responsive, dark/light mode, real‑time feedback.
- **Backend:** Node.js + Express (JWT auth, rate limiting, Helmet).
- **Database:** MongoDB (encrypted user data, breach cache).
- **Face Recognition:** Python/Flask microservice using `face_recognition` (dlib + OpenCV).  
  *Face embeddings are encrypted and never stored as raw images.*
- **APIs:** HaveIBeenPwned, VirusTotal (mock or real), plus heuristic checks.
- **Alerts you to leaked credentials** – change passwords before criminals use them.
- **Blocks phishing attempts** – stop fake login pages.
- **Protects secrets with zero‑knowledge encryption** – even the server admin cannot read your vault.
- **Adds a biometric factor** – face unlock prevents unauthorized physical access to the vault.

## 🧪 Demo / Screenshots

> *Add images of dashboard, vault with webcam overlay, breach results, etc.*

## ⚙️ Tech Stack

| Layer          | Technology |
|----------------|------------|
| Frontend       | React, Vite, Tailwind CSS, Web Crypto API |
| Backend        | Node.js, Express, JWT, bcrypt |
| Database       | MongoDB Atlas |
| Face Recognition | Python 3.9+, OpenCV, face_recognition, Flask |
| Deployment     | Vercel (frontend) + Render/Railway (backend) + PythonAnywhere (OpenCV service) |

## 🚀 Quick Start

```bash
# Clone
git clone https://github.com/yourusername/secureguard.git
cd secureguard

# Backend setup
cd backend
npm install
cp .env.example .env   # add your JWT secret, MongoDB URI
npm run dev

# Frontend setup (new terminal)
cd frontend
npm install
npm run dev
## 🌍 Real‑World Value

- **Prevents weak password reuse** – the #1 cause of account takeovers.
