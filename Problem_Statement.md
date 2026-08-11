# Problem Statement

## 1. Title

Vacation Slot Booking & Tracking Platform

## 2. Domain

Travel / Tourism / Vacation Management

## 3. Who is the user?

### 1. Tourist / Customer
- Searches for available vacation destinations and activities.
- Views available dates and time slots.
- Books vacation slots.
- Makes or views booking status.
- Tracks their booking and itinerary.
- Cancels or modifies eligible bookings.
- Provides reviews and ratings.

### 2. Service Provider
- Manages vacation destinations and activities.
- Creates and manages available slots.
- Updates slot capacity and availability.
- Views customer bookings.
- Updates booking status.

### 3. Admin
- Manages users and service providers.
- Manages destinations and activities.
- Monitors bookings and cancellations.
- Manages complaints and reported issues.
- Views booking and revenue statistics.

## 4. What problem are we solving?

Tourists often face difficulties when planning vacations because
availability, booking slots, activity timings and booking status are
managed across different platforms.

Users may not know whether a particular vacation activity or destination
has available slots before planning their trip. Manual booking processes
can also result in overbooking, scheduling conflicts and difficulty in
tracking reservations.

The proposed system provides a centralized platform where tourists can
search destinations, check real-time slot availability, book vacation
activities and track their booking status in one place.

### Real-life Example

A tourist wants to visit a popular tourist destination and participate
in activities such as boating, sightseeing or adventure activities.

Instead of contacting different service providers, the tourist can use
this platform to check available dates and slots, make a booking and
receive notifications about the booking status.

## 5. Proposed Solution

The application will provide a centralized vacation slot booking and
tracking platform.

### Main Features

- User registration and login
- Destination search
- Activity search
- Date and time slot selection
- Real-time slot availability
- Vacation slot booking
- Booking confirmation
- Booking cancellation
- Booking status tracking
- Tourist itinerary
- Notifications and reminders
- Reviews and ratings
- Service provider dashboard
- Admin dashboard
- Booking and availability reports

The system will automatically update slot availability after every
successful booking to reduce overbooking and scheduling conflicts.

## 6. Core Entities / Database Tables

1. Users
2. Destinations
3. Activities
4. TimeSlots
5. Bookings
6. Payments
7. Reviews
8. ServiceProviders
9. Notifications
10. Itineraries
11. Cancellations
12. Reports

### Important Relationships

- One User can make multiple Bookings.
- One Destination can have multiple Activities.
- One Activity can have multiple TimeSlots.
- One TimeSlot can have multiple Bookings based on its capacity.
- One User can create multiple Reviews.
- One Booking can have one Payment record.
- One User can have an Itinerary containing multiple Bookings.
- Service Providers can manage multiple Activities and TimeSlots.

## 7. User Roles & Permissions

### Admin

- Manage users
- Manage service providers
- Manage destinations
- Manage activities
- Monitor bookings
- Manage cancellations
- Handle complaints
- View reports and statistics

### Tourist / Customer

- Register/Login
- Search destinations and activities
- View available slots
- Book slots
- View booking status
- Cancel eligible bookings
- Manage itinerary
- Receive notifications
- Give reviews and ratings

### Service Provider

- Login
- Manage activities
- Create and update time slots
- Manage slot capacity
- View customer bookings
- Update booking status
- View activity statistics

## 8. Success Criteria

- A tourist should be able to register and log in successfully.
- A tourist should be able to search for destinations and activities.
- The system should display available slots correctly.
- A tourist should be able to book an available slot.
- The system should prevent booking when the slot reaches its capacity.
- Booking status should be updated correctly.
- Users should receive booking confirmation notifications.
- Service providers should be able to manage their slots.
- Admin should be able to monitor bookings and users.
- The system should contain at least 5 relational database tables.

## 9. Out of Scope

The following features will NOT be built in the initial version:

- Actual hotel room management
- Flight ticket booking
- Complete travel agency management
- Real-time vehicle/flight tracking
- Cryptocurrency payments
- Full-scale international payment gateway
- Live video tour

These features may be considered for future development.

## 10. Chosen Track

Java (Spring Boot) + MySQL + React.js

### Third-Party Integration

- Google Maps API – destination location and map services
- Payment Gateway Sandbox – simulated booking payment
- Email / SMS / Firebase – booking notifications

### Future AI Feature

AI-based vacation/activity recommendation and
personalized itinerary generation.
