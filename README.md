# 🚗 RideX — Real-Time Ride Booking & Management Platform

RideX is a full-stack ride-booking and management platform inspired by modern ride-hailing applications. It provides separate experiences for **Users** and **Captains (Drivers)**, allowing users to request rides while captains can receive, accept, manage, and complete rides in real time.

The project is built using the **MERN stack** with **Socket.IO** for real-time communication and a RESTful backend architecture.

----

## 🌐 Overview

RideX is designed to simulate a real-world ride-hailing ecosystem where users can:

- Register and log in securely
- Search for pickup and destination locations
- Request rides
- Select suitable vehicle types
- Track ride status
- Communicate with the backend in real time

Captains can:

- Register and log in
- Configure vehicle details
- Receive ride requests
- Accept or reject rides
- Manage active rides
- Update ride status
- Complete rides

The application follows a client-server architecture with a React frontend communicating with a Node.js/Express backend and MongoDB database.

---

## ✨ Features

### 👤 User Features

- User registration and login
- Secure authentication using JWT
- Protected user routes
- Pickup and destination selection
- Vehicle selection
- Ride request functionality
- Ride confirmation flow
- Real-time ride status updates
- Live ride tracking
- User logout

### 🚕 Captain Features

- Captain registration and login
- Vehicle information management
- Vehicle type selection
- Protected captain routes
- Real-time ride request notifications
- Accept/reject ride requests
- Active ride management
- Ride completion flow
- Captain logout

### ⚡ Real-Time Communication

- Real-time client-server communication using Socket.IO
- Captain connection management
- Real-time ride request updates
- Ride status synchronization
- Event-driven communication between users and captains

### 🔐 Authentication & Authorization

- JWT-based authentication
- Protected routes using authentication middleware
- Separate authentication flows for Users and Captains
- Secure logout functionality
- Backend request validation using Express Validator

### 🗺️ Location & Ride Management

- Pickup and destination handling
- Location search
- Map-based ride interaction
- Ride distance and fare-related services
- Real-time ride tracking architecture

---

## 🛠️ Tech Stack

### Frontend

- React.js
- Vite
- Tailwind CSS
- Axios
- React Router
- Socket.IO Client

### Backend

- Node.js
- Express.js
- MongoDB
- Mongoose
- JWT
- bcrypt
- Express Validator
- Socket.IO
- Axios

### Development Tools

- Git
- GitHub
- VS Code
- npm
- Postman

---

## 🏗️ Architecture

```text
                    ┌─────────────────────┐
                    │       User          │
                    │   React Frontend    │
                    └──────────┬──────────┘
                               │
                               │ HTTP / Axios
                               │
                               ▼
                    ┌─────────────────────┐
                    │    Express Server   │
                    │      REST APIs      │
                    └──────────┬──────────┘
                               │
                ┌──────────────┼──────────────┐
                │              │              │
                ▼              ▼              ▼
          ┌──────────┐   ┌──────────┐   ┌──────────┐
          │ MongoDB  │   │ Socket.IO│   │ Services │
          └──────────┘   └─────┬────┘   └──────────┘
                               │
                               │ Real-Time Events
                               ▼
                    ┌─────────────────────┐
                    │      Captain        │
                    │   React Frontend    │
                    └─────────────────────┘

---

## 🧪 API Endpoints

### 👤 User APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/users/register` | Register a new user |
| `POST` | `/users/login` | Authenticate user |
| `GET` | `/users/profile` | Get authenticated user profile |
| `GET` | `/users/logout` | Logout user |

### 🚕 Captain APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/captains/register` | Register a captain |
| `POST` | `/captains/login` | Authenticate captain |
| `GET` | `/captains/profile` | Get authenticated captain profile |
| `GET` | `/captains/logout` | Logout captain |

### 🚗 Ride APIs

| Method | Endpoint | Description |
|--------|----------|-------------|
| `POST` | `/rides/create` | Create a ride request |
| `GET` | `/rides/get-fare` | Calculate ride fare |
| `POST` | `/rides/confirm` | Confirm a ride |
| `POST` | `/rides/start-ride` | Start a ride |
| `POST` | `/rides/end-ride` | Complete a ride |

> **Note:** Endpoint names may vary depending on the current backend implementation.

---

## 📚 What I Learned

Building RideX provided hands-on experience with:

- MERN stack application development
- REST API design
- React component architecture
- React Router
- Context API
- JWT authentication
- Password hashing
- MongoDB and Mongoose
- Express middleware
- Request validation
- Socket.IO
- Real-time client-server communication
- API integration
- Environment variable management
- Git and GitHub workflows
- Full-stack debugging

---

## 📄 License

This project is created for educational and portfolio purposes.

---

## 👩‍💻 Author

### Shreyal Gupta

**B.Tech — Computer Science & Engineering**

**GitHub:**  
https://github.com/ShreyalGupta701

**LinkedIn:**  
https://www.linkedin.com/in/shreyal-gupta-178500301

---

⭐ If you found this project useful or interesting, consider giving the repository a star!
