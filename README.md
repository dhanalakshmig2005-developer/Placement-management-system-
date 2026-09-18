🎓 Placement Management System

A Java-based Placement Management System that connects students, companies, and administrators through a centralized platform for managing job opportunities, applications, and recruitment activities.

📌 Overview

The Placement Management System is a web-based application designed to simplify and organize the college campus recruitment process.

The system provides separate functionalities for:

- 👨‍🎓 Students — Browse job opportunities, check eligibility, and apply for jobs.
- 🏢 Companies — Manage job openings and review student applications.
- ⚙️ Administrators — Manage student details, company information, job postings, and placement records.

Technologies Used: Java, JDBC, MySQL, HTML, CSS, and JavaScript.

🚀 Features

👨‍🎓 Student Module

- Student registration and login
- View and update student profile
- Browse available job opportunities
- View job details and eligibility criteria
- Apply for suitable job openings
- Track application status

🏢 Company Module

- Company registration and login
- Create and manage job postings
- View student applications
- Review applicant details
- Update recruitment and application status

⚙️ Admin Module

- View and manage student details
- Manage company information
- Add, update, and delete job postings
- Monitor student applications
- Manage placement records
- Oversee placement activities

🛠️ Tech Stack

Technology| Purpose
☕ Java| Backend logic and application functionality
🔗 JDBC| Database connectivity
🛢️ MySQL| Database storage and management
🌐 HTML5| Web page structure
🎨 CSS3| UI styling and layout
⚡ JavaScript| Client-side interactivity
💻 Eclipse IDE / IntelliJ IDEA| Development environment

🏗️ Project Architecture

The project follows a layered architecture to organize database operations, business logic, and application functionality.

PlacementManagementSystem/
│
├── src/
│   ├── controller/
│   ├── dao/
│   ├── model/
│   ├── service/
│   ├── repository/
│   └── util/
│
├── html/
├── css/
├── js/
├── sql/
│   └── schema.sql
│
├── lib/
├── README.md
└── .gitignore

Layer Description

- Controller: Handles user requests and application flow.
- DAO: Performs database operations using JDBC.
- Model: Stores student, company, job, and application data.
- Service: Contains business logic and validation.
- Repository: Organizes data access functionality.
- Util: Contains database connection and utility classes.

«Note: Adjust the folder structure according to your actual project files.»

🗄️ Database Design

The application uses MySQL as its relational database to store and manage placement-related information.

Main Tables

Table| Description
"students"| Stores student information
"companies"| Stores company details
"jobs"| Stores job and placement opportunities
"applications"| Stores student job applications and their status

Basic Relationship

Students
   │
   │ Applies
   ▼
Applications
   │
   │ Belongs to
   ▼
Jobs
   │
   │ Posted by
   ▼
Companies

⚙️ Getting Started

Prerequisites

Make sure the following software is installed:

- ☕ Java JDK
- 🛢️ MySQL Server
- 💻 Eclipse IDE or IntelliJ IDEA
- 🔗 MySQL Connector/J
- 🌐 A modern web browser

1️⃣ Clone the Repository

git clone https://github.com/dhanalakshmig2005-developer/PlacementManagementSystem.git
cd PlacementManagementSystem

2️⃣ Open the Project

1. Open Eclipse IDE or IntelliJ IDEA.
2. Select Open Project or Import Project.
3. Choose the project folder.
4. Configure the Java JDK.
5. Add the required project dependencies.

3️⃣ Configure MySQL

Create the database:

CREATE DATABASE placement_db;

Select the database:

USE placement_db;

4️⃣ Create Database Tables

Execute the SQL script provided in the project:

sql/schema.sql

This creates the required tables for managing students, companies, jobs, and applications.

5️⃣ Configure Database Connection

Configure the database connection in your project.

Example:

db.url=jdbc:mysql://localhost:3306/placement_db
db.user=root
db.password=your_password

⚠️ Security Note: Do not upload database passwords, API keys, or other sensitive credentials to GitHub. Keep configuration files containing secrets out of version control.

6️⃣ Add MySQL Connector/J

1. Download MySQL Connector/J.
2. Add the connector JAR file to your project.
3. Configure it in your IDE's project dependencies.

7️⃣ Run the Application

1. Start the MySQL server.
2. Verify the database connection.
3. Open the project in your IDE.
4. Run the main Java class.
5. Open the frontend HTML file in your browser, if applicable.

📸 Screenshots

Screenshots of the application interface can be added here.

- Student Login Page
- Student Dashboard
- Company Dashboard
- Admin Dashboard
- Job Application Page

🎯 Project Objectives

- Simplify the college placement process.
- Reduce manual placement management.
- Provide students with easy access to job opportunities.
- Help companies manage recruitment activities.
- Enable administrators to maintain placement records efficiently.
- Improve communication between students, companies, and placement officers.

🔮 Future Enhancements

- 📄 Resume upload and management
- 📧 Email notifications for placement updates
- 📊 Admin dashboard with analytics
- 🔐 Improved authentication and authorization
- 🔑 Secure password hashing
- 🔎 Advanced job search and filtering
- 📱 Responsive and mobile-friendly design
- 🌐 REST API integration
- ☁️ Cloud deployment

👨‍💻 Author

Dhanalakshmi G

B.E. Computer Science and Engineering

GitHub: "dhanalakshmig2005-developer" (https://github.com/dhanalakshmig2005-developer)

📄 License

This project is developed for educational and academic purposes.

⭐ Project Goals

The Placement Management System aims to connect students with career opportunities, support companies in recruitment, and help colleges manage placement activities in an organized and efficient way.

---

⭐ Placement Management System — Connecting students with opportunities and companies with talent.
