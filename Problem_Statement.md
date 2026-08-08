# Problem Statement

## 1. Title

**Property Rental Management Platform**

## 2. Domain

**Real Estate / Property Rental Management**

## 3. Who is the user?

* **Admin** – Manages users, properties, rental requests, and bookings.
* **Property Owner** – Adds and manages properties and handles rental requests.
* **Customer / Tenant** – Searches available properties and sends rental requests.

## 4. What problem are we solving?

Property owners and customers often manage rental properties using phone calls, messages, or manual records. This can make it difficult to track available properties, rental requests, and bookings. The platform provides a centralized system where owners can manage properties and customers can easily find and request properties. For example, a customer can search for an available house, send a rental request, and track its status through the platform.

## 5. Proposed Solution

The application will provide:

* User registration and login
* Role-based access for Admin, Owner, and Customer
* Property listing and management
* Property search and availability checking
* Rental request submission
* Rental request approval/rejection
* Booking management
* User and property management by Admin
* Rental request status tracking

## 6. Core Entities / Database Tables

1. **User**
2. **Admin**
3. **Property**
4. **Rental_Request**
5. **Booking**
6. **Payment**
7. **Property_Category**

## 7. User Roles & Permissions

| Role         | Permissions                                                |
| ------------ | ---------------------------------------------------------- |
| **Admin**    | Manage users, properties, requests, and bookings           |
| **Owner**    | Add/update/delete properties and manage rental requests    |
| **Customer** | Search properties, send rental requests, and view bookings |

## 8. Success Criteria

* A customer should be able to search available properties quickly.
* A customer should be able to submit a rental request in under **1 minute**.
* An owner should be able to add and manage a property easily.
* Owners should be able to approve or reject rental requests.
* Customers should be able to view their request and booking status.

## 9. Out of Scope

* Real-time GPS/property tracking
* Actual online payment gateway integration
* Property verification by government authorities
* Video calling between owners and customers
* Mobile application development
* Advanced AI features in the initial version

## 10. Chosen Track

**Java – Spring Boot**

