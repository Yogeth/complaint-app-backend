# Complaint Tracker Backend

Backend API for the Complaint Tracker application built with Spring Boot, Spring Data JPA, and MariaDB.

## Features

- Create complaints
- View all complaints
- Update complaint status
- Delete complaints
- RESTful API architecture
- Database persistence using JPA/Hibernate

## Tech Stack

- Java 21
- Spring Boot
- Spring Data JPA
- Hibernate
- MariaDB
- Maven

## Prerequisites

Before running the project, make sure you have:

- Java 21+
- Maven
- MariaDB/MySQL
- Git

## Installation

### 1. Clone the Repository

```bash
git clone https://github.com/yogeth/complaint-tracker-backend.git
cd complaint-tracker-backend
```

### 2. Create Database

Login to MariaDB/MySQL:

```sql
CREATE DATABASE complaint_tracker;
```

### 3. Configure Database

Update `application.properties`:

```properties
spring.datasource.url=jdbc:mariadb://localhost:3306/complaint_tracker
spring.datasource.username=root
spring.datasource.password=your_password

spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
```

### 4. Install Dependencies

```bash
mvn clean install
```

### 5. Run the Application

```bash
mvn spring-boot:run
```

The server will start on:

```text
http://localhost:8080
```

## API Endpoints

| Method | Endpoint | Description |
|----------|----------|-------------|
| GET | /complaints | Get all complaints |
| POST | /complaints | Create complaint |
| PUT | /complaints/{id} | Update complaint |
| DELETE | /complaints/{id} | Delete complaint |

## Project Structure

```text
src
├── main
│   ├── java
│   │   ├── controller
│   │   ├── model
│   │   ├── repository
│   │   └── service
│   └── resources
│       └── application.properties
```

## Frontend Repository

The frontend application is deployed separately.

Frontend:
[https://your-frontend-url.vercel.app](https://complaint-app-lovat.vercel.app/]


## Future Improvements

- Authentication & Authorization
- Admin Dashboard
- Email Notifications
- Complaint Categories
- File Attachments
- Complaint Analytics

## Author

Yogeth

Built as a full-stack complaint management system using Spring Boot and React.
