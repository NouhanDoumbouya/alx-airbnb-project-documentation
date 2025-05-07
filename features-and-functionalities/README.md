# Airbnb Clone Backend - Features and Functionalities

This document outlines the key features and functionalities supported by the backend system of the Airbnb Clone project.

## 1. User Management

- **User Registration**: Sign up as guest or host using email/password. OAuth (Google/Facebook) supported.
- **Login and Authentication**: JWT-based session handling for secure access.
- **Profile Management**: Users can upload profile photos and update personal information.

## 2. Property Listings Management

- **Add Listings**: Hosts can add properties with details such as title, location, price, and amenities.
- **Edit/Delete Listings**: Hosts can modify or delete their own listings.

## 3. Search and Filtering

- Search by location, price range, number of guests, and amenities.
- Support for pagination for large search results.

## 4. Booking Management

- **Booking Creation**: Guests can reserve properties for available dates.
- **Booking Status**: Booking lifecycle includes Pending, Confirmed, Cancelled, and Completed.
- **Cancellation**: Hosts or guests can cancel bookings per policy.

## 5. Payment Integration

- Stripe/PayPal integration for secure transactions.
- Upfront payments by guests, scheduled payouts for hosts.
- Multi-currency support.

## 6. Reviews and Ratings

- Guests can leave reviews; hosts can respond.
- Reviews are tied to completed bookings only.

## 7. Notifications

- Email and in-app notifications for bookings, payments, and cancellations.

## 8. Admin Dashboard

- Admins can manage users, listings, bookings, and monitor payments.
