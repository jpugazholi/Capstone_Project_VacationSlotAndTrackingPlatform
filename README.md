# Problem Statement

## 1. Title
Cloud Bus Pass Management System

## 2. Domain
Transportation Management

## 3. Who is the user? (2-3 user types, with roles)
- Admin – Manages bus pass applications, approves/rejects requests, and maintains records.
- Student/Passenger – Applies for a bus pass, views application status, and renews passes.
- Bus Inspector – Verifies the validity of bus passes during travel.

## 4. What problem are we solving?
Many bus pass systems rely on manual paperwork, making the process slow and inefficient. Users often have to visit transport offices multiple times to apply, renew, or check the status of their bus passes. This results in delays, errors, and unnecessary paperwork. For example, a student may spend hours waiting in line just to renew a bus pass. A digital system simplifies the entire process by allowing users to apply and track their bus passes online.

## 5. Proposed Solution
The application will provide an online platform for bus pass management. Users can register, log in, apply for new passes, renew existing passes, and check application status. Admins can review applications, approve or reject requests, and manage user records. Bus inspectors can verify pass details using the system.

## 6. Core Entities / Database Tables
- Users
- BusPass
- Applications
- Routes
- Payments
- RenewalRequests
- Notifications

## 7. User Roles & Permissions
### Admin
- Manage users
- Approve/Reject applications
- Manage routes
- View reports
- Update bus pass records

### User (Student/Passenger)
- Register/Login
- Apply for a bus pass
- Renew bus pass
- View application status
- Download bus pass

### Bus Inspector
- Verify bus pass
- View passenger details
- Validate pass status

## 8. Success Criteria
- A user should be able to apply for a bus pass in under 2 minutes.
- Admin should be able to approve or reject applications efficiently.
- Users should be able to track application status in real time.
- The system should securely store and manage all bus pass records.

## 9. Out of Scope
- Online payment gateway integration
- SMS or Email notification service
- GPS/live bus tracking
- Mobile application
- AI-based route recommendations

## 10. Chosen Track
Java (Spring Boot)
