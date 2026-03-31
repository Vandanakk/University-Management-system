# University Management System — Role-Based Event Platform

A role-based University Event Management platform with vendor bidding, real-time sponsorship tracking, and multi-stakeholder coordination. Built with PHP, MySQL, and XAMPP.

## 🛠 Tech Stack

- **Backend:** PHP
- **Database:** MySQL
- **Local Server:** XAMPP (Apache)
- **Frontend:** HTML, CSS, JavaScript

## User Roles

| Role | Capabilities |
|------|-------------|
| Admin | Manage events, approve vendors, view all bids |
| Vendor | Submit bids for events, track bid status |
| Sponsor | View sponsorship opportunities, track contributions |
| Student | Browse events, register, view schedules |

## Key Features

- Role-based access control — each user sees only what they need
- Vendor bidding system — vendors submit proposals, admins approve/reject
- Sponsorship tracking dashboard — real-time view of contribution status
- Multi-stakeholder coordination — admins, vendors, sponsors, and students on one platform

## Database Schema

Core tables:
- `users` — id, name, email, password, role
- `events` — id, title, date, budget, status
- `vendors` — id, user_id, company_name, category
- `bids` — id, vendor_id, event_id, amount, status
- `sponsorships` — id, sponsor_id, event_id, amount, confirmed

## How to Run

```bash
# Requirements: XAMPP installed

1. Clone this repo into your XAMPP /htdocs folder
2. Start Apache and MySQL in XAMPP Control Panel
3. Import database/schema.sql into phpMyAdmin
4. Open http://localhost/university-management-system
```

## What I Learned

- Designing a normalized relational schema for multi-role systems
- Implementing role-based access control in PHP sessions
- Building a bidding workflow with state transitions (pending → approved → rejected)
- Coordinating between multiple user types in a single platform

## Status

Core schema and role-based architecture designed. PHP implementation in progress.
Copy
