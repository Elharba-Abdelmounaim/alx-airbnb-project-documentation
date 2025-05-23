# Backend Requirement Specifications

Welcome to the backend requirements documentation for the project. This document outlines the main API endpoints, their expected inputs, outputs, validation rules, and performance criteria.

---

## 1. User Authentication

### Description
Allows users to register and log in to the system securely.

### Endpoints
- `POST /api/register` - Register a new user
- `POST /api/login` - Log in an existing user

### Input

**Register:**
```json
{
  "name": "John Doe",
  "email": "john@example.com",
  "password": "12345678"
}
```Login:

{
  "email": "john@example.com",
  "password": "12345678"
}
```Output
On success (Register):

{
  "message": "User registered successfully"
}
```On success (Login):
{
  "token": "jwt-token",
  "message": "Login successful"
}
