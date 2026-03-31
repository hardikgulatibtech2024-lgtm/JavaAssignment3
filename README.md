
---

# Book Store Management System (Java)

## Overview

This project is a **Java-based Book Store Management System** that demonstrates core object-oriented programming concepts along with custom exception handling and dynamic data storage using collections.

The program allows the creation and management of book objects, validates input data using a custom exception, and stores multiple books using an `ArrayList`. It also demonstrates the use of constructors, including default, parameterized, and copy constructors.

---

## Features

* Create book objects using different types of constructors
* Store multiple books using `ArrayList`
* Validate book data using a custom exception
* Display details of all books
* Demonstrate exception handling with invalid inputs
* Copy existing book objects using a copy constructor

---

## Project Structure

### 1. InvalidBookException Class

A custom exception class that extends `Exception`.

Purpose:

* Used to validate book data during object creation
* Ensures that invalid values such as negative price or stock are not accepted

---

### 2. Book Class

Represents a book entity with relevant attributes and methods.

#### Data Members

* `title` – name of the book
* `author` – author of the book
* `price` – price of the book
* `stockCount` – number of copies available
* `ISBN` – unique identifier for the book

#### Constructors

* **Default Constructor** – initializes values with defaults
* **Parameterized Constructor** – initializes with user-defined values and performs validation
* **Copy Constructor** – creates a new object by copying an existing book

#### Methods

* `display()` – prints the details of the book

---

### 3. BookStoreDemo Class

The main class containing the `main` method.

Responsibilities:

* Creates book objects
* Stores them in an `ArrayList`
* Displays all book details
* Demonstrates exception handling by attempting to create an invalid book

---

## Validation Rules

The program enforces the following conditions:

* Price must not be negative
* Stock count must not be negative
* ISBN must not be null and should have a minimum length

If any of these conditions fail, an `InvalidBookException` is thrown.

---

## How to Run the Program

### Prerequisites

* Java Development Kit (JDK) installed
* Terminal or command prompt

### Steps

1. Compile the program:

```
javac BookStoreDemo.java
```

2. Run the program:

```
java BookStoreDemo
```

---

## Sample Output

```
Book Details:

Title      : Java Programming
Author     : Herbert Schildt
Price      : 550.0
StockCount : 10
ISBN       : ISBN001
---------------------------

Title      : Python for Data Science
Author     : Jake VanderPlas
Price      : 650.0
StockCount : 5
ISBN       : ISBN002
---------------------------

Exception Occurred: Price cannot be negative.
```

---

## Concepts Used

* Object-Oriented Programming (OOP)
* Classes and Objects
* Encapsulation
* Constructors (Default, Parameterized, Copy)
* Exception Handling (try-catch)
* Custom Exceptions
* Java Collections (`ArrayList`)

---

## Future Enhancements

* Add methods to update or delete books
* Search functionality by title or ISBN
* File handling for persistent storage
* User input-based system instead of hardcoded values
* GUI implementation using Java Swing or JavaFX

---


