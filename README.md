## Demo video link of the project 
https://drive.google.com/file/d/1PnkgLrqQ5byodFsrKGMN_r9o3aqPOdvK/view

**Screenshots** 
1. Home Page: [screenshots/Home page.png](https://github.com/maruthicharanteja10/Employee-Login-Register-alongwith-differentAuthtication-roles-UsingSpringboot/blob/48477273db632e2416d953dc45e6cfc9b0f0f508/screenshots/Home%20page.png)
2. Login Page:  [screenshot/loginpage](https://github.com/maruthicharanteja10/Employee-Login-Register-alongwith-differentAuthtication-roles-UsingSpringboot/blob/2170bb978a6e5ac01bc45156b3c20e0524c90628/screenshots/loginpage.png)
3. Register page : [screenshots/register page.png](https://github.com/maruthicharanteja10/Employee-Login-Register-alongwith-differentAuthtication-roles-UsingSpringboot/blob/7297f3f6e1468add09cad8678e60e8fb69cffdb5/screenshots/register%20page.png)
4. Admin Dashboard: [screenshots/Admin Dashboard.png](https://github.com/maruthicharanteja10/Employee-Login-Register-alongwith-differentAuthtication-roles-UsingSpringboot/blob/d2425e4d498213a764563611ef9eada3fa3a23a7/screenshots/Admin%20Dashboard.png)
5. manager Dashboard : [screenshots/Manager Dashboard.png](https://github.com/maruthicharanteja10/Employee-Login-Register-alongwith-differentAuthtication-roles-UsingSpringboot/blob/d4622354e69a839d122955e2526e4c55db7811e0/screenshots/Manager%20Dashboard.png)
6. staff Dashboard : [screenshots/staff dashboard.png](https://github.com/maruthicharanteja10/Employee-Login-Register-alongwith-differentAuthtication-roles-UsingSpringboot/blob/70df98d2f00bdd48b5cdb08ae003a6e29fba0204/screenshots/staff%20Dashboard.png)
   
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







