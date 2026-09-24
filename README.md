# EduSupport - Student Support & Ticket Management (Assignment 4)

A complete SLA & Ownership based ticket system for student issues like Fees, ID Card, Attendance, Certificates.

**Live Proof:** Backend runs on `localhost:8080` and Frontend on `5500` with Management Visibility Dashboard.

### Features Implemented
- **Ticket Lifecycle:** OPEN -> IN_PROGRESS -> RESOLVED
- **SLA Auto Calculation:** HIGH=24h, MEDIUM=48h, LOW=72h
- **Ownership & Assignment:** Assign to Admin1/Admin2 etc
- **Ageing:** 0m old, 1h old tracking
- **Management Visibility:** Total / Pending / In Progress / Overdue / Escalated cards
- **Resolution Tracking & Activity**

### Tech Stack
Backend: Spring Boot 3, Spring Data JPA, H2 In-Memory DB, REST API
Frontend: HTML, CSS, Vanilla JS (Fetch API)
Build: Maven

### How to Run
1. Backend: 
   cd helpdesk
   .\mvnw.cmd spring-boot:run
   -> http://localhost:8080/api/tickets

2. Frontend: 
   Open frontend/index.html with Live Server
   -> http://127.0.0.1:5500/frontend/index.html

### API Endpoints
GET /api/tickets - Get all tickets
POST /api/tickets - Create ticket
PUT /api/tickets/{id} - Update status/owner

### Screenshots
- Management dashboard with BLUE cards showing Owner, Priority, SLA Deadline
- Overdue detection logic

Author: Kamasani Dhanush
Assignment 4 - Pre-Drive Product Engineering
