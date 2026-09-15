# 🚗 Car Rental System

A simple **Car Rental System built using Java**. This is a console-based application that allows users to rent and return cars while managing customers, rentals, car availability, and rental prices.

## 📌 Project Overview

The Car Rental System provides a basic implementation of a car rental service using **Object-Oriented Programming (OOP)** concepts in Java.

The system allows users to:

* 🚘 View available cars
* 👤 Enter customer information
* 📅 Select the number of rental days
* 💰 Calculate the total rental price
* ✅ Confirm a car rental
* 🔄 Return a rented car
* 🚫 Prevent unavailable cars from being rented

## 🛠️ Technologies Used

* **Java**
* **Java Collections Framework**
* `ArrayList`
* `Scanner`
* Object-Oriented Programming (OOP)

## 📂 Project Structure

```text
Car-Rental-System/
│
├── rental_car_project.java
└── README.md
```

## 🧩 Main Classes

### 1. `Car`

Represents a car in the rental system.

It stores:

* Car ID
* Brand
* Model
* Price per day
* Availability status

Main methods:

```java
calculatePrice()
isAvailable()
rent()
returnCar()
```

### 2. `Customer`

Represents a customer who rents a car.

It stores:

* Customer ID
* Customer name

### 3. `Rental`

Represents a rental transaction.

It connects:

* A `Car`
* A `Customer`
* Number of rental days

### 4. `CarRentalSystem`

Manages the complete rental system.

It maintains:

* List of cars
* List of customers
* List of rentals

It also provides functionality for:

* Adding cars
* Adding customers
* Renting cars
* Returning cars
* Displaying the menu

### 5. `rental_car_project`

Contains the `main()` method and starts the application.

## 🚘 Available Cars

The program currently contains three cars:

| Car ID | Brand    | Model  | Price/Day |
| ------ | -------- | ------ | --------- |
| C001   | Toyota   | Camry  | $60       |
| C002   | Honda    | Accord | $70       |
| C003   | Mahindra | Thar   | $150      |

## ▶️ How to Run

### Prerequisites

Make sure **Java JDK** is installed on your computer.

Check the Java installation:

```bash
java -version
```

Check the Java compiler:

```bash
javac -version
```

### Step 1: Clone the Repository

```bash
git clone https://github.com/your-username/your-repository-name.git
```

### Step 2: Open the Project Folder

```bash
cd your-repository-name
```

### Step 3: Compile the Program

```bash
javac rental_car_project.java
```

### Step 4: Run the Program

```bash
java rental_car_project
```

## 💻 Sample Output

```text
===== Car Rental System =====
1. Rent a Car
2. Return a Car
3. Exit
Enter your choice: 1

== Rent a Car ==

Enter your name: Meet

Available Cars:
C001 - Toyota Camry
C002 - Honda Accord
C003 - Mahindra Thar

Enter the car ID you want to rent: C003
Enter the number of days for rental: 2

== Rental Information ==

Customer ID: CUS1
Customer Name: Meet
Car: Mahindra Thar
Rental Days: 2
Total Price: $300.00

Confirm rental (Y/N): Y

Car rented successfully.
```

## 🔄 Returning a Car

To return a car, select option `2`:

```text
===== Car Rental System =====
1. Rent a Car
2. Return a Car
3. Exit
Enter your choice: 2

== Return a Car ==

Enter the car ID you want to return: C003

Car returned successfully by Meet
```

The car will become available again for future rentals.

## 🧠 OOP Concepts Used

This project demonstrates several important Java OOP concepts:

### Encapsulation

Class variables are declared `private` and accessed through methods.

Example:

```java
private String carId;
private String brand;
private double basePricePerDay;
```

### Classes and Objects

The project creates objects such as:

```java
Car car1 = new Car("C001", "Toyota", "Camry", 60.0);
```

### Constructors

Constructors are used to initialize objects:

```java
public Car(String carId, String brand, String model, double basePricePerDay)
```

### Association

A `Rental` object connects a `Car` with a `Customer`.

```java
private Car car;
private Customer customer;
```

### Collections

`ArrayList` is used to store cars, customers, and rental records:

```java
private List<Car> cars;
private List<Customer> customers;
private List<Rental> rentals;
```

## 💰 Price Calculation

The rental price is calculated using:

```text
Total Price = Price Per Day × Number of Rental Days
```

For example:

```text
Mahindra Thar
Price per day = $150
Rental days = 2

Total = $150 × 2
      = $300
```

## ✨ Features

* [x] Add cars
* [x] Display available cars
* [x] Rent a car
* [x] Calculate rental price
* [x] Generate customer ID
* [x] Return a car
* [x] Track car availability
* [x] Prevent renting an already rented car
* [x] Console-based menu

## 🔮 Future Improvements

The project can be extended with:

* 🔐 User login and authentication
* 💳 Online payment system
* 🗄️ Database integration using MySQL
* 📋 Rental history
* 📅 Rental dates
* 🚘 More car categories
* 💵 Discounts and offers
* 🧾 Automatic invoice generation
* 🖥️ GUI using Java Swing or JavaFX
* 🌐 Web-based version using Spring Boot

## 🎓 Learning Purpose

This project was created as a **Java learning project** to practice:

* Java fundamentals
* OOP concepts
* Classes and objects
* Constructors
* Encapsulation
* ArrayList
* Loops and conditional statements
* User input using `Scanner`
* Basic project structure

## 👨‍💻 Author

**Meet Patel**

This project is created for learning and educational purposes.

## 📄 License

This project is available for educational and personal use.
