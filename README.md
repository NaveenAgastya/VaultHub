# VaultHub - 2

<div align="center">

![VaultHub](https://img.shields.io/badge/VaultHub-Secure%20File%20Sharing-2563eb?style=for-the-badge&logo=files&logoColor=white)
![TypeScript](https://img.shields.io/badge/TypeScript-007ACC?style=for-the-badge&logo=typescript&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![Prisma](https://img.shields.io/badge/Prisma-2D3748?style=for-the-badge&logo=prisma&logoColor=white)

**Secure file sharing platform with client-side encryption, expiring links, and download tracking.**

</div>

---

## Overview

VaultHub is a secure file sharing platform designed to make private file transfer simple and controlled.
It lets users encrypt files in the browser, share them through token-based links, and manage access using expiry rules and download limits.

The project includes a React + TypeScript frontend, an Express + Prisma backend, PostgreSQL for metadata storage, and AWS S3 for file delivery.

---

## What VaultHub solves

Sharing sensitive files through email or generic cloud links can be risky.
VaultHub is built around a privacy-first flow so that:

- files are encrypted before upload
- access can be limited by time or download count
- encrypted files can require a password
- download attempts can be tracked
- the share link stays simple for recipients

---

## Features

- 🔐 Client-side file encryption
- 🔗 Token-based share links
- ⏳ Expiring file access
- 📥 Download tracking and activity logs
- 🛡️ Password-protected download flow
- ☁️ AWS S3-backed file delivery
- 🗄️ PostgreSQL metadata storage via Prisma
- 🧾 Local setup script for development

---

## Stack

### Implemented stack
- **Frontend:** React, TypeScript, Vite
- **Backend:** Express, TypeScript
- **Database:** PostgreSQL
- **ORM:** Prisma
- **Storage:** AWS S3
- **Local development:** Docker / Docker Compose

### UI prototype stack
- HTML
- CSS
- JavaScript

---

## How it works

1. A file is uploaded from the frontend.
2. The file is encrypted in the browser before upload.
3. The backend stores metadata in PostgreSQL.
4. The actual file is stored in S3.
5. A unique token link is created for sharing.
6. When a recipient opens the link, the backend validates token, expiry, and download rules.
7. If the file is encrypted, the recipient must provide the password.
8. Each successful download is logged.

---

## Team

- **Naveen** — Upload & Encryption
- **Rahul** — Download & Decryption 

---

## License

MIT
