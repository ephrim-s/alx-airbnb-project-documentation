# 📌 Airbnb Clone – Backend Requirement Specifications

This document outlines the **technical and functional requirements** for three core backend features of the Airbnb Clone project:  
- User Authentication  
- Property Management  
- Booking System

Each section includes API endpoints, input/output specs, validation rules, and performance expectations.

---

## 🔐 1. User Authentication

### ✅ Functional Requirements
- Users can register as guests or hosts.
- Users can log in with email/password or OAuth (Google/Facebook).
- JWT-based authentication for protected routes.
- Users can update profile information and upload profile photos.

### 🌐 API Endpoints

| Method | Endpoint            | Description                     |
|--------|---------------------|---------------------------------|
| POST   | `/api/auth/register` | Register new user               |
| POST   | `/api/auth/login`    | Login with email/password       |
| POST   | `/api/auth/oauth`    | OAuth login                     |
| GET    | `/api/users/me`      | Fetch authenticated user data   |
| PATCH  | `/api/users/me`      | Update profile info             |

### 🔄 Input/Output Example

**Register Request**
```json
{
  "email": "user@example.com",
  "password": "StrongPass123",
  "role": "host",
  "first_name": "Jane",
  "last_name": "Doe"
}
