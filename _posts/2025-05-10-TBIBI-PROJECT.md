---
layout: post
title: "Tbibi: Doctor Appointment Booking System"
date: 2025-05-10 12:00:00 +0000
categories: projects
tags: [React, Nodejs, MongoDB, Healthcare, Fullstack, Booking System]
---



## Overview
**Tbibi** is a full-stack **doctor appointment booking platform** developed to streamline the process of connecting patients with healthcare providers. Using **React**, **Node.js**, and **MongoDB**, it provides a responsive UI, robust backend APIs, and role-based access for patients, doctors, and admins.

### Key Features
- **Patient & doctor registration/login**
- **Doctor availability management**
- **Appointment booking system**
- **Admin dashboard for user control**
- **JWT-based authentication**
- **Modern UI with responsiveness**

## Tech Stack

| Layer        | Technology         |
|-------------|---------------------|
| Frontend     | React, Tailwind CSS |
| Backend      | Node.js, Express    |
| Database     | MongoDB             |
| Auth         | JWT (JSON Web Token)|
| Deployment   | Vercel, Render      |

## Core Functionality

### 🔐 Authentication System
- Secure login and registration with role-based access
- Separate dashboard views for doctors, patients, and admins

### 🧑‍⚕️ Doctor Features
- Edit profile: name, bio, specialty, image
- Add/edit weekly availability
- View booked appointments

### 👨‍💻 Patient Features
- Browse doctors by specialty and availability
- Book appointments by selecting date and time
- View upcoming and past appointments

### 🛠️ Admin Dashboard
- Manage all users (view, delete, ban)
- Monitor appointments
- View system statistics

## Example API Endpoint

### POST `/api/appointments/book`

**Request Body:**
```json
{
  "doctorId": "66417ecb1a2d35fa8d7c56a1",
  "patientId": "6641896fbd1457f5a98f36f3",
  "date": "2025-05-15",
  "time": "14:30"
}
```

**Response:**
```json
{
  "status": "success",
  "message": "Appointment booked successfully"
}
```

## Future Improvements
- Integration with **Twilio** for SMS reminders
- **Telemedicine (video calls)** feature
- Advanced search and filtering (by city, specialty, rating)
- **Review system** for patients to rate doctors

## Project Architecture

```text
Frontend (React + Tailwind)
│
├── Auth pages (Login, Register)
├── Dashboard views (Patient, Doctor, Admin)
└── API calls (Axios)

Backend (Node.js + Express)
│
├── Routes
│   ├── /auth
│   ├── /users
│   ├── /appointments
│
├── Middleware (auth, role-check)
└── MongoDB models (User, Appointment, Availability)
```

## Conclusion
**Tbibi** delivers a robust, user-friendly system for healthcare appointment scheduling. It's built to scale and can be easily extended with new features like remote consultations or third-party integrations.

Whether you're building a medical startup or digitizing a private clinic, **Tbibi** provides a reliable foundation.

## Author
**SARAH**
