# Airbnb Clone Backend - Requirement Specifications

This document details the technical and functional specifications of key backend features.

---

## 1. User Authentication

### API Endpoints
- `POST /api/auth/register`
- `POST /api/auth/login`

### Input
- Email, password (hashed), name, user role (guest/host)

### Output
- JWT token, user profile data

### Validation
- Unique email
- Password minimum 8 characters

### Performance
- Response time < 500ms
- Secure password storage using bcrypt

---

## 2. Property Management

### API Endpoints
- `POST /api/properties`
- `PUT /api/properties/:id`
- `DELETE /api/properties/:id`
- `GET /api/properties`

### Input
- Title, description, location, price, amenities, images

### Output
- Property listing objects

### Validation
- Required fields: title, price, location
- Only hosts can manage listings

### Performance
- Database indexing on location and price for optimized search

---

## 3. Booking System

### API Endpoints
- `POST /api/bookings`
- `GET /api/bookings/:userId`
- `PATCH /api/bookings/:id/status`

### Input
- Property ID, guest ID, booking dates

### Output
- Booking confirmation object

### Validation
- No overlapping bookings
- Dates must be valid

### Performance
- Date conflict check optimized
- Response < 700ms under load

---
