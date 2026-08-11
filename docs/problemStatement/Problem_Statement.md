# Problem Statement

## 1. Title

**Vaccination Slot Booking & Tracking Platform**

## 2. Domain

**Healthcare / Vaccination Management**

## 3. Who is the User?

The platform consists of three primary user roles:

* **Patient / User**
* **Vaccination Center Staff**
* **Admin**

## 4. Patient / User

Patients can:

* Register and log in securely.
* Search for available vaccination centers.
* View available vaccines.
* View available dates and time slots.
* Book vaccination appointments.
* View booking confirmation.
* Track appointment status.
* Cancel eligible appointments.
* View vaccination history.
* Manage their profile.

## 5. Vaccination Center Staff

Vaccination center staff can:

* Log in securely.
* Manage vaccination center information.
* Manage available vaccines.
* Create and manage vaccination slots.
* Update slot capacity and availability.
* View patient appointments.
* Update appointment status.
* Monitor daily vaccination bookings.

## 6. Admin

Administrators can:

* Manage users.
* Manage vaccination center staff.
* Manage vaccination centers.
* Manage vaccines.
* Monitor vaccination slots.
* Monitor appointments and cancellations.
* View vaccination booking statistics.
* Manage reported issues and complaints.

## 7. What Problem Are We Solving?

People often face difficulties when booking vaccination appointments because vaccination center availability, vaccine information, time slots, and appointment status may be managed through different systems or manual processes.

Users may not know whether a particular vaccination center has the required vaccine or an available appointment slot before visiting the center. Manual booking processes can also lead to overbooking, scheduling conflicts, long waiting times, and difficulty in tracking appointments.

The proposed system provides a centralized platform where users can search for vaccination centers, view available vaccines and time slots, book appointments, and track their vaccination appointment status in one place.

### Real-Life Example

A patient wants to receive a vaccination at a nearby vaccination center.

Instead of contacting multiple centers or visiting them directly, the patient can use the platform to:

1. Search for a vaccination center.
2. View available vaccines.
3. Check available dates and time slots.
4. Book an appointment.
5. Receive booking confirmation.
6. Track the appointment status.

The system automatically updates slot availability after successful bookings to reduce overbooking and scheduling conflicts.

## 8. Proposed Solution

The application will provide a centralized **Vaccination Slot Booking & Tracking Platform**.

### Main Features

* User registration and login
* JWT-based authentication
* Vaccination center search
* Vaccine information
* Vaccination slot management
* Real-time slot availability
* Appointment booking
* Booking confirmation
* Appointment cancellation
* Appointment status tracking
* Vaccination history
* User profile management
* Notifications
* Vaccination center dashboard
* Admin dashboard
* Booking and availability reports

The system will automatically reduce the available slot capacity after a successful booking and prevent new bookings when the slot reaches its maximum capacity.

## 9. Core Entities / Database Tables

The main database entities are:

* Users
* Admins
* VaccinationCenters
* Vaccines
* VaccinationSlots
* Bookings
* Notifications
* Cancellations

### Important Relationships

* One **User** can make multiple **Bookings**.
* One **VaccinationCenter** can have multiple **VaccinationSlots**.
* One **Vaccine** can be associated with multiple **VaccinationSlots**.
* One **VaccinationSlot** can have multiple **Bookings** based on its capacity.
* One **User** can have multiple vaccination records through completed bookings.
* One **Booking** can have one cancellation record when cancelled.
* One **User** can receive multiple **Notifications**.
* A **VaccinationCenter** can provide multiple vaccines.

## 10. User Roles & Permissions

### Admin

* Manage users.
* Manage vaccination center staff.
* Manage vaccination centers.
* Manage vaccines.
* Manage vaccination slots.
* Monitor bookings.
* Manage cancellations.
* Handle complaints.
* View reports and statistics.

### Patient / User

* Register and log in.
* Search vaccination centers.
* View available vaccines.
* View available slots.
* Book vaccination appointments.
* View appointment status.
* Cancel eligible appointments.
* View vaccination history.
* Manage profile.
* Receive notifications.

### Vaccination Center Staff

* Log in securely.
* Manage vaccination center details.
* Manage vaccines.
* Create and update vaccination slots.
* Manage slot capacity.
* View patient bookings.
* Update appointment status.
* View booking statistics.

## 11. Success Criteria

The system should satisfy the following criteria:

* A user should be able to register and log in successfully.
* Authentication should be secured using Spring Security and JWT.
* A user should be able to search vaccination centers.
* A user should be able to view available vaccines and slots.
* A user should be able to book an available vaccination slot.
* The system should prevent booking when the slot reaches its capacity.
* The system should correctly update appointment status.
* Users should receive booking confirmation notifications.
* Users should be able to cancel eligible appointments.
* Vaccination center staff should be able to manage slots.
* Admin should be able to monitor users, centers, vaccines, and bookings.
* The application should expose REST APIs under `/api/v1/`.
* API responses should follow a consistent structure:
  `{ success, data, message }`.
* The application should contain at least five relational database tables.
* Basic backend unit tests should be implemented using JUnit 5.

## 12. Out of Scope

The following features will **NOT** be implemented in the initial version:

* Complete hospital management system
* Doctor appointment management
* Ambulance management
* Real-time medical emergency tracking
* Insurance claim processing
* Advanced medical diagnosis
* Full-scale payment gateway
* Telemedicine / video consultation
* National-level vaccination certificate integration

These features may be considered for future development.

## 13. Chosen Track

**Java Track**

### Technology Stack

* **Frontend:** React.js + Bootstrap / Tailwind CSS
* **HTTP Client:** Axios
* **Backend:** Spring Boot 3.x
* **Programming Language:** Java 17
* **Authentication:** Spring Security + JWT
* **ORM / Data Layer:** Spring Data JPA + Hibernate
* **Database:** MySQL 8
* **Build Tool:** Maven
* **Testing:** JUnit 5
* **API Documentation:** Springdoc OpenAPI / Swagger UI
* **CI/CD:** GitHub Actions
* **Containerization:** Docker — Optional
* **Backend Hosting:** Render / Railway
* **Frontend Hosting:** Vercel / Netlify
* **Database Hosting:** Railway / Clever Cloud / Aiven

## 14. API Standards

The application follows a REST API architecture.

All APIs will be organized under:

```text
/api/v1/
```

Example endpoints:

```text
/api/v1/auth
/api/v1/users
/api/v1/centers
/api/v1/vaccines
/api/v1/slots
/api/v1/bookings
```

### Standard API Response

Every API response should follow a consistent JSON structure:

```json
{
  "success": true,
  "data": {},
  "message": "Operation completed successfully"
}
```

## 15. Third-Party Integration

The initial version may integrate with:

* **Email / SMS / Firebase** – Appointment notifications and reminders.
* **Swagger / OpenAPI** – API documentation.
* **Payment Gateway Sandbox** – Optional simulated payment functionality if required.

## 16. Future AI Feature

An AI-based vaccination assistant may be considered as a future enhancement.

Possible features include:

* Personalized vaccination reminders.
* Vaccine schedule recommendations based on user-provided information.
* Smart appointment suggestions.
* Intelligent vaccination center and slot recommendations.

The AI feature will be considered only after completing the core booking and tracking functionality.
