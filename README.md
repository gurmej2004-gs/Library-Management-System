# 📚 Library Management System (LMS)

> A full-stack web-based Library Management System to digitize and automate book records, user management, and issue/return operations — built with PHP, MySQL & Bootstrap.



## 📌 Overview

The **Library Management System (GEHU LMS)** is a web-based application designed to streamline the day-to-day operations of a library. It provides a fully functional admin panel and user portal, enabling efficient management of books, members, and book issue/return workflows — eliminating the need for manual record keeping.

---

## 🎯 Objectives

- Digitize and automate library operations end-to-end
- Improve accuracy and accessibility of book and member records
- Reduce administrative workload through a structured database-driven system
- Provide a clean, user-friendly interface for both admins and students

---

## ✨ Key Features

### 👤 User Side
- 🔐 User registration, login & logout
- 📖 View issued books and due dates
- 👤 View and edit profile
- 🔑 Change password functionality

### 🛠️ Admin Side
- 📚 Add, update, and delete book records
- 👥 Manage student/member registrations
- 📋 Issue and return books
- 📊 View all active book issues and history
- 🔍 Search and filter records

### ⚙️ System
- MySQL database backend with structured schema (`lms.sql`)
- Session-based authentication
- Bootstrap-powered responsive UI

---

## 🛠️ Tools & Technologies

| Technology | Role |
|---|---|
| PHP | Backend server-side logic |
| MySQL | Database for books, users & transactions |
| Bootstrap 5 | Responsive UI framework |
| HTML & CSS | Page structure and styling |
| JavaScript | Frontend interactivity |

---

## 📁 Project Structure

```
Library-Management-System/
│
├── index.php                  # Login page
├── register.php               # New user registration
├── signup.php                 # Signup handler
├── logout.php                 # Session logout
│
├── user_dashboard.php         # Student dashboard
├── view_issued_book.php       # View books issued to user
├── view_profile.php           # User profile viewer
├── edit_profile.php           # Edit profile details
├── change_password.php        # Password change form
├── update_password.php        # Password update handler
├── update.php                 # General update handler
│
├── admin/                     # Admin panel (CRUD for books & members)
├── bootstrap/                 # Bootstrap CSS/JS assets
│
├── lms.sql                    # MySQL database schema & seed data
└── README.md                  # Project documentation
```

---

## 🚀 Getting Started

### Prerequisites

- [XAMPP](https://www.apachefriends.org/) or any PHP + MySQL server (Apache, WAMP, LAMP)
- PHP 7.4+
- MySQL 5.7+

### Installation Steps

```bash
# 1. Clone the repository
git clone https://github.com/gurmej2004-gs/Library-Management-System.git

# 2. Move to your server's web root
# For XAMPP: copy the folder to C:/xampp/htdocs/
cp -r Library-Management-System/ /xampp/htdocs/lms/
```

**3. Import the Database**
- Open **phpMyAdmin** → `http://localhost/phpmyadmin`
- Create a new database named `lms`
- Click **Import** → select `lms.sql` → click **Go**

**4. Configure Database Connection**
- Open the database config file (inside `admin/` or root)
- Update with your local credentials:
```php
$host = "localhost";
$user = "root";
$password = "";
$database = "lms";
```

**5. Run the App**
- Open your browser and navigate to:
```
http://localhost/lms/index.php
```

---

## 🖥️ Usage

| Role | URL | Default Credentials |
|---|---|---|
| Admin | `/admin/` | Set during setup |
| User | `/index.php` | Register a new account |

---

## 🗃️ Database Schema

The `lms.sql` file includes tables for:

- **users** — member/student records and credentials
- **books** — book catalogue with title, author, category
- **issued_books** — active issue records with dates
- **admin** — admin login credentials

---

## 💡 Use Cases

- 🏫 **School / College libraries** — manage student book borrowing
- 🏢 **Office libraries** — track internal resource lending
- 📖 **Small public libraries** — digitize catalogues and member records

---

## 🎓 Skills Demonstrated

- ✅ Full-stack web development (PHP + MySQL)
- ✅ CRUD operations and relational database design
- ✅ Session-based authentication & access control
- ✅ Responsive UI design with Bootstrap
- ✅ Admin & user role separation
- ✅ Real-world system design and implementation

---


## 📄 License

This project is open source and available for educational and personal use.

---
