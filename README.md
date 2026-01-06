# RK News

**By:**  
- Rafa Salem (4423)  
- Khalifa Miloud (4486)

---

## 1. Project Overview

**RK News** is a full-stack dynamic news platform developed using **HTML, CSS, JavaScript, PHP, and MySQL**.  
The system features a modern **Red/Blue user interface**, comprehensive **multimedia support** (images, video, and audio), **secure user authentication**, and a powerful **administrative dashboard** for managing content.

### Key Features

- **Public Feed:** Visitors can browse news articles, search content, and contact the administration.
- **Authentication:** Secure role-based access control (Admin vs. User).
- **Multimedia Support:** Supports embedded images, direct video files, and audio content.
- **Admin Dashboard:** Full Create, Read, Update, and Delete (CRUD) functionality for news, services, and pages.
- **Dynamic Content:** All sections (About Us, Services, News) are dynamically loaded from the database.

---

## 2. Prerequisites

- XAMPP (or any local server with Apache and MySQL).
- PHP version **7.4** or higher.
- MySQL Database Server.
- A modern web browser (Chrome, Firefox, Edge, etc.).

---

## 3. Setup Instructions

### Step 1: Environment Setup

1. Download and install **XAMPP**.
2. Open the **XAMPP Control Panel**.
3. Start the **Apache** module.
4. Start the **MySQL** module.

### Step 2: Project Installation

Navigate to your XAMPP installation directory (usually `C:\xampp\htdocs\`).  
Create a new folder named **rk_news** and copy all project files into it.

Ensure the following folder structure:

- `assets/` — CSS and JavaScript files  
- `api/` — Backend logic files  
- `includes/` — Header, Footer, Navigation bar  
- Root PHP files (`index.php`, `login.php`, `admin_dashboard.php`, etc.)

### Step 3: Accessing the Application

Open your browser and navigate to:

```
http://localhost/rk_news/
```

---

## 4. Database Migration (Schema)

To set up the database:

1. Open the file "SQL code.pdf" included with the project.
2. Copy the SQL code.
3. Open **phpMyAdmin** at:
   ```
   http://localhost/phpmyadmin
   ```
4. Click the **SQL** tab.
5. Paste the copied code and run it.

---

## 5. Default Credentials

The database is pre-seeded with default user accounts.

| Role  | Username  | Password |
|------|-----------|----------|
| Admin | KhalifaA | 2324 |
| Admin | RafaA    | 0000 |
| User  | KhalifaU | 2324 |
| User  | RafaU    | 0000 |

---

## 6. API Documentation

The system exposes backend endpoints through PHP scripts located in the `api/` directory.  
These endpoints manage **news, comments, services, users**, and public interactions.

### 6.1 News Management

Endpoints are available for adding, editing, and deleting news articles.  
Administrative authentication is required for all operations.

### 6.2 Comment System

Authenticated users can add comments to news articles.  
Comments may be deleted by their owner or an administrator.

### 6.3 Admin Utilities

Administrative utilities include service management and admin user creation or promotion.

### 6.4 Public API

The contact form endpoint is publicly accessible and returns JSON responses indicating success or failure.
