Library Management System (LMS)
Overview

This project is a Library Management System web application developed as part of a technical assignment. The system allows users to search books, issue books, return books, and manage fines. It also provides an Admin panel for managing books, memberships, and users.

The system has role-based access control:

Admin can access Maintenance, Transactions, and Reports modules.

User can access only Transactions and Reports.

The application focuses on implementing basic library operations, validations, and simple UI forms.

Modules
1. Maintenance (Admin Only)

Admin can manage system data.

Features:

Add Book

Update Book

Add Membership

Update Membership

User Management

2. Transactions

Handles library operations.

Features:

Search available books

Issue book

Return book

Pay fine

Important rules:

Issue date cannot be before today.

Return date is automatically set to 15 days after issue date.

Fine must be confirmed before completing a return transaction if applicable.

3. Reports

Displays basic information such as:

Available books

Issued books

Membership details

Validations

The system includes form validations such as:

Required fields cannot be empty.

At least one field must be entered when searching books.

Issue date cannot be earlier than the current date.

Return date cannot exceed the allowed limit.

Error messages are displayed on the same page.

Development Approach

The project was developed using a modular approach:

Understand the requirements and identify system modules.

Design pages for login, transactions, and maintenance.

Implement forms with validations.

Connect modules to simulate a basic library workflow.

The focus was on building a minimum working system that satisfies the assignment requirements.

Assumptions

A user can issue only one book at a time.

The maximum borrowing period for a book is 15 days.

A fine is charged per day if a book is returned after the due date.

Each book has a unique serial number.

Only Admin users can manage books and memberships.

Membership must be active for issuing books.

The system is designed for basic demonstration purposes with simple UI.
