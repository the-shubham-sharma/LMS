# Library Management System (LMS)

## Overview
This project is a **Library Management System (LMS)** web application created for a technical assignment. The system allows users to search books, issue books, return books, and manage fines. It also provides an **Admin panel** to manage books, memberships, and users.

The system uses **role-based access control**:
- **Admin** → Can access Maintenance, Transactions, and Reports
- **User** → Can access Transactions and Reports only

The main focus of the project is to implement basic library workflows with validations and simple UI forms.

---

## Modules

### 1. Maintenance (Admin Only)
The admin can manage system data.

Features:
- Add Book
- Update Book
- Add Membership
- Update Membership
- User Management

---

### 2. Transactions
Handles library operations.

Features:
- Search available books
- Issue book
- Return book
- Pay fine

Important rules:
- Issue date cannot be before the current date.
- Return date is automatically set to **15 days after issue date**.
- If a fine exists, the user must confirm **Fine Paid** before completing the return.

---

### 3. Reports
Displays basic information such as:
- Available books
- Issued books
- Membership details

---

## Validations

The system performs the following validations:

- Required fields cannot be empty.
- At least one field must be entered when searching books.
- Issue date cannot be earlier than today.
- Return date cannot exceed the allowed limit.
- Error messages appear on the same page if the form is invalid.

---

## Development Approach

The project was developed using a **simple modular approach**:

1. Analyze the assignment requirements.
2. Divide the system into modules (Maintenance, Transactions, Reports).
3. Create pages for login, search, issue, and return book.
4. Implement form validations and role-based access control.

The goal was to build a **minimum working application** that satisfies the assignment requirements.

---

## Assumptions

1. A user can issue **only one book at a time**.
2. The maximum borrowing period is **15 days**.
3. A **daily fine** is charged for late returns.
4. Each book has a **unique serial number**.
5. Only **Admin users** can manage books and memberships.
6. Membership must be **active** to issue books.
7. The system is designed for **demonstration purposes** with basic UI.

LINK:- https://subtle-sprite-794ecb.netlify.app/
