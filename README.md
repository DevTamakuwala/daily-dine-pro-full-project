# Daily Dine Pro – Full Project Overview

This repository **daily-dine-pro-full-project** is the central documentation hub for the complete **Daily Dine Pro** ecosystem.

Daily Dine Pro is a platform that connects **customers** with **mess owners**, helping users discover nearby messes, view daily menus, and manage operations through dedicated interfaces for admins, mess owners, and customers.

The full project is split into three main repositories:

- **Admin Web Panel (React.js)**
- **Customer, Mess Owner & Admin Mobile App (Flutter)**
- **Backend REST API (Spring Boot)**

---

## 🔗 Repositories

### 1. Admin Panel – React.js

**Repository:**  
👉 https://github.com/DevTamakuwala/daily-dine-pro-admin-react  

**Role in the system:**

- Web-based **admin dashboard** for platform administrators.
- Manage and monitor:
  - Users (customers, mess owners, admins)
  - Mess listings and details
  - Platform operations and configuration
- Provides an overview of the entire system to keep everything running smoothly.

**Tech stack:**

- React.js
- JavaScript, HTML, CSS
- Consumes APIs from the Spring Boot backend

---

### 2. Mobile App – Flutter

**Repository:**  
👉 https://github.com/DevTamakuwala/daily-dine-pro-flutter  

**Role in the system:**

- Main **mobile application** used by:
  - **Customers** – discover nearby messes, view menus, interact with mess owners.
  - **Mess Owners** – manage their mess profile, menu, and customer-facing information.
  - **Admins** – limited admin functionality on mobile.
- Provides the core daily experience for end users on Android/iOS.
- Communicates with the Spring Boot backend for all data (auth, mess data, menus, etc.).

**Tech stack:**

- Flutter (Dart)
- Targets Android (and can be extended to iOS)
- Integrates with the Spring Boot API

---

### 3. Backend API – Spring Boot

**Repository:**  
👉 https://github.com/DevTamakuwala/daily-dine-pro-spring-boot  

**Role in the system:**

- **Central backend** that powers both:
  - Flutter mobile app
  - React admin panel
- Responsibilities:
  - User authentication & authorization
  - Business logic for customers, mess owners, and admins
  - Mess, menu, and related data management
  - Exposes REST APIs for all frontends
  - Integrates with a relational database for persistent storage

**Tech stack:**

- Java + Spring Boot
- Maven for build
- REST APIs for communication with clients

---

## 🧩 How Everything Fits Together

- The **Flutter App** and **React Admin Panel** both communicate with the **Spring Boot Backend** via REST APIs.
- All **core data and business rules** live in the backend.
- The **admin panel** focuses on management & oversight.
- The **mobile app** focuses on daily usage by customers and mess owners.

---

## 📁 This Repository (daily-dine-pro-full-project)

This repo is meant to:

- Give a **single place** to understand the full architecture.
- Provide **links** to each codebase.
- Explain **which repo does what** for easier navigation and onboarding.

You can clone each repo individually as needed:

```bash
# Admin panel
git clone https://github.com/DevTamakuwala/daily-dine-pro-admin-react

# Flutter mobile app
git clone https://github.com/DevTamakuwala/daily-dine-pro-flutter

# Spring Boot backend
git clone https://github.com/DevTamakuwala/daily-dine-pro-spring-boot
