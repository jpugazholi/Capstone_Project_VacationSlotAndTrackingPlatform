# Problem Statement

## Project Title

**Vaccination Slot Booking & Tracking Platform**

## 1. Problem Statement

Managing vaccination appointments can be challenging when users have difficulty finding available vaccination slots, selecting suitable dates and times, and tracking their appointment status.

Vaccination centers also need an efficient way to manage available slots, vaccination capacity, vaccines, centers, and user bookings. Manual or poorly integrated processes can result in outdated slot information, booking conflicts, overbooking, and difficulty maintaining appointment records.

Therefore, a centralized web-based platform is required to simplify vaccination slot management and appointment booking. The proposed system will allow users to securely register, log in, view available vaccination slots, book appointments, and track their booking status. Administrators will be able to manage vaccination centers, vaccines, slots, and bookings through an administrative interface.

---

## 2. Existing System

In a traditional or manual vaccination appointment process:

* Users may need to check availability through different sources.
* Available slots may not be updated efficiently.
* Appointment information may be difficult to track.
* Vaccination centers may manage slots manually.
* Booking conflicts or overbooking may occur.
* Users may not have a centralized platform to manage their appointments.
* Administrators may find it difficult to monitor slot availability and bookings.

---

## 3. Problems in the Existing System

The existing process may have the following problems:

1. Difficulty in finding available vaccination slots.
2. Manual management of vaccination schedules.
3. Possibility of booking conflicts.
4. Risk of slot overbooking.
5. Difficulty in tracking appointment status.
6. Lack of centralized booking information.
7. Inefficient management of vaccination center capacity.
8. Lack of secure authentication and role-based access.
9. Difficulty for administrators to manage slots and bookings efficiently.

---

## 4. Proposed Solution

The proposed **Vaccination Slot Booking & Tracking Platform** is a full-stack web application that provides a centralized system for vaccination appointment management.

The platform will provide secure **Signup and Login** functionality using **JWT authentication**. Registered users can view available vaccination centers, vaccines, dates, and time slots and book an available appointment.

Administrators can manage vaccination centers, vaccines, vaccination slots, and user bookings.

The system will store all relevant information in a centralized **MySQL database**. When a user books or cancels a slot, the available capacity will be updated accordingly.

The application will be developed using **React.js for the frontend, Spring Boot for the backend, MySQL for database management, and Spring Security with JWT for authentication**.

---

## 5. Objectives

The main objectives of the project are:

* To provide secure user registration and login.
* To implement JWT-based authentication.
* To allow users to view available vaccination slots.
* To allow users to book vaccination appointments.
* To allow users to track their booking status.
* To allow users to cancel eligible bookings.
* To allow administrators to manage vaccination centers.
* To allow administrators to manage vaccines.
* To allow administrators to create and manage vaccination slots.
* To prevent overbooking by maintaining slot capacity.
* To maintain centralized appointment records.
* To provide a simple and user-friendly web interface.

---

## 6. Target Users

### 6.1 Users

Users will be able to:

* Create an account.
* Log in securely.
* View vaccination centers.
* View available vaccines.
* View available dates and time slots.
* Book vaccination appointments.
* View booking details.
* Track booking status.
* Cancel eligible appointments.

### 6.2 Administrators

Administrators will be able to:

* Log in securely.
* Manage vaccination centers.
* Manage vaccine information.
* Create vaccination slots.
* Update slot capacity.
* View available slots.
* View user bookings.
* Update booking status.
* Manage booking information.

---

## 7. Core Modules

### Module 1 — Authentication & User Management

Features:

* User Signup
* User Login
* Password validation
* JWT token generation
* Protected APIs
* Role-based access
* User profile

### Module 2 — Vaccination Slot Management

Features:

* Add vaccination center
* Update vaccination center
* Delete vaccination center
* Add vaccine
* Update vaccine
* Delete vaccine
* Create vaccination slots
* Set slot date and time
* Set slot capacity
* Update slot availability

### Module 3 — Vaccination Slot Booking

Features:

* View available slots
* Select vaccination center
* Select vaccine
* Select date
* Select time
* Book a slot
* Receive booking confirmation
* Prevent booking when the slot is full

### Module 4 — Booking Tracking

Features:

* View upcoming appointments
* View booking history
* Track booking status
* Cancel eligible bookings
* View appointment details

---

## 8. Functional Requirements

The system shall:

1. Allow new users to register.
2. Allow registered users to log in.
3. Generate a valid JWT after successful login.
4. Authenticate protected API requests using JWT.
5. Store user information securely in the database.
6. Allow administrators to manage vaccination centers.
7. Allow administrators to manage vaccines.
8. Allow administrators to create vaccination slots.
9. Allow users to view available slots.
10. Allow users to book available slots.
11. Prevent users from booking a full slot.
12. Store booking details in the database.
13. Update slot availability after booking.
14. Allow users to view their bookings.
15. Allow users to cancel eligible bookings.
16. Update slot availability after cancellation.
17. Allow administrators to view and manage bookings.

---

## 9. Non-Functional Requirements

### Security

* Passwords must be stored securely using password hashing.
* JWT must be used for authentication.
* Protected APIs must require valid authentication.
* Users must only be able to access their own booking information.
* Admin functions must be restricted to authorized administrators.

### Performance

* The application should provide quick responses for normal operations.
* Database queries should be efficient.
* Slot availability should be updated consistently.

### Usability

* The interface should be simple and user-friendly.
* Users should be able to book a slot with minimal steps.
* Clear success and error messages should be displayed.

### Reliability

* Invalid requests should be handled safely.
* Full vaccination slots must not accept additional bookings.
* Invalid account or booking operations should not crash the application.

---

## 10. Technology Stack

### Frontend

* React.js
* HTML
* CSS
* JavaScript
* Axios

### Backend

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* Spring Security
* JWT

### Database

* MySQL

### Development Tools

* Git
* GitHub
* VS Code
* IntelliJ IDEA / Eclipse
* Postman

---

## 11. High-Level System Flow

```text
User
  |
  v
React.js Frontend
  |
  v
REST API
  |
  v
Spring Boot Backend
  |
  +----------------------+
  |                      |
  v                      v
Authentication       Business Logic
  |                      |
  v                      v
JWT                 Slot / Booking
                         |
                         v
                      MySQL
                         |
                         v
                    API Response
                         |
                         v
                  React.js Frontend
```

---

## 12. Core End-to-End Modules

### Core Module 1 — Vaccination Slot Management

```text
Admin
  |
  v
React Frontend
  |
  v
Spring Boot REST API
  |
  v
MySQL Database
  |
  v
Updated Slot Information
  |
  v
React Frontend
```

The administrator can create, view, update, and manage vaccination slots.

### Core Module 2 — Vaccination Slot Booking

```text
User
  |
  v
React Frontend
  |
  v
View Available Slots
  |
  v
Select Slot
  |
  v
Spring Boot REST API
  |
  v
Validate Availability
  |
  v
MySQL Database
  |
  v
Booking Confirmation
  |
  v
React Frontend
```

This provides the required **frontend → backend → database → backend → frontend** flow.

---

## 13. Database Entities

The initial database will contain the following major entities:

```text
Users
  |
  └── Bookings
          |
          └── Vaccination Slots
                  |
                  ├── Vaccines
                  |
                  └── Vaccination Centers
```

Main tables:

* `users`
* `vaccines`
* `vaccination_centers`
* `vaccination_slots`
* `bookings`

---

## 14. Scope

### In Scope

* User Signup and Login
* JWT Authentication
* User and Admin roles
* Vaccination center management
* Vaccine management
* Slot management
* Slot booking
* Booking cancellation
* Booking tracking
* Database integration
* REST API
* React frontend
* Admin dashboard
* User dashboard

### Out of Scope

* Medical diagnosis
* Medical recommendations
* Vaccine suitability decisions
* Emergency medical services
* Actual vaccine administration
* Payment processing

---

## 15. Expected Outcome

The expected outcome is a functional full-stack web application that provides a centralized and secure platform for managing vaccination slots and appointments.

The system will allow users to easily find available slots, book appointments, and track their booking status. Administrators will be able to efficiently manage vaccination centers, vaccines, slots, and bookings.

The project will demonstrate complete integration between:

```text
React.js
    ↓
Spring Boot REST API
    ↓
JWT Authentication
    ↓
MySQL Database
    ↓
React.js
```

---

## 16. Success Criteria

The project will be considered successful when:

* Users can successfully register.
* Users can successfully log in.
* A real JWT is issued after successful login.
* Protected APIs require valid authentication.
* Administrators can manage vaccination slots.
* Users can view available vaccination slots.
* Users can book available slots.
* Full slots cannot be overbooked.
* Users can view their bookings.
* Users can track booking status.
* Booking information is stored correctly in MySQL.
* At least two core modules work end-to-end.
* The application can be run locally by following only the instructions in `README.md`.

---

## 17. Future Enhancements

Future versions may include:

* Email appointment notifications.
* SMS reminders.
* QR-code-based appointment verification.
* Advanced analytics dashboard.
* Vaccination demand forecasting.
* Automatic appointment reminders.
* Mobile application support.
* Multi-language support.

