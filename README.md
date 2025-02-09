## Demo video link of the project 
https://drive.google.com/file/d/1PnkgLrqQ5byodFsrKGMN_r9o3aqPOdvK/view

**Screenshots** 
1. Home Page: ![image](https://github.com/user-attachments/assets/793a16ec-ae20-43ab-bbcd-4e0989584445)

2. Login Page:![image](https://github.com/user-attachments/assets/1b7274d8-584e-49e6-9e25-731fac23b7d6)

3. Register page :![image](https://github.com/user-attachments/assets/02a9b238-cd29-4dc0-baf7-b2c8cafbfc8b)

4. Admin Dashboard:![image](https://github.com/user-attachments/assets/0c2a16e0-f5ae-4d2c-8eff-a6606cd81b15)

5. manager Dashboard :![image](https://github.com/user-attachments/assets/30cc80c9-f004-40a7-8b92-a2a95b88692b)

6. staff Dashboard :![image](https://github.com/user-attachments/assets/75b3ade0-7220-49bc-b67b-f9844c1518b2)

   
# Employee Management System using Spring Security

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
## Key Configuration
**application.properties:**
 ```bash
properties
 
server.port=8082
spring.jpa.hibernate.ddl-auto=update
spring.jpa.show-sql=true
spring.thymeleaf.cache=false
management.endpoints.web.exposure.include=health,info
 ```
## Contributing
Contributions are welcome! Please open an issue or submit a pull request for any improvements.

## License
This project is licensed under the MIT License - see the LICENSE file for details.







