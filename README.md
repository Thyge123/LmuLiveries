# LMU Liveries

## 📖 Overview

**LMU Liveries** is a full-stack web application designed for the *Le Mans Ultimate* racing community. It provides a modern, high-performance platform for users to upload, share, discover, and download custom car liveries. Built with a .NET 8 API backend and a Nuxt 3 frontend, the project emphasizes a clean user experience, robust features, and a scalable architecture.

---

## ✨ Core Features

*   **User Authentication**: Secure account creation and management using JWT.
*   **Livery Upload & Management**: A multi-step, user-friendly form for uploading livery files, screenshots, and detailed specifications.
*   **Advanced Discovery**: Browse, search, and filter liveries by car class, model, and tags.
*   **Community Interaction**: Users can favorite liveries and view profiles of other creators.
*   **Admin Dashboard**: A comprehensive backend interface for managing users, liveries, reports, and site statistics.
*   **GDPR Compliance**: Built with user privacy in mind, featuring consent management, data export, and account anonymization/deletion tools.
*   **Responsive Design**: A seamless experience across desktop and mobile devices.
*   **Optimized File Delivery**: Cloudflare-powered CDN integration for fast, cost-effective file downloads with intelligent caching.

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

### Frontend (`lmu-liveries-frontend`)

*   **Framework**: Nuxt 3
*   **State Management**: Pinia
*   **Build Tool**: Vite

### Infrastructure & Deployment

*   **Backend Hosting**: MonsterASP
*   **Frontend Hosting**: Cloudflare Pages
*   **CDN & File Delivery**: Cloudflare with custom domain routing
*   **File Storage**: Backblaze B2 with Cloudflare integration

---

*During the development of this project, a generative AI assistant was utilized as a tool to aid with tasks such as brainstorming, refactoring, and generating code.*

