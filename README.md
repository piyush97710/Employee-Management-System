# Employee Management System

A simple Employee Management System developed using Java, Spring Boot, REST API, Spring Data JPA and MySQL.

## Technologies Used

* Java
* Spring Boot
* Spring Web
* Spring Data JPA
* MySQL
* Maven
* REST API
* Thunder Client

## Features

* Add a new employee
* View all employees
* View employee by ID
* Update employee details
* Delete employee
* Search employees by department

## Project Structure

The project follows a layered architecture:

* **Controller** - Handles REST API requests
* **Service** - Contains business logic
* **Repository** - Handles database operations
* **Entity** - Represents employee data

## API Endpoints

| Method | Endpoint                                 | Description                    |
| ------ | ---------------------------------------- | ------------------------------ |
| POST   | `/api/employees`                         | Add a new employee             |
| GET    | `/api/employees`                         | Get all employees              |
| GET    | `/api/employees/{id}`                    | Get employee by ID             |
| PUT    | `/api/employees/{id}`                    | Update employee                |
| DELETE | `/api/employees/{id}`                    | Delete employee                |
| GET    | `/api/employees/department/{department}` | Search employees by department |

## Database

The application uses MySQL for storing employee information.

Database name:

```text
employee_db
```

Hibernate/JPA is used to create and update the required database table automatically.

## Example API Request

### Add Employee

**POST**

```text
/api/employees
```

Request body:

```json
{
    "name": "Rahul Kumar",
    "email": "rahul@gmail.com",
    "department": "IT",
    "salary": 60000
}
```

## How to Run the Project

### 1. Clone the repository

```bash
git clone https://github.com/piyush97710/Employee-Management-System.git
```

### 2. Create the MySQL database

```sql
CREATE DATABASE employee_db;
```

### 3. Configure MySQL

Update the MySQL username and password in:

```text
src/main/resources/application.properties
```

### 4. Run the application

For Windows:

```bash
mvnw.cmd spring-boot:run
```

For Linux/Mac:

```bash
./mvnw spring-boot:run
```

The application will run at:

```text
http://localhost:8080
```

## Testing

The REST APIs were tested using Thunder Client.

## Author

**Piyush Kumar**

B.Tech Computer Science and Engineering
