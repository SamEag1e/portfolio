# BeautyPlus – Skincare E-Commerce Platform

> **Status:** Live | In Development | Private Codebase  
> **Tech Stack:** Django • PostgreSQL • Docker • Nginx • Cloudflare SSL • HTML • CSS • JavaScript • jQuery

---

## Overview

This project is a fully functional e-commerce platform built with Django.  
It features user authentication via OTP, recursive product categories, and user/admin panels.

Originally developed as a real-world project, it is **currently live at:**  
[irbeautyplus.com](https://irbeautyplus.com)

---

## Key Features

### Authentication System

- **OTP-based login** using phone numbers — a secure, password-less approach

### Modular E-Commerce Backend

- **Recursive product categories** using MPTT
- **Extensible Core Apps:** Built modular from day one — including Products, Carts, Orders, Notifications, Tags, and Accounts

### Project Structure & Design Philosophy

- **Modular code structure**: Models, forms, and admin classes are split into separate modules — even for simpler apps
  - This design optimizes for long-term maintainability, localization (e.g., i18n), and easy admin customization
- Introduced a **service layer (singleton class per model)** to centralize business logic
  - Inspired by best practices from **NestJS** and other backend frameworks
  - Helps isolate logic and reduce tight coupling between apps

### SEO & Social Media Optimization

- **Auto-generated meta tags** tailored for products, brands, and categories
- Dynamic **Open Graph images (og:image)** for rich social media previews
- **JSON-LD schema markup** for products to boost search engine understanding and rich results
- Fully managed **sitemap generation** with Django to keep search engines updated
- Clean, **smart hierarchical slugs** powering SEO-friendly URLs with clear category and product nesting

### Deployment & Infrastructure

- **Dockerized** for consistent and portable deployments
- Configured **Nginx** as a reverse proxy with **Certbot** for automated SSL certificates
- DNS managed via **Cloudflare** for performance and security
- **Cron jobs** set up for routine maintenance tasks

### Backup & Disaster Recovery

- Automated daily backups using `rclone` to Google Drive
- Backups are lightweight, encrypted, and versioned to ensure data integrity and project continuity

---

## Screenshots

![beautyplus-source](./assets/beautyplus-source.png)
![beautyplus-homepage](./assets/beautyplus-homepage.png)
![beautyplus-shoppage](./assets/beautyplus-shoppage.png)
![beautyplus-user-dashboard](./assets/beautyplus-user-dashboard.png)
![beautyplus-admin](./assets/beautyplus-admin.png)

---

## Access or Demo

The codebase is in a private repository.

<p>
    Contact me if you'd like access or a walkthrough of the architecture.
    <a href="mailto:samadeagle@yahoo.com" target="_blank" rel="noreferrer">
    <img src="https://img.icons8.com/fluency/20/new-post.png" width="20" height="20" alt="Email" style="display:inline; text-decoration: none; vertical-align:middle; margin: 0 6px;" />
    </a>
    <a href="https://wa.me/989146446078" target="_blank" rel="noreferrer">
    <img src="https://img.icons8.com/color/20/whatsapp--v1.png" width="20" height="20" alt="WhatsApp" style="display:inline; text-decoration: none; vertical-align:middle; margin: 0 6px;" />
    </a>
    <a href="https://t.me/SamadTnd" target="_blank" rel="noreferrer">
    <img src="https://img.icons8.com/ios-filled/20/0088cc/telegram-app.png" width="20" height="20" alt="Telegram" style="display:inline; text-decoration: none; vertical-align:middle; margin: 0 6px;" />
    </a>
    <a href="https://www.linkedin.com/in/samad-taghinejad/" target="_blank" rel="noreferrer">
    <img src="https://raw.githubusercontent.com/danielcranney/readme-generator/main/public/icons/socials/linkedin.svg" width="20" height="20" alt="LinkedIn" style="display:inline; text-decoration: none; vertical-align:middle; margin: 0 6px;" />
    </a>
</p>

---

## Lessons & Next Steps

- Explored Django’s **GenericForeignKey**, `ContentType`, and `GenericRelation` mechanics
- Ultimately chose **explicit, readable design** over abstract “magic”:
  - Ratings implemented via a `BaseRate` model inherited per target type, even though this feature is not yet live on the UI (e.g., `ProductRate`, `BlogRate`)
  - Categories follow the same logic (`BaseCategory` → `ProductCategory`, `BlogCategory`, etc.)
- Result: **clearer models**, **cleaner queries**, better admin integration, and more maintainable code
- Learned deep integrations of Django with real deployment scenarios
- Future plans: Add payment gateway, refine order flow, improve admin UX

### 🔙 [Back to Project Index](../README.md)
