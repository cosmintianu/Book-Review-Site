# Book Review Site

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [User Requirements](#user-requirements)
- [Data Model](#data-model)
- [Technologies Used](#technologies-used)
- [Implementation Details](#implementation-details)
- [Graphical User Interface](#graphical-user-interface)
- [Future Upgrades](#future-upgrades)
- [Setup & Installation](#setup--installation)

---

## Introduction
This Book Review Site is a dedicated platform for critical analysis and discussion of literary works. It allows users to review books, comment on existing reviews, and engage in meaningful literary discussions.

## Features
- User registration and authentication
- Book review submission and commenting system
- Book categorization by genre and author
- Sorting and filtering of books
- Admin functionalities (book management)
- User profile management

## User Requirements
- Unique username, email, password, and age for registration
- Ability to post book reviews
- Ability to comment on existing reviews
- Secure login/logout system

## Data Model
The system follows a relational database model with the following tables:
- **User**: Stores user information
- **Role**: Defines user roles (USER, ADMIN)
- **Book**: Contains book details
- **Author**: Stores book authors (linked via many-to-many relationship)
- **Genre**: Categorizes books
- **Review**: Stores user reviews
- **Comment**: Holds comments on reviews
- **Publisher**: Maintains publisher details

## Technologies Used
### **Backend:**
- Java Spring Boot
- Spring Data JPA
- RESTful API

### **Frontend:**
- React.js

### **Database:**
- PostgreSQL

## Implementation Details
### **Backend Architecture:**
- **Domain Layer:** Defines business entities (User, Book, Review, etc.)
- **Repository Layer:** Handles database interactions
- **Service Layer:** Manages business logic
- **Controller Layer:** Handles HTTP requests

### **Frontend:**
- React components for dynamic UI
- Secure authentication & state management

## Graphical User Interface
- **Login Page:** Secure authentication
- **Create Account Page:** User registration
- **Home Page:** Displays available books
- **Add Book Form:** Allows users to add books
- **Book List Page:** Sort and filter books
- **Individual Book Page:** Book details, reviews, and comments
- **Profile Page:** User account settings

## Future Upgrades
- User-to-user messaging
- Wishlist & Read Books List
- Enhanced security measures
- Additional entity details

## Setup & Installation
1. Clone the repository:
   ```sh
   git clone https://github.com/cosmintianu/Book-Review-Site.git
   ```
2. Navigate to the backend folder and install dependencies:
   ```sh
   cd Back-End
   mvn install
   ```
3. Start the backend server:
   ```sh
   mvn spring-boot:run
   ```
4. Navigate to the frontend folder and install dependencies:
   ```sh
   cd Front-End
   npm install
   ```
5. Start the frontend application:
   ```sh
   npm start
   ```
