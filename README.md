# HR Management System

A web-based **HR Management System** designed to manage employees, vacations, meeting rooms, equipment, bookings, and attachments.

The project is built using **Spring Boot, JHipster, Angular, Spring Security, JWT, and MySQL/JPA technologies**.

---

## 🚀 Features

* 👤 Employee Management
* 🏢 Department and Role Management
* 🏖️ Vacation Request Management
* 🏢 Meeting Room Management
* 💻 Equipment Management
* 📅 Meeting Room Booking
* 👥 Employee Invitations
* 📎 File Attachments
* 🔐 Secure Authentication and Authorization
* 🛡️ Role-Based Access Control
* 📊 RESTful APIs
* 📖 OpenAPI / Swagger Documentation
* 🐳 Docker Support
* ⚡ Spring Boot Actuator

---

## 🔐 Security

Security is implemented using **Spring Security and JWT-based authentication**.

### Technologies Used

* **Spring Security**

  * Authentication
  * Authorization
  * Securing REST APIs
  * Role-based access control

* **JWT (JSON Web Token)**

  * Secure authentication tokens
  * Stateless authentication
  * Token-based API access

* **Role-Based Access Control (RBAC)**

  * Controls access depending on the user's role
  * Protects restricted HR operations and resources

### Authentication Flow

```text
User
  ↓
Angular Frontend
  ↓
Login
  ↓
Spring Boot Backend
  ↓
Authentication
  ↓
JWT Token
  ↓
Angular Stores Token
  ↓
Authenticated API Requests
  ↓
Spring Security
  ↓
Access Granted / Denied
```

Protected API requests use the JWT token for authentication.

```http
Authorization: Bearer <JWT_TOKEN>
```

---

## 🏗️ Backend

The backend is built using:

* Java 17
* Spring Boot
* JHipster
* Spring Security
* JWT
* Spring Data JPA
* Hibernate
* REST APIs
* Bean Validation
* Maven
* Spring Boot Actuator
* Undertow

---

## 🎨 Frontend

The frontend is built using:

* Angular
* TypeScript
* HTML5
* CSS3
* Webpack
* npm
* JHipster

---

## 🗄️ Database

The application uses **JPA/Hibernate** for database persistence.

### Main Entities

* Employee
* Meeting Room
* Equipment
* Booking Request
* Vacation Request
* Attachment
* User

### Main Relationships

```text
Employee
 ├── Booking Requests
 ├── Vacation Requests
 └── User

Meeting Room
 ├── Booking Requests
 └── Equipment

Vacation Request
 └── Attachments

Booking Request
 └── Invited Employees
```

---

## 📅 Main Modules

### Employee Management

Manage employee information including:

* Name
* Email
* Role
* Vacation Balance
* Account information

### Vacation Management

Employees can create vacation requests with:

* Start Date
* End Date
* Vacation Type
* Reason
* Status

Supported vacation types:

* Annual
* Sick

Request statuses:

* Pending
* Approved
* Rejected

### Meeting Room Management

Manage meeting rooms including:

* Room Name
* Capacity
* Approval Requirement
* Room Equipment

### Equipment Management

Manage company equipment including:

* Name
* Description
* Availability

### Booking Management

Employees can create meeting room booking requests with:

* Start Time
* End Time
* Purpose
* Status
* Invited Employees

### Attachments

Vacation requests can contain uploaded files and attachments.

---

## 🌐 REST API

The backend provides RESTful APIs for managing the system resources.

Main API areas include:

```text
Employees
Users
Vacation Requests
Meeting Rooms
Equipment
Booking Requests
Attachments
```

API documentation is available through **OpenAPI / Swagger**.

---

## 🐳 Docker

The project supports Docker for easier deployment and environment setup.

Docker can be used to containerize the application and run it consistently across different environments.

---

## 📂 Project Structure

```text
hr-management-system/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   └── webapp/
│   │
│   └── test/
│
├── webpack/
├── .jhipster/
├── .mvn/
├── .husky/
│
├── Docker configuration
├── pom.xml
├── package.json
├── model.jdl
└── README.md
```

---

## 🛠️ Complete Technology Stack

| Category          | Technologies               |
| ----------------- | -------------------------- |
| Backend           | Java 17, Spring Boot       |
| Framework         | JHipster                   |
| Security          | Spring Security, JWT       |
| ORM               | Hibernate, Spring Data JPA |
| API               | RESTful APIs               |
| API Documentation | OpenAPI / Swagger          |
| Validation        | Jakarta Bean Validation    |
| Frontend          | Angular, TypeScript        |
| UI                | HTML5, CSS3                |
| Build Tools       | Maven, npm, Webpack        |
| Server            | Undertow                   |
| Monitoring        | Spring Boot Actuator       |
| DevOps            | Docker                     |

---

## ▶️ How to Run

### 1. Clone the repository

```bash
git clone https://github.com/OmarAbdelmonem1/hr-management-system.git
cd hr-management-system
```

### 2. Run the Backend

```bash
./mvnw
```

On Windows:

```bash
mvnw.cmd
```

### 3. Run the Frontend

```bash
./npmw start
```

The application will be available at:

```text
http://localhost:8080
```

---

## 📦 Production Build

To create a production build:

```bash
./mvnw -Pprod clean verify
```

---

## 🎯 Project Goal

The goal of this project is to provide a complete **Human Resources Management System** that simplifies employee management and automates common HR operations such as vacation requests, meeting room bookings, equipment management, and employee invitations.

The system combines a modern **Angular frontend** with a secure **Spring Boot backend** and **JWT-based authentication** to provide a scalable and maintainable HR platform.
