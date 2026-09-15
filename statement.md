# Problem Statement

Traditional car rental exercises often lack a structured way to model real-world operations such as car availability, customer registration, rental duration, price calculation, and vehicle returns in a single, cohesive system. This project addresses that gap by providing a simple command-line car rental management system where users can rent and return cars while tracking their rental information and car availability in real time.

## Scope of the Project

* 1. Implements a single-system, console-based car rental management system using object-oriented programming.
* 2. Supports basic car rental lifecycle actions: viewing available cars, renting a car, calculating rental charges, and returning a car.
* 3. Maintains customer and rental information using Java collections such as `ArrayList`.
* 4. Tracks the availability status of each car and prevents unavailable cars from being rented.
* 5. Focuses on backend logic and CLI interaction only; no database, networking, GUI, online payment, or authentication is included in the current scope.
* 6. Designed as a learning/demo project for Java OOP, collections, control flow, and basic business logic, not as a production-ready rental platform.

## Target Users

* 1. Students and beginners learning Java and object-oriented programming concepts.
* 2. Recruiters or reviewers evaluating basic OOP, collections, input handling, and business logic in Java.
* 3. Educators who need a small, understandable example of a car rental management system for teaching purposes.
* 4. Users who want to understand how a simple command-line rental system works.

## High-Level Features

* 1. Car management with unique car IDs, brand, model, daily rental price, and availability status.
* 2. Customer registration with automatically generated customer IDs and customer names.
* 3. Display of all currently available cars before making a rental.
* 4. Car rental operation with validation to ensure that only available cars can be rented.
* 5. Rental price calculation based on the car's daily price and the number of rental days.
* 6. Rental confirmation before changing the car's availability status.
* 7. Return operation that makes the rented car available again and removes the completed rental record.
* 8. Maintenance of customer and rental information using Java `ArrayList`.
* 9. Menu-driven command-line interface allowing continuous interaction until the user chooses to exit.
* 10. Demonstrates important Java OOP concepts including classes, objects, constructors, encapsulation, methods, and object relationships.

## System Components

The project consists of the following main classes:

### 1. Car

Represents a vehicle available for rental.

Stores:

* Car ID
* Brand
* Model
* Base price per day
* Availability status

### 2. Customer

Represents a customer using the rental service.

Stores:

* Customer ID
* Customer name

### 3. Rental

Represents an individual rental transaction.

Stores:

* Car information
* Customer information
* Number of rental days

### 4. CarRentalSystem

Acts as the main management component of the application.

Manages:

* Cars
* Customers
* Rental records
* Renting cars
* Returning cars
* Menu interaction

### 5. rental_car_project

Contains the `main()` method and initializes the car rental system with sample vehicles before starting the menu-driven application.

## Rental Price Calculation

The total rental price is calculated using the following formula:

```text
Total Price = Base Price Per Day × Number of Rental Days
```

For example:

```text
Mahindra Thar
Base Price = $150 per day
Rental Days = 3

Total Price = $150 × 3
            = $450
```

## Current Sample Cars

| Car ID | Brand    | Model  | Price Per Day |
| ------ | -------- | ------ | ------------- |
| C001   | Toyota   | Camry  | $60           |
| C002   | Honda    | Accord | $70           |
| C003   | Mahindra | Thar   | $150          |

## Project Limitations

* 1. Only a command-line interface is provided.
* 2. Data is stored temporarily in memory and is lost when the program terminates.
* 3. No database is used for permanent storage.
* 4. Only basic rental price calculation is implemented.
* 5. No user authentication or authorization is included.
* 6. No online payment or invoice generation is supported.
* 7. The current implementation is intended for educational purposes rather than real-world commercial use.

## Future Enhancements

The system can be extended with:

* 1. Database integration using MySQL.
* 2. Login and user authentication.
* 3. Admin and customer roles.
* 4. Rental history and detailed reports.
* 5. Different categories of vehicles.
* 6. Discount and promotional offers.
* 7. Online payment integration.
* 8. Automatic invoice generation.
* 9. Date-based rental and return tracking.
* 10. GUI using Java Swing or JavaFX.
* 11. Web-based implementation using Spring Boot.
* 12. REST API integration for a web or mobile application.

## Learning Objectives

This project helps demonstrate:

* Java fundamentals
* Object-Oriented Programming
* Classes and objects
* Constructors
* Encapsulation
* Methods
* Object relationships
* ArrayList and Java Collections
* Loops and conditional statements
* User input using `Scanner`
* Basic validation
* Menu-driven programming
* Simple business logic implementation

## Conclusion

The Car Rental System provides a simple and understandable implementation of a real-world rental management process using Java. It demonstrates how object-oriented programming can be used to represent cars, customers, and rental transactions while maintaining car availability and calculating rental costs. The project provides a foundation that can later be extended into a complete database-driven or web-based car rental application.
