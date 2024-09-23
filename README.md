# Contact Manager Application
[Try it here!](https://enriqueferrermelian.github.io/contact-manager/)

[![Try it here!](https://github.com/user-attachments/assets/d78e25c5-923c-48d3-8636-96a509fd0eeb)](https://enriqueferrermelian.github.io/contact-manager/)


## Description

A full-stack Contact Manager application that allows users to create, view, update, and delete contacts. The backend is built with Spring Boot and H2 database, while the frontend is created with React.

## Features

- Add new contacts (name, email, phone)
- View a list of existing contacts
- Delete contacts
- Data stored in an H2 in-memory database
- Simple user interface with React

## Table of Contents

- [Technologies](#features)
- [Prerequisites](#technologies-used)
- [Installation](#installation)
- [Running the Backend](#available-scripts)
- [Running the Frontend](#contribution)
- [API Endpoints](#license)
- [Usage](#contact)
- [Screenshots](#screenshots)
- [License](#licese)

## Demo
- Backend runs locally on localhost:8080
- 
## Technologies

- Backend: Java, Spring Boot, H2 Database
- Frontend: React, Axios, CSS
- Tools: Maven, IntelliJ, VSCode, Postman

## Prerequisites
- Java (version 11 or higher)
- Node.js and npm (for running React)
- Maven (for building the Spring Boot backend)
- A tool like Postman (optional, for testing APIs)

## Installation

To clone and run this project, follow these steps:

1. Clone the repository:

   ```bash
   git clone https://github.com/EnriqueFerrerMelian/contact-manager
   cd contact-manager

2. Directory Structure:
   The project is divided into two parts:
   - src/ (Spring Boot project)
   - frontend/ (React project)


## Running the Backend
- Navigate to the backend directory:
   ```bash 
   ./mvnw spring-boot:run
  
- Run the Spring Boot application:
  * You can use Maven from the terminal:
    ```bash
    ./mvnw spring-boot:run
- Alternatively, you can run it directly in an IDE like IntelliJ by executing the ContactManagerApplication.java file.

4. H2 Database:
- The H2 database is an in-memory database and will be initialized automatically when the application starts. You can access the H2 console in your browser at:
   ```bash
   http://localhost:8080/h2-console
- Default credentials:
  - JDBC URL: jdbc:h2:mem:testdb
  - Username: sa
  - Password: password

## Running the Frontend
- Navigate to the frontend directory:
   ```bash
   cd frontend
- Install dependencies:
   ```bash
   npm install
- Start the React app:
   ```bash
   npm start
- This will start the development server, and you can view the app in your browser at:
   ```bash
   http://localhost:3000

## API Endpoints
- GET /api/contacts - Get a list of all contacts
- POST /api/contacts - Add a new contact
- PUT /api/contacts/{id} - Update an existing contact
- DELETE /api/contacts/{id} - Delete a contact

Example API Calls

Using Postman or another tool, you can make requests to these endpoints. Ensure the backend is running on http://localhost:8080.
   - Get all contacts:
   - GET http://localhost:8080/api/contacts

   - Add a contact:
     - POST http://localhost:8080/api/contacts
     {
     "name": "John Doe",
     "email": "johndoe@example.com",
     "phone": "123-456-7890"
     }

## Usage

Once both the backend and frontend are running, you can:
- View the contact list in the UI.
- Add, edit, or delete contacts using the React interface.
- The changes will be reflected in the H2 database (which is temporary and resets each time the backend restarts).

## Screenshots
- Add screenshots

## License

This project is licensed under the MIT License.

## Additional Notes
- The H2 database is in-memory and will reset upon server restart. If you want to use a persistent database, consider configuring MySQL or PostgreSQL in the application.properties.
- Feel free to fork this project and modify it according to your needs.

## Contact

If you have any questions or comments, feel free to reach out at progranauta@gmail.com

Thank you for visiting the To-Do List App repository! If you encounter any issues, please open an issue.
