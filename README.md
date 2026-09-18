# 🎓 SmartPlacementSystem

A **Java-based Smart Placement Management System** that connects students, companies, and administrators through a streamlined platform for managing job opportunities, applications, and recruitment.

----

## 📌 Overview

**SmartPlacementSystem** is a full-stack placement management application designed to simplify the campus recruitment process.

The system provides separate functionality for:

* 👨‍🎓 **Students** — discover and apply for job opportunities
* 🏢 **Companies** — post jobs and manage applicants
* ⚙️ **Administrators** — manage students, companies, jobs, and applications

The project is built using **Java, JDBC, MySQL, HTML, CSS, and JavaScript**.

---

## 🚀 Features

### 👨‍🎓 Student

* 📝 Student registration and login
* 🔍 Browse available job opportunities
* 📄 View job details
* 📩 Apply for jobs
* 📊 Track application status
* 👤 Manage student information

### 🏢 Company

* 📝 Company registration and login
* 📢 Create and publish job openings
* 👀 View student applications
* 🔎 Review applicant information
* 🛠️ Manage recruitment and application status

### ⚙️ Admin

* 👨‍🎓 View and manage students
* 🏢 View and manage companies
* 💼 Manage job postings
* 📩 Monitor applications
* 🔍 Oversee the complete placement process

---

## 🛠️ Tech Stack

| Technology           | Purpose                                     |
| -------------------- | ------------------------------------------- |
| ☕ **Java**           | Backend logic and application functionality |
| 🔗 **JDBC**          | Database connectivity                       |
| 🛢️ **MySQL**        | Data storage and management                 |
| 🌐 **HTML5**         | Web page structure                          |
| 🎨 **CSS3**          | UI styling and layout                       |
| ⚡ **JavaScript**     | Client-side interactivity                   |
| 💻 **IntelliJ IDEA** | Development environment                     |

---

## 🏗️ Architecture

The project follows a layered structure to keep database operations, business logic, models, and controllers organized.

```text
SmartPlacementSystem/
│
├── src/
│   ├── controller/       # Handles application requests
│   ├── dao/              # Database access using JDBC
│   ├── model/            # POJO / entity classes
│   ├── service/          # Business logic
│   └── util/             # Utilities and database configuration
│
├── view/
│   ├── html/             # HTML pages
│   ├── css/              # Stylesheets
│   ├── js/               # JavaScript files
│   └── images/           # Images and other assets
│
├── sql/
│   └── schema.sql        # Database schema
│
├── lib/
│   └── mysql-connector/  # MySQL JDBC driver
│
└── README.md
```

---

## 🗄️ Database Design

The application uses **MySQL** as its relational database.

### Main Tables

| Table          | Description                                      |
| -------------- | ------------------------------------------------ |
| `students`     | Stores student information                       |
| `companies`    | Stores company information                       |
| `jobs`         | Stores job and placement opportunities           |
| `applications` | Stores student job applications and their status |

### Basic Relationship

```text
Students
   │
   │ applies
   ▼
Applications
   │
   │ belongs to
   ▼
Jobs
   │
   │ posted by
   ▼
Companies
```

---

## ⚙️ Getting Started

### Prerequisites

Make sure the following are installed:

* ☕ Java JDK
* 🛢️ MySQL Server
* 💻 IntelliJ IDEA
* 🔗 MySQL Connector/J
* 🌐 A modern web browser

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/jiteshkhatri11/SmartPlacementSystem.git
cd SmartPlacementSystem
```

---

### 2️⃣ Open in IntelliJ IDEA

1. Open **IntelliJ IDEA**
2. Select **Open Project**
3. Choose the cloned `SmartPlacementSystem` directory
4. Allow IntelliJ to configure the project

---

### 3️⃣ Configure MySQL

Create the database:

```sql
CREATE DATABASE placement_db;
```

Select the database:

```sql
USE placement_db;
```

---

### 4️⃣ Run the Database Schema

Execute the SQL file:

```text
sql/schema.sql
```

This will create the required tables and database structure.

---

### 5️⃣ Configure Database Connection

Create:

```text
src/util/db.properties
```

Add your MySQL configuration:

```properties
db.url=jdbc:mysql://localhost:3306/placement_db
db.user=root
db.password=your_password
```

> ⚠️ Do not commit passwords or other sensitive credentials to GitHub.

For local development, consider adding `db.properties` to `.gitignore`.

---

### 6️⃣ Add MySQL Connector/J

Download **MySQL Connector/J** and place the JAR inside:

```text
lib/
```

Then add the JAR to the project's dependencies in IntelliJ IDEA.

---

### 7️⃣ Run the Application

Open the main HTML entry point:

```text
view/html/index.html
```

Run it using your preferred browser.

---

## 📸 Screenshots

Screenshots and UI demonstrations will be added soon.

> 🚧 **Coming Soon**

---

## 🔮 Future Improvements

The project can be extended with several features:

* 📄 Resume upload and management
* 📧 Email notifications
* 📊 Admin dashboard and analytics
* 🔐 Improved authentication and authorization
* 🔑 Password hashing and security improvements
* 🔎 Advanced job search and filtering
* 📱 Responsive/mobile-friendly UI
* 🌐 REST API integration
* 🏗️ Migration from JDBC-based architecture to **Spring Boot**
* 🗃️ Improved database validation and transaction management
* ☁️ Cloud deployment

---

## 🎯 Project Goals

The main objectives of SmartPlacementSystem are to:

* Simplify the student placement process
* Reduce manual placement management
* Provide companies with an organized applicant-management system
* Give administrators centralized control
* Create a foundation for a scalable recruitment platform

---

## 👨‍💻 Author

### Jitesh Khatri

GitHub: **jiteshkhatri11**

---

## 📄 License

This project is licensed under the **MIT License**.

See the `LICENSE` file for more information.

---

## ⭐ Support

If you find this project useful:

⭐ **Star** the repository
🍴 **Fork** the repository
🛠️ **Contribute** improvements
🐛 **Report** issues

---

## 📌 Project Status

**🚧 Active Development**

New features, UI improvements, security enhancements, and documentation will be added over time.

---

### ⭐ SmartPlacementSystem

> **Connecting students with opportunities and companies with talent.**
