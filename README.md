# SECURITY_SERVICE
security company from Roy
 Security Company Management System

A Django-based application to manage a security company's operations, including guards, clients, sites, assignments, incidents, and equipment.  

This project also features a **custom Django admin** interface called **Blog MOHAPI ADMIN** for managing models with a customized header and look.

---

## Features

- **Employee Management:** Manage security guards and their details.
- **Client Management:** Track clients and associated sites.
- **Site Management:** Maintain information about security locations.
- **Shift Assignments:** Assign guards to sites with start and end times.
- **Incident Logging:** Record security incidents linked to assignments.
- **Equipment Tracking:** Assign and manage equipment to guards.
- **Custom Admin Interface:** Uses a custom `AdminSite` (`BlogAdminArea`) with a personalized header.

---

## Models

### 1. Guard
- `user`: Linked to Django `User` for authentication
- `employee_id`, `phone`, `is_active`

### 2. Client
- `name`, `company_name`, `email`, `phone`

### 3. Site
- `client`, `name`, `address`, `active`

### 4. Assignment
- `guard`, `site`, `start_time`, `end_time`

### 5. Incident
- `assignment`, `title`, `description`, `reported_at`

### 6. Equipment
- `name`, `assigned_to`, `serial_number`

---
