# Car Showroom Management Application

## Project Overview

This web application manages car showrooms and their associated cars, built using Java, Spring Boot for the backend, and Angular for the frontend. The application provides APIs for CRUD operations on car showrooms and cars, complete with pagination, sorting, and data validation.

## Table of Contents

1. [General Requirements](#general-requirements)
2. [Backend Requirements](#backend-requirements)
3. [Technologies Used](#technologies-used)
4. [Testing](#testing)

## General Requirements

- **Documentation**: Include this README file explaining the project structure, setup instructions, and any assumptions made.
- **Code Quality**: Ensure clean, readable code that follows best practices. Include comments where necessary and ensure modularity.
- **Error Handling**: Proper error responses with appropriate HTTP status codes.
- **Git Usage**: Version control should be managed using Git. Include commits with meaningful messages to show your approach.

## Backend Requirements

The backend is built using the latest stable version of Java and Spring Boot with Spring Data JPA for data management.

### API Requirements:

1. **Create Car Showroom API**: Allows creating a new showroom.
   - Inputs: `name`, `commercial_registration_number`, `manager_name`, `contact_number`, `address`.
   - Validations: All fields adhere to their constraints before saving.

2. **List Car Showrooms API**: Lists all existing car showrooms with pagination and sorting.
   - Response: Specific fields - `name`, `commercial_registration_number`, `contact_number`.

3. **Get Specific Car Showroom API**: Retrieves all details of a showroom.

4. **Update Car Showroom API**: Updates specific fields of a showroom.

5. **Delete Car Showroom API**: Performs a soft delete.

6. **Create new Car in Car Showroom API**: Allows adding a new car associated with a showroom.

7. **List Cars with Showroom Details API**: Lists cars with pagination and dynamic filtering.

### Additional Guidelines:

- **Exception Handling**: Implemented throughout the application.
- **Authentication & Authorization**: Utilizes Spring Security for securing endpoints (optional but considered a plus).
- **Caching**: Implemented to enhance performance by storing frequently accessed data.
- **Database Version Control**: Managed using Flyway or Liquibase.

## Technologies Used

- Java
- Spring Boot
- Spring Data JPA
- Spring Security
- Caching (Spring Cache)
- Maven
- SQL Server

## Testing
The application includes comprehensive unit tests to ensure the functionality of the backend APIs and the overall integrity of the application. Unit tests are created using the JUnit framework. Each API endpoint is tested for various scenarios, including:

- Valid and invalid input data
- Successful responses for valid requests
- Appropriate error handling and HTTP status codes for invalid requests
- Edge cases, such as empty fields or non-existent resources




