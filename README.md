# Demo video link of the project 
https://drive.google.com/file/d/1PnkgLrqQ5byodFsrKGMN_r9o3aqPOdvK/view

# Employee Management System

A Spring Boot-based web application for managing employees with role-based access control (ADMIN, MANAGER, STAFF).

## Features

- User registration and authentication
- Role-based access control:
  - ADMIN: Full CRUD operations on employees
  - MANAGER: Create and Update employees
  - STAFF: View employee list
- MySQL database integration
- Thymeleaf templating for UI
- Spring Security implementation
- Responsive UI with Bootstrap

## Technologies Used

- **Backend**:
  - Spring Boot 3.2.4
  - Spring Security
  - Spring Data JPA
- **Frontend**:
  - Thymeleaf
  - Bootstrap 5
  - Font Awesome
- **Database**:
  - MySQL
- **Build Tool**:
  - Maven

## Prerequisites

- Java 17
- MySQL Server
- Maven

## Installation & Setup

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-username/TejUserApplication.git


## Database Setup:

- Create a MySQL database named tej_db

- Update database credentials in src/main/resources/application.properties:

**properties**
 ```bash
 spring.datasource.url=jdbc:mysql://localhost:3306/tej_db
 spring.datasource.username=your-username
 spring.datasource.password=your-password
  ```
Build and Run:

 ```bash
mvn clean install
mvn spring-boot:run
 ```
- Access the application at: http://localhost:8082
# Usage
## Registration:

- Navigate to /register

- Fill in user details (role field must be either "ADMIN", "MANAGER", or "STAFF")

## Login:

- Use registered email and password at /signin

## Role-based Access:

- **ADMIN:** Full access to create, read, update, and delete employees

- **MANAGER:** Can create and update employees

- **STAFF:** Read-only access to employee list

## Project Structure
 ```bash
src/main/java
├── com.springboot.project.TejUserApplication
│   ├── config          # Security configurations
│   ├── controller      # MVC Controllers
│   ├── entity          # JPA Entities
│   ├── repository      # Spring Data JPA Repositories
│   ├── service         # Business logic implementations
│   └── TejUserApplication.java # Main application class

src/main/resources
├── static              # CSS, JS, images
├── templates           # Thymeleaf templates
└── application.properties # Configuration
 ```
Key Configuration
application.properties:

properties
Copy
server.port=8082
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.thymeleaf.cache=false
management.endpoints.web.exposure.include=health,info
Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Copy

**Screenshots** (You can add these as images in your repository):

1. Login Page:
![Login Page](screenshots/login.png)

2. Admin Dashboard:
![Admin Dashboard](screenshots/admin-dashboard.png)

3. Employee Management:
![Employee Management](screenshots/employee-management.png)

Note: You should create a `screenshots` directory in your repository and add actual screenshots from your application.

This README provides:
- Clear project description
- Installation instructions
- Usage guide
- Technology stack overview
- Project structure explanation
- Contribution guidelines
- License information

Make sure to:
1. Replace `your-username` in the clone command with your actual GitHub username
2. Add actual screenshots to the repository
3. Create a LICENSE file if needed
4. Update the database credentials in the README to match your local setup
