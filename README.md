# MakerSharks
Makersharks is building a search page where buyers can search for manufacturers based on their customized requirements. We're building a proof of concept for the search API.

# Makersharks Search API

## Overview

This project is a proof of concept (POC) for the Makersharks search API. The API allows buyers to search for manufacturers based on customized requirements such as location, nature of business, and manufacturing processes.

## Features

- Retrieve manufacturers based on location, nature of business, and manufacturing processes.
- Pagination support for large result sets.
- Input validation and sanitization.
- Basic exception handling.
- Basic security configuration using Spring Security.
- API documentation using Swagger.

## Technologies Used

- Java 17
- Spring Boot 3.x
- Spring Data JPA
- H2 Database
- Maven
- Swagger (Springdoc OpenAPI)
- Spring Security
- Lombok

## Setup and Running the Application

### Prerequisites

- JDK 17 or higher installed
- Maven installed and configured in your PATH
- An IDE like IntelliJ IDEA, Eclipse, or VS Code

### Cloning the Repository

## Installation

Clone the Repository:
```bash
  https://github.com/Aadarshprajapati777/Makersharks
  cd Makersharks

```
Build and Run the Application:
```bash
 mvn spring-boot:run                     
```

Access Swagger Documentation:
```bash
http://localhost:8080/swagger-ui.html
```
## Testing
```bash
./mvnw test
```


## Configuration

```bash
cd src/main/resources/application.properties
Setup postgres Configuration
```
Replace the Postgres Configuration with your own or mail to get the password.


Accessing the API
Once the application is running, the API will be available at http://localhost:8080.

API Endpoints
1. Query Manufacturers
Endpoint: /api/supplier/query
Method: POST
Description: Retrieve a list of manufacturers based on location, nature of business, and manufacturing processes.

Request Parameters:

location: The location of the manufacturer (e.g., India).
natureOfBusiness: The nature of the business (e.g., small_scale).
manufacturingProcesses: The manufacturing processes the manufacturer can perform (e.g., 3d_printing).
Example Request:


```bash
curl -X 'POST' \
  'http://localhost:8080/api/v1/supplier/create' \
  -H 'accept: */*' \
  -H 'Content-Type: application/json' \
  -d '{
  "company_name": "Example Co.",
  "website": "example.com",
  "location": "India",
  "nature_of_business": "small_scale",
  "manufacturing_processes": "3d_printing"
}'
```

Accessing Swagger Documentation
The API documentation can be accessed at http://localhost:8080/swagger-ui.html or http://localhost:8080/swagger-ui/index.html after starting the application.

Running Tests
You can run the unit tests using Maven:

```bash
mvn test
```

Security
The application uses basic authentication for simplicity. For production, consider using OAuth2 or JWT tokens for more secure authentication and authorization mechanisms.

Troubleshooting
If you encounter issues with the mvn command not being recognized, ensure Maven is properly installed and added to your system's PATH.

Contributing
If you'd like to contribute to this project, please fork the repository and create a pull request. We welcome all contributions!


Contact Information:

For any queries or support, please contact your-official.varad20@gmail.com.


### Instructions:
- Replace `https://github.com/your-username/makersharks-search-api.git` with the actual GitHub repository URL.
- Customize the contact information, project name, and any specific details relevant to your project.
- Ensure you test the curl command and the Swagger URL to confirm they work as expected before
