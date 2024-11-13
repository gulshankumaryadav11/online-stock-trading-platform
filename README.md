Online Stock Trading Platform
Overview
This is a simplified online stock trading platform built using Spring Boot. The platform allows users to register, view available stocks, and place buy or sell orders. It uses an in-memory H2 database for data storage.

Features
User registration and authentication
View available stocks
Place buy and sell orders
In-memory database (H2) for testing
Technologies Used
Java: Programming language
Spring Boot: Framework for building the application
Spring Data JPA: For data access and manipulation
H2 Database: In-memory database for testing
Spring Security: For securing the application
Getting Started
Prerequisites
Java 11 or later
Maven
Installation
Clone the repository:

bash

Verify

Open In Editor
Edit
Copy code
git clone https://github.com/yourusername/stock-trading-platform.git
cd stock-trading-platform
Build the project using Maven:

bash

Verify

Open In Editor
Edit
Copy code
mvn clean install
Run the application:

You can run the application using the following command:

bash

Verify

Open In Editor
Edit
Copy code
mvn spring-boot:run
Alternatively, you can run the generated JAR file:

bash

Verify

Open In Editor
Edit
Copy code
java -jar target/stock-trading-platform-0.0.1-SNAPSHOT.jar
Accessing the Application
Once the application is running, you can access it at http://localhost:8080.

API Endpoints
User Registration

POST /api/users/register
Request body:
json

Verify

Open In Editor
Edit
Copy code
{
  "username": "your_username",
  "password": "your_password"
}
Get All Stocks

GET /api/stocks
Place an Order

POST /api/orders
Request body:
json

Verify

Open In Editor
Edit
Copy code
{
  "userId": 1,
  "stockSymbol": "AAPL",
  "quantity": 10,
  "orderType": "buy"
}
Example Usage
Register a new user: Send a POST request to /api/users/register with the required fields.

View available stocks: Send a GET request to /api/stocks.

Place an order: Send a POST request to /api/orders with the appropriate JSON body.

Database
This application uses an in-memory H2 database. You can access the H2 console at http://localhost:8080/h2-console (default username: sa, no password).

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Special thanks to the Spring community for their extensive documentation and support.
