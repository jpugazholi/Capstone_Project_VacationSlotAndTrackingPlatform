Vaccination Slot Booking & Tracking Platform

Project Overview

The Vaccination Slot Booking & Tracking Platform is a full-stack web application developed to simplify the vaccination appointment process. The platform enables users to securely register, log in, search for available vaccination slots, book appointments, track vaccination status, and manage their vaccination records.

The system also provides an administrator portal to manage vaccination centers, vaccine availability, vaccination schedules, and booking information. It ensures secure access through JWT-based authentication and stores all records in a MySQL database. The application is designed to reduce manual effort, improve scheduling efficiency, and provide a seamless user experience.

---

Objectives

The primary objectives of this project are:

- Develop a secure online vaccination booking system.
- Provide real-time vaccination slot availability.
- Enable users to book and manage vaccination appointments.
- Allow users to track their vaccination status.
- Maintain secure vaccination records.
- Provide an admin dashboard for managing vaccination centers and bookings.
- Implement scheduling logic for efficient slot allocation.
- Support future AI-based demand prediction.

---

Features

User Features

- User Registration
- User Login using JWT Authentication
- View Vaccination Centers
- Search Available Vaccination Slots
- Book Vaccination Appointments
- View Booking History
- Cancel Booked Appointments
- Track Vaccination Status
- View Vaccination Records

Admin Features

- Secure Admin Login
- Manage Vaccination Centers
- Manage Vaccines
- Manage Vaccination Slots
- View User Bookings
- Update Vaccination Status
- Dashboard for Monitoring Bookings

---

Core Modules

Module 1 – Authentication

- User Registration
- User Login
- JWT Token Generation
- Secure API Authentication
- Role-Based Authorization

---

Module 2 – Vaccination Slot Management

- Add Vaccination Centers
- Manage Vaccines
- Create Vaccination Slots
- Update Slot Availability
- Delete Slots
- View Available Slots

---

Module 3 – Booking Management

- Search Available Slots
- Book Vaccination Slot
- Cancel Appointment
- View Booking History
- Track Vaccination Status

---

Module 4 – Admin Dashboard

- View Registered Users
- View Bookings
- Monitor Slot Availability
- Manage Vaccination Data
- Generate Basic Reports

---

Technology Stack

Frontend

- HTML5
- CSS3
- JavaScript

Backend

- Java
- Spring Boot
- Spring MVC
- Spring Data JPA
- Spring Security
- JWT Authentication
- REST API

Database

- MySQL

Development Tools

- IntelliJ IDEA / Eclipse / VS Code
- MySQL Workbench
- Postman
- Git
- GitHub
- Maven

---

System Architecture

+---------------------+
|      Frontend       |
| HTML | CSS | JS     |
+----------+----------+
           |
           | HTTP Request
           |
+----------v----------+
|      Spring Boot    |
| REST API + JWT      |
+----------+----------+
           |
           |
+----------v----------+
|       MySQL         |
| Database Storage    |
+---------------------+

---

Project Structure

VaccinationSlotBookingPlatform
│
├── backend
│   ├── controller
│   ├── service
│   ├── repository
│   ├── entity
│   ├── dto
│   ├── security
│   ├── config
│   └── exception
│
├── frontend
│   ├── html
│   ├── css
│   └── javascript
│
├── database
│   └── vaccination_booking.sql
│
├── docs
│   └── diagrams
│       ├── architecture-v1.png
│       ├── er-diagram-v1.png
│       └── class-diagram-v1.png
│
├── Problem_Statement.md
├── README.md
└── pom.xml

---

Database Tables

The project uses the following database tables:

- Users
- Vaccination_Centers
- Vaccines
- Vaccination_Slots
- Bookings

---

Security Features

The application ensures secure access through:

- Spring Security
- JWT Authentication
- Password Encryption
- Role-Based Access Control
- Secure REST APIs

---

Prerequisites

Before running the project, ensure the following software is installed:

- Java JDK 17 or above
- MySQL Server
- Maven
- Git
- IntelliJ IDEA / Eclipse / VS Code
- Postman

---

Installation

Step 1

Clone the repository.

git clone <repository-url>

---

Step 2

Navigate to the project folder.

cd VaccinationSlotBookingPlatform

---

Step 3

Create the MySQL database.

CREATE DATABASE vaccination_booking;

---

Step 4

Import the SQL script.

database/vaccination_booking.sql

---

Step 5

Update the database configuration inside:

application.properties

Example:

spring.datasource.url=jdbc:mysql://localhost:3306/vaccination_booking
spring.datasource.username=root
spring.datasource.password=your_password

---

Step 6

Build the project.

mvn clean install

---

Step 7

Run the Spring Boot application.

mvn spring-boot:run

---

Step 8

Open the frontend.

http://localhost:8080

---

Application Workflow

User Registration
        │
        ▼
User Login
        │
        ▼
JWT Authentication
        │
        ▼
Search Vaccination Slots
        │
        ▼
Book Appointment
        │
        ▼
Database
        │
        ▼
Track Vaccination Status

---

Future Enhancements

The following features can be implemented in future versions:

- AI-Based Vaccination Demand Prediction
- Smart Slot Allocation
- Email Notifications
- SMS Appointment Reminders
- QR Code Vaccination Certificates
- Cloud Deployment
- Mobile Application
- Online Payment Integration

---

Expected Outcome

The Vaccination Slot Booking & Tracking Platform provides a secure, reliable, and user-friendly solution for managing vaccination appointments. It minimizes manual work, improves slot management, protects vaccination records, and enables efficient administration through a centralized system.

---

Repository

This project follows the standard capstone repository structure and includes:

- Problem Statement
- README
- Architecture Diagram
- ER Diagram
- Class Diagram
- Source Code
- Database Scripts
- Documentation

---

Author

Project Title: Vaccination Slot Booking & Tracking Platform

Course: Bachelor of Technology – Information Technology

Academic Year: 2024–2028

Project Type: Capstone Project

---

License

This project is developed for academic purposes as part of the Capstone Project and is intended for educational use only.
