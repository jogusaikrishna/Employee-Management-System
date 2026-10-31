 
# Employee Management System

## Project Overview

The **Employee Management System** is a backend application developed using Java and Spring Boot to manage employee information efficiently.

It provides RESTful APIs to perform CRUD operations (Create, Read, Update, Delete) on employee records. The application uses Spring Data JPA and Hibernate for database operations and MySQL for data storage.

## Technologies Used

- **Programming Language:** Java 25
- **Backend Framework:** Spring Boot
- **ORM Framework:** Hibernate
- **Data Access:** Spring Data JPA
- **Database:** MySQL 8
- **Build Tool:** Maven
- **API Testing:** Postman
- **IDE:** IntelliJ IDEA
- **Version Control:** Git & GitHub

## Features

- Add new employee records.
- Retrieve all employee details.
- Retrieve employee details by ID.
- Update existing employee information.
- Delete employee records.
- Input validation using `@Valid`.
- Global exception handling.
- Pagination using Spring Data JPA.
- Sorting employee records by different fields.
- RESTful API architecture.

## Project Architecture

The project follows a layered architecture:

```text
Employee Management System
          |
          v
     Controller
          |
          v
       Service
          |
          v
     Repository
          |
          v
      Database
        MySQL
```

- **Controller:** Handles incoming HTTP requests.
- **Service:** Contains business logic.
- **Repository:** Communicates with the database.
- **Entity:** Represents employee data.

## Database Configuration

Database Name: `employee_db`

Table Name: `employee`

Employee fields:

| Field | Description |
|---|---|
| id | Employee ID |
| name | Employee Name |
| email | Employee Email |
| department | Employee Department |
| salary | Employee Salary |

## REST API Endpoints

Base URL: `http://localhost:8080`

| HTTP Method | Endpoint | Description |
|---|---|---|
| POST | `/api/employees` | Add employee |
| GET | `/api/employees` | Get all employees |
| GET | `/api/employees/{id}` | Get employee by ID |
| PUT | `/api/employees/{id}` | Update employee |
| DELETE | `/api/employees/{id}` | Delete employee |
| GET | `/api/employees/page?page=0&size=3` | Pagination |
| GET | `/api/employees/sort?field=name&direction=asc` | Sorting |

## Sample JSON Request

```json
{
  "name": "Sai Krishna",
  "email": "saikrishna@gmail.com",
  "department": "Java Developer",
  "salary": 50000
}
```

## How to Run the Project

1. Clone the repository:

```bash
git clone YOUR_GITHUB_REPOSITORY_URL
```

2. Open the project in IntelliJ IDEA.

3. Configure MySQL and create the database:

```sql
CREATE DATABASE employee_db;
```

4. Configure your database username and password in `application.properties`.

5. Run the Spring Boot application.

6. Open Postman and test the REST API endpoints.

## Learning Outcomes

- Understanding Spring Boot application development.
- Implementing RESTful web services.
- Performing CRUD operations using Spring Data JPA.
- Connecting Java applications with MySQL.
- Understanding layered architecture.
- Testing APIs using Postman.
- Implementing pagination, sorting and exception handling.

## Author

**Jogu Sai Krishna**

Java Developer | Spring Boot | MySQL
