# LMU Liveries

## 📖 Overview

**LMU Liveries** is a full-stack web application designed for the *Le Mans Ultimate* racing community. It provides a modern, high-performance platform for users to upload, share, discover, and download custom car liveries. Built with a .NET 8 API backend and a Nuxt 3 frontend, the project emphasizes a clean user experience, robust features, and a scalable, edge-optimized architecture.

---

## ✨ Core Features

*   **User Authentication**: Secure account creation and management using JWT.
*   **Livery Upload & Management**: A multi-step, user-friendly form for uploading livery files, screenshots, and detailed specifications.
*   **Advanced Discovery**: Browse, search, and filter liveries by car class, model, and tags.
*   **Community Interaction**: Users can favorite liveries and view profiles of other creators.
*   **Admin Dashboard**: A comprehensive backend interface for managing users, liveries, reports, and site statistics.
*   **GDPR Compliance**: Built with user privacy in mind, featuring consent management, data export, and account anonymization/deletion tools.
*   **Responsive Design**: A seamless experience across desktop and mobile devices.
*   **High-Performance File Delivery**: Cost-optimized file serving through Cloudflare caching.

---

## 🚀 Live Demo

You can view the live, deployed version of the application here:

**[https://lmuliveries.net](https://lmuliveries.net)**

---

## 🛠️ Tech Stack

This project is a modern, decoupled full-stack application optimized for performance and cost efficiency.

### Backend (`LmuLiveriesAPI`)

*   **Framework**: .NET 8 Web API
*   **Database**: PostgreSQL (Supabase)
*   **ORM**: Entity Framework Core 8
*   **Authentication**: Supabase (JSON Web Tokens)
*   **File Storage**: Backblaze B2 via AWS SDK for .NET
*   **Architecture**: Manager/Service Layer Pattern with relative path storage

### Frontend (`lmu-liveries-frontend`)

*   **Framework**: Nuxt 3
*   **State Management**: Pinia
*   **Routing**: Nuxt Router with file-based routing
*   **Build Tool**: Vite

### Infrastructure & Deployment

*   **Backend Hosting**: MonsterASP
*   **Frontend Hosting**: Cloudflare Workers
*   **File Delivery**: Cloudflare CDN with custom Transform Rules for B2 integration
*   **CDN & Security**: Cloudflare

### File Storage Architecture

*   **Storage Backend**: Backblaze B2 Cloud Storage
*   **Delivery Method**: Cloudflare CDN proxy with intelligent caching
*   **Cost Optimization**: Relative path storage with dynamic URL construction
*   **Cache Strategy**: Aggressive edge caching to minimize origin requests
*   **CORS Configuration**: Optimized cross-origin resource sharing for seamless file access

---

## 🏗️ Architecture Highlights

### Edge-Optimized File Delivery

The application implements a sophisticated file delivery system that minimizes costs while maximizing performance:

1.  **Relative Path Storage**: Files are stored with relative paths in the database.
2.  **Dynamic URL Construction**: The frontend builds full CDN URLs on-demand.
3.  **Cloudflare Transform Rules**: Automatic path rewriting provides seamless B2 integration.
4.  **Intelligent Caching**: Files are cached at the edge after the first request.
5.  **Cost Efficiency**: Reduces Backblaze Class B transactions by ~99% through caching.


*During the development of this project, a generative AI assistant was utilized as a tool to aid with tasks such as brainstorming, refactoring, and generating code.*
