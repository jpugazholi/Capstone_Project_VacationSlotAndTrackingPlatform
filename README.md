# 💉 Vaccination Slot Booking & Tracking Platform

A full-stack web application for managing vaccination centers, vaccines, vaccination slots, user appointments, and booking status tracking.

## 📌 Project Overview

The **Vaccination Slot Booking & Tracking Platform** is a web-based application designed to simplify the process of finding vaccination centers, viewing available vaccination slots, booking appointments, and tracking appointment status.

Users can securely register and log in, explore available vaccination centers and vaccines, select suitable vaccination slots, book appointments, and monitor their booking status.

Administrators can manage users, vaccination centers, vaccines, vaccination slots, and appointments through a dedicated admin dashboard.

The platform aims to provide a centralized, secure, and user-friendly solution for efficient vaccination appointment management.

## 🎯 Objectives

* Provide an easy-to-use online vaccination booking system.
* Allow users to register and securely log in.
* Display available vaccination centers and vaccines.
* Allow users to view available vaccination slots.
* Enable users to book vaccination appointments.
* Allow users to track their appointment status.
* Provide administrators with complete management capabilities.
* Maintain vaccination and appointment data efficiently.
* Implement secure authentication and role-based authorization.

## ✨ Key Features

### 👤 User

* User registration
* Secure login
* JWT authentication
* View vaccination centers
* View available vaccines
* View available slots
* Book vaccination appointments
* View booking details
* Track appointment status
* View booking history
* Manage profile

### 🛡️ Admin

* Admin login
* Manage users
* Manage vaccination centers
* Manage vaccines
* Create and manage vaccination slots
* View all appointments
* Approve or reject bookings
* Update booking status
* Monitor vaccination availability

## 🧩 Core Modules

1. Authentication & User Management
2. Vaccination Center Management
3. Vaccine Management
4. Vaccination Slot Management
5. Vaccination Slot Booking
6. Booking Tracking
7. Admin Management

## 🛠️ Tech Stack

### Frontend

* React.js
* HTML5
* CSS3
* JavaScript
* Axios
* React Router

### Backend

* Java
* Spring Boot
* Spring Security
* JWT
* Spring Data JPA
* REST APIs

### Database

* MySQL

### Tools

* Git
* GitHub
* VS Code
* IntelliJ IDEA / Eclipse
* Postman
* MySQL Workbench

## 📂 Project Structure

```text
vaccination-slot-booking/
│
├── frontend/
├── backend/
├── database/
├── docs/
│   └── diagrams/
├── Problem_Statement.md
├── README.md
└── .gitignore
```

## 🔄 Booking Workflow

```text
User Registration
       ↓
      Login
       ↓
User Dashboard
       ↓
Select Vaccination Center
       ↓
Select Vaccine
       ↓
View Available Slots
       ↓
Select Date & Time
       ↓
Confirm Appointment
       ↓
Booking Created
       ↓
Track Booking Status
```

## 🔐 Security

The platform uses **Spring Security and JWT** for secure authentication and authorization.

Security features include:

* JWT-based authentication
* Password protection
* Role-based authorization
* Protected API endpoints
* Admin-only operations
* Secure user sessions

## 🗄️ Main Database Tables

```text
Users
Vaccination_Centers
Vaccines
Vaccination_Slots
Bookings
Admins
```

## 📊 Project Status

**Current Status:** 🚧 In Development

### Completed

* [x] Project idea finalized
* [x] Problem statement
* [x] Repository structure
* [x] Technology stack selection
* [x] Core module planning
* [x] Database planning
* [x] Authentication planning

### In Progress

* [ ] Backend development
* [ ] Frontend development
* [ ] Database implementation
* [ ] JWT authentication
* [ ] Vaccination center management
* [ ] Vaccine management
* [ ] Slot management
* [ ] Booking system

### Planned

* [ ] Booking tracking
* [ ] Admin dashboard
* [ ] Frontend-backend integration
* [ ] Testing
* [ ] Deployment
* [ ] Final documentation

## 🚀 Future Enhancements

* Email notifications
* SMS appointment reminders
* QR code-based appointment verification
* Digital vaccination certificate
* Appointment cancellation and rescheduling
* Advanced admin analytics
* Search and filter functionality
* Cloud deployment
* Mobile application

## 📚 Learning Outcomes

This project provides practical experience in:

* Full-stack web development
* React.js
* Java
* Spring Boot
* Spring Security
* JWT authentication
* REST API development
* MySQL
* JPA and Hibernate
* Git and GitHub
* Postman API testing
* Database design
* Frontend-backend integration
* Role-based access control

## 📝 Conclusion

The **Vaccination Slot Booking & Tracking Platform** provides a centralized digital solution for managing vaccination appointments. By combining React.js, Spring Boot, Spring Security, JWT, and MySQL, the system provides a secure and scalable architecture for users and administrators.

The project demonstrates the practical implementation of authentication, authorization, REST APIs, database management, slot scheduling, appointment booking, and booking status tracking.

## 👩‍💻 Author

**Pugazholi J**

B.Tech Information Technology
J. J. College of Engineering and Technology

## 📄 License

This project is developed for **educational and academic purposes**.
