# LMU Liveries

## 📖 Overview

**LMU Liveries** is a full-stack web application designed for the *Le Mans Ultimate* racing community. It provides a modern, high-performance platform for users to upload, share, discover, and download custom car liveries. Built with a .NET 8 API backend and a Nuxt 3 frontend, the project emphasizes a clean user experience, robust features, and a scalable architecture.

---

## ✨ Core Features

*   **User Authentication**: Secure account creation and management using JWT, powered by Supabase.
*   **Transactional Emails**: Reliable email delivery for account confirmation, password resets, and notifications using a robust, proxied SMTP setup.
*   **Livery Upload & Management**: A multi-step, user-friendly form for uploading livery files, screenshots, and detailed specifications.
*   **Advanced Discovery**: Browse, search, and filter liveries by car class, model, and tags with a seamless infinite scroll experience.
*   **Community Interaction**: Users can favorite liveries and view profiles of other creators.
*   **Admin Dashboard**: A comprehensive backend interface for managing users, liveries, reports, and site statistics.
*   **GDPR Compliance**: Built with user privacy in mind, featuring consent management, data export, and account anonymization/deletion tools.
*   **Optimized File Delivery**: Cloudflare-powered CDN integration for fast, cost-effective file downloads with intelligent caching.
*   **Responsive Design**: A seamless experience across desktop and mobile devices.

---

## 🚀 Live Demo

You can view the live, deployed version of the application here:

**[https://lmuliveries.net](https://lmuliveries.net)**

---

## 🛠️ Tech Stack

This project is a modern, decoupled full-stack application.

### Backend (`LmuLiveriesAPI`)

*   **Framework**: .NET 8 Web API
*   **Database**: PostgreSQL
*   **ORM**: Entity Framework Core 8
*   **Authentication**: Supabase (JSON Web Tokens)
*   **File Storage**: Backblaze B2 via AWS SDK for .NET
*   **Email**: Mailjet for reliable SMTP email delivery, triggered by Supabase auth events.

### Frontend (`lmu-liveries-frontend`)

*   **Framework**: Nuxt 3 (Vue 3)
*   **State Management**: Pinia
*   **UI Components**: Nuxt UI & Custom Components
*   **Build Tool**: Vite

### Infrastructure & Deployment

*   **Backend Hosting**: MonsterASP
*   **Frontend Hosting**: Cloudflare Pages
*   **CDN & File Delivery**: Cloudflare with custom domain routing
*   **Email Routing**: Cloudflare Email Routing proxies transactional emails, enhancing deliverability and security.
*   **File Storage**: Backblaze B2 with Cloudflare integration for near-zero egress fees.

---

*During the development of this project, a generative AI assistant was utilized as a tool to aid with tasks such as brainstorming, refactoring, and generating code.*
