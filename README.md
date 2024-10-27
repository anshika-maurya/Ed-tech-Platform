# Studynotion: An Online Education Platform

## Website Link
[Studynotion - Live Demo](#) *https://ed-tech-platform-khaki.vercel.app/*

## Overview
**Studynotion** is an ed-tech platform built with the **MERN stack** (MongoDB, ExpressJS, ReactJS, NodeJS) designed to enhance educational accessibility and engagement. Users can create, consume, and rate educational content, while instructors can showcase expertise, connect with learners globally, and manage courses.

## Table of Contents
1. [Project Description](#project-description)
2. [System Architecture](#system-architecture)
3. [Front-end](#front-end)
4. [Back-end](#back-end)
5. [Database](#database)
6. [API Design](#api-design)
7. [Deployment](#deployment)
8. [Testing](#testing)
9. [Future Enhancements](#future-enhancements)

---

## Project Description
StudyNotion aims to provide:
- A **seamless learning experience** for students through an interactive interface.
- A **platform for instructors** to share their expertise and connect with learners globally.

---

## System Architecture
StudyNotion follows a **client-server architecture** with:
- **Front-end**: ReactJS application for a dynamic, user-friendly interface.
- **Back-end**: NodeJS and ExpressJS, providing RESTful APIs for authentication, course management, and more.
- **Database**: MongoDB for storing courses, user information, and other data.

### Architecture Diagram



---

## Front-end
The front-end application, built with **ReactJS**, includes:
- **For Students**:
  - **Homepage**: Introduction and links to courses and user details.
  - **Course List**: Browse available courses.
  - **Wishlist**: View saved courses.
  - **Cart/Checkout**: Complete purchases.
  - **Course Content**: Access videos and related materials.
  - **User Profile**: View and edit user information.
- **For Instructors**:
  - **Dashboard**: Overview of courses, ratings, and feedback.
  - **Insights**: Detailed metrics on course views and engagements.
  - **Course Management**: Create, update, and delete courses.
  - **Profile Management**: Edit account details.

**Frameworks and Libraries Used**:  
- **ReactJS**
- **Redux**: State management.
- **CSS/Tailwind**: For styling and responsive design.

---

## Back-end
The back-end application leverages **NodeJS** and **ExpressJS**, with **MongoDB** for data storage.

### Key Features
- **User Authentication**: Supports email/password login, OTP verification, and password recovery.
- **Course Management**: Instructors can create, read, update, and delete courses.
- **Payment Integration**: Secure course purchase through Razorpay.
- **Cloud-based Media Management**: Cloudinary for storing images, videos, and documents.
- **Markdown Support**: Allows document formatting for easy display on the front end.

### Frameworks, Libraries, and Tools
- **Node.js**
- **Express.js**
- **JWT**: JSON Web Tokens for authentication.
- **Bcrypt**: For password hashing.
- **Mongoose**: MongoDB ODM for schema management.

### Data Models
1. **Student**: Details on name, email, password, enrolled courses.
2. **Instructor**: Details on name, email, password, managed courses.
3. **Course**: Details on title, description, instructor, media content, etc.

---

## API Design
The platform's **RESTful API** supports the following endpoints:

- **Authentication**:
  - `/api/auth/signup` (POST) - Register a new user.
  - `/api/auth/login` (POST) - Log in and receive a JWT token.
  - `/api/auth/verify-otp` (POST) - Verify OTP for login.
  - `/api/auth/forgot-password` (POST) - Request a password reset.

- **Course Management**:
  - `/api/courses` (GET) - List all courses.
  - `/api/courses/:id` (GET) - View a course by ID.
  - `/api/courses` (POST) - Create a new course.
  - `/api/courses/:id` (PUT) - Update a course.
  - `/api/courses/:id` (DELETE) - Delete a course.
  - `/api/courses/:id/rate` (POST) - Add a rating (out of 5) to a course.
  - `/api/courses` (GET) - Get all courses.
  - `/api/courses/:id` (GET) - Get a single course by ID.


---

## Deployment
The application is deployed on Vercel for frontend & Render for Backend, with configurations for scalability and continuous integration. Deployment scripts are available in this repository to facilitate deployment.

---

## Testing
StudyNotion uses automated testing to ensure robust functionality:
- **Types of Tests**: Unit, integration, and end-to-end.
- **Test Frameworks**: Mocha, Chai, Jest (update as needed based on actual tools used).

---

## Future Enhancements
Possible improvements include:
1. **Social Media Integration**: To enable students to share achievements.
2. **AI-based Course Recommendations**: Personalized content suggestions for each user.
3. **Enhanced Instructor Analytics**: Real-time data on course engagement.

---

## Getting Started

### Prerequisites
- **Node.js**
- **MongoDB**
- **Razorpay Account**

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/anshika-maurya/studynotion.git
   ```
2. **Install dependencies**:
   ```bash
   cd studynotion
   npm install
   ```

3. **Run the Application**:
   ```bash
   npm start
   ```


---

## License
Distributed under the MIT License. See `LICENSE` for more information.

---
