# 👥 HR Management System

A web-based **Human Resources Management System** built with **Java, Spring Boot, JHipster, and Angular/TypeScript**.

The system helps organizations manage employees, vacation requests, meeting rooms, equipment, and booking requests.

## 🚀 Main Features

* Employee Management
* User Management
* Employee Roles
* Vacation Requests
* Vacation Approval / Rejection
* Meeting Room Management
* Equipment Management
* Meeting Room Booking
* Booking Requests
* Booking Approval / Rejection
* File Attachments
* User Authentication & Authorization
* REST APIs
* API Documentation

## 🔐 Security

The application uses **Spring Security** and **OAuth2 Resource Server** to secure the application and its APIs.

Main security technologies:

* Spring Security
* OAuth2
* Authentication & Authorization
* Role-Based Access Control
* Secure REST APIs

## 🏗️ Backend

The backend is built with:

* Java
* Spring Boot
* JHipster
* Spring Data JPA
* Hibernate
* Spring Security
* REST APIs
* Spring Validation
* Spring Boot Actuator

## 💻 Frontend

The frontend uses:

* TypeScript
* Angular
* HTML
* CSS
* Webpack

## 🗄️ Main Entities

```text
Employee
   │
   ├── Booking Requests
   │
   └── Vacation Requests
           │
           └── Attachments

Meeting Room
   │
   ├── Equipment
   │
   └── Booking Requests

User
   │
   └── Employee
```

Main entities include:

* Employee
* MeetingRoom
* Equipment
* BookingRequest
* VacationRequest
* Attachment
* User

## 🛠️ Technologies

### Backend

* Java
* Spring Boot
* JHipster
* Spring Data JPA
* Hibernate
* Spring Security
* OAuth2
* REST API
* Maven

### Frontend

* Angular
* TypeScript
* HTML
* CSS
* Webpack

### Development Tools

* Docker
* JUnit
* Jest
* Sonar
* OpenAPI / Swagger

## 📁 Project Structure

```text
hr-management-system/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   ├── resources/
│   │   └── webapp/
│   │
│   └── test/
│
├── webpack/
├── .jhipster/
├── pom.xml
├── package.json
├── model.jdl
└── README.md
```

## ▶️ How to Run

### Backend

```bash
./mvnw
```

### Frontend

In another terminal:

```bash
./npmw start
```

Then open:

```text
http://localhost:8080
```

The project also provides Maven and npm wrappers, so the project dependencies can be managed without relying on globally installed Maven/npm versions.

## 🧪 Testing

Run backend tests:

```bash
./mvnw verify
```

Run frontend tests:

```bash
./npmw test
```

## 📚 API Documentation

The project includes **OpenAPI support** for documenting the REST APIs.

## 🎯 Project Goal

The goal of this project is to provide a simple and secure HR platform for managing employees, vacations, meeting rooms, equipment, and internal booking requests.
