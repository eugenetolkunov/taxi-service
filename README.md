﻿# taxi-service
This web application is a straightforward taxi service that incorporates authentication, registration, and CRUD (Create, Read, Update, Delete) functionalities. It has been developed following the SOLID principles and utilizes the Dependency Injection pattern. The application's key features encompass authentication, CRUD operations for managing cars and drivers, clear separation between the logical layers of the system, and authentication filtering. It prioritizes user-friendliness, adheres to programming standards, and presents users with a convenient and intuitive user interface.

# Functional
1. Authentication:
* Register or log in as a driver.
2. Driver Management:
* Create, delete, and update driver information.
* Display a list of all drivers.
3. Car Management:
* Create, delete, and update car details.
* Add a driver to a car.
* Display a list of all cars.
4. Manufacturer Management:
* Create, delete, and update manufacturer information.
* Display a list of all manufacturers.

# Project structure
* Controller Layer: This layer handles user requests and contains the logic for responding to those requests. It communicates with the Service Layer to access the business logic. The Controller Layer ensures that the user's input is processed correctly and triggers the appropriate actions.

* Service Layer: The Service Layer contains the business logic for the entire application. It encapsulates the rules and operations that drive the functionality of the taxi service. The Service Layer communicates with the DAO Layer to perform CRUD operations on Car, Manufacturer, and Driver entities. It ensures that the application's business logic is applied consistently and handles any necessary data transformations.

* DAO Layer: The DAO (Data Access Object) Layer provides access to the underlying data storage and performs CRUD operations on Car, Manufacturer, and Driver entities. It encapsulates the logic for interacting with the database or any other persistence mechanism. The DAO Layer is responsible for executing queries, fetching and storing data, and maintaining data integrity.

# Technologies
* Java 11
* Maven 3.1.1
* MySQL 8.0.22
* JDBC
* Tomcat 9.0.76
* Java Servlet
* JSTL 1.2

# How to run app
1.  Fork the project on GitHub to create your own copy.
2. Clone the project from your GitHub repository to your local machine.
3. Install Apache Tomcat version 9.x.x on your system.
4. Create all the required tables by executing the code from the init_db.sql file. This will set up the necessary database schema.
5. In the ConnectionUtil class, provide the necessary data for the URL, username, password, and JDBC driver fields. This information will allow the application to connect to your database.
6. Configure Tomcat to include this project. This typically involves specifying the project's context path and other relevant settings in the Tomcat configuration files.
7. Run the project by starting Apache Tomcat. This will deploy the web application and make it accessible through the specified context path.
