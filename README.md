# 📝 Date Notes

> A minimalist, privacy-first, client-side encrypted daily note-taking & journaling web application.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Status](https://img.shields.io/badge/status-ready-brightgreen.svg)
![Zero Dependencies](https://img.shields.io/badge/dependencies-0-success.svg)

---

## ✨ Features

- 🔒 **Client-Side Encryption (Zero-Knowledge)**
  - AES-GCM 256-bit encryption with PBKDF2 key derivation (250,000 iterations, SHA-256).
  - All notes are encrypted and stored in `localStorage`—passwords and plaintexts never leave your browser.
  - Automatic session timeout & lock after 5 minutes of inactivity.
- 📌 **Visual Sticky-Note Board**
  - Tactile corkboard feel with organic note tilts and 5 pastel color choices.
  - Pin important notes to keep them at the top.
- 📅 **Monthly Calendar View**
  - Switch between Board and Calendar views.
  - Interactive month picker with color-coded dot indicators for days containing notes.
- 🏷️ **Tagging & Instant Filter**
  - Add comma-separated tags to any note.
  - One-click filter chips to quickly view notes by tag.
- 🔍 **Real-Time Search**
  - Filter notes instantly across titles, body text, and tags.
- 💡 **Daily Motivation & Reminders**
  - Rotating motivational quotes with manual refresh.
  - Notification banner showing notes for today and upcoming events in the next 7 days.
- 🌓 **Dark / Light Theme**
  - Toggle between dark and light themes with automatic system preference detection.
- 🚀 **Zero Dependencies**
  - Fully self-contained in standard HTML/CSS/JavaScript. No build step or node modules required!

---

## 🚀 Quick Start

### Run Locally
Simply open `index.html` (or `date-notes.html`) in any modern web browser:
```bash
# On Windows PowerShell
Start-Process index.html

# On macOS
open index.html

# On Linux
xdg-open index.html
```

### GitHub Pages Deployment
1. Go to your repository settings on GitHub: **Settings** > **Pages**.
2. Under **Build and deployment** > **Branch**, select `main` and root `/`.
3. Click **Save**. Your site will be live at `https://ragulk07.github.io/Date-Notes/`.

---

## 🔐 Security Overview

| Parameter | Specification |
|---|---|
| **Cipher** | AES-GCM (256-bit key length) |
| **Key Derivation** | PBKDF2 (`HMAC-SHA-256`) |
| **Iterations** | 250,000 rounds |
| **Salt & IV** | Cryptographically secure random values via Web Crypto API (`crypto.getRandomValues`) |
| **Storage** | Encrypted vault in browser `localStorage` |

> ⚠️ **Important**: Because encryption is zero-knowledge and runs entirely client-side, **forgotten passwords cannot be recovered**. 

---

## 📄 License
This project is open source and available under the [MIT License](LICENSE).
