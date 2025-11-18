#📄 iTECHMobile – Internal Website Repository

Private Repository (iD01tstore Organization)
Public site: https://itechmobile.site


---

📌 Overview

This private repository hosts the official iTECHMobile website, served publicly at:

👉 https://itechmobile.site

The repo itself belongs to the internal brand iD01tstore, but all public-facing branding is iTECHMobile only.

No customer will ever see any GitHub infrastructure — everything is routed through the custom domain.


---

🌐 Deployment (GitHub Pages → Custom Domain)

GitHub Pages builds the site from the main branch or /docs depending on configuration.

The custom domain overrides the GitHub Pages URL.

Required Files

CNAME

Located at project root:

itechmobile.site

GitHub uses this to route traffic correctly.


---

🔧 DNS Configuration (Namecheap)

Set the following DNS records for itechmobile.site:

Type	Host	Value

A	@	185.199.108.153
A	@	185.199.109.153
A	@	185.199.110.153
A	@	185.199.111.153
CNAME	www	iD01tstore.github.io


⚠️ Important:
The GitHub Pages URL will never be shown publicly.
Traffic is always routed to itechmobile.site.


---

📁 Project Structure

iD01tstore/itechmobile-site/
│
├── index.html           # Public landing page
├── assets/              # Images, CSS, icons, animations
├── downloads/           # Installers for the USB Client
├── docs/                # Legal pages, FAQ, security docs
├── CNAME                # Domain binding for itechmobile.site
└── README.md            # (This file)

This repo is strictly for hosting the marketing site, not the actual app code.


---

🚀 Products

iTECHMobile USB Client

Desktop application for customers (Win/macOS/Linux).

iTECHMobile Technician Dashboard

Web-based interface for certified repair technicians.

Both products are distributed outside this repo.


---

🔐 Security Model (Internal Notes)

The website references:

Secure Session™ (custom encrypted tunnel wrapper)

AI Diagnostics Engine

Firebase Realtime Database

Stripe Checkout

ADB-over-TCP orchestration

scrcpy remote control


None of this logic lives in this repo — this repo is static website hosting only.


---

📦 Updating the Website

1. Push commits to main


2. GitHub Pages redeploys automatically


3. Custom domain instantly reflects changes



For critical fixes:

git pull
git add .
git commit -m "Update website"
git push


---

🔒 Privacy

This repository is private, meaning:

Customers cannot access it

The internal brand iD01tstore remains invisible

Only itechmobile.site is exposed publicly


Perfect separation of internal + external identity.


---

🧑‍💻 Internal Contact

Developer: Guillaume Lessard

Brand: iD01tstore

Production platform: iTECHMobile

Support: support@itechmobile.site



---

🏁 Final Notes

This README is intentionally simple because the repo is private and exists only for:

Hosting the website

Redirecting traffic

Managing static assets

