
Assignment 2 – Object-Oriented Vehicle Management System

Project Overview

This project is a simple Object-Oriented Vehicle Management System written in Java.
It demonstrates the use of core Object-Oriented Programming (OOP) concepts such as
inheritance, abstraction, method overriding, composition, polymorphism, and working
with arrays of objects.

The system models different types of vehicles (Car, Motorcycle, Truck) using a common
abstract superclass Vehicle. Each vehicle can be associated with a driver and provides
its own implementation of engine behavior.

The project was developed as part of an academic assignment to practice object-oriented
design, clean code structure, and GitHub project organization.


---

Learning Goals Covered

Inheritance and superclass–subclass relationships

Abstract classes and abstract methods

Method overriding and polymorphism

Composition and aggregation between classes

Constructor chaining using super

Access modifiers (private and protected)

Working with arrays of objects

Clean and readable Java code structure

GitHub repository organization and documentation


---

Class Descriptions

Vehicle Class (Abstract)

The Vehicle class represents a general vehicle and serves as the superclass for all
specific vehicle types.

Fields:

brand – vehicle brand

year – manufacturing year

driver – Driver object associated with the vehicle


Key Methods:

startEngine() – abstract method

stopEngine() – abstract method

displayInfo() – prints vehicle brand and year

displayDriver() – prints driver information if assigned


The Vehicle class demonstrates abstraction and defines common behavior for all vehicles.


---

Car Class

The Car class represents a car and extends the Vehicle class.

Additional Fields:

doors – number of doors

fuelType – type of fuel


Key Features:

Overrides startEngine() and stopEngine()

Uses constructor chaining with super


---

Motorcycle Class

The Motorcycle class represents a motorcycle and extends the Vehicle class.

Additional Field:

hasSidecar – indicates whether the motorcycle has a sidecar


Key Features:

Overrides startEngine() and stopEngine()

Provides its own engine behavior


---

Truck Class

The Truck class represents a truck and extends the Vehicle class.

Additional Fields:

capacity – load capacity

numAxles – number of axles


Key Features:

Overrides startEngine() and stopEngine()

Demonstrates inheritance with additional properties


---

Driver Class

The Driver class represents a vehicle driver.

Fields:

name – driver’s name

licenseNumber – driver’s license number


Key Method:

displayDriverInfo() – prints driver details


This class is used to demonstrate composition and aggregation with vehicles.


---

Main Class

The Main class is the entry point of the program.

It:

Creates multiple Driver objects

Creates Car, Motorcycle, and Truck objects

Assigns drivers to vehicles

Stores all vehicles in a Vehicle[] array

Uses a loop to:

Start the engine

Display vehicle information

Display driver information

Stop the engine


This demonstrates polymorphism and array-based processing.


---

How to Compile and Run

From the src directory:

javac *.java
java Main


---

Screenshots

Screenshots of the program output can be found in:

docs/screenshots/

They demonstrate correct execution of the program and vehicle-driver interactions.


---

Reflection

Working on this project helped me better understand inheritance and abstraction in Java.
Using an abstract superclass simplified the design by allowing shared behavior to be
defined in one place, while method overriding allowed each vehicle type to implement
its own engine logic.

One of the main challenges was correctly designing class relationships and using access
modifiers properly. This project improved my understanding of polymorphism and clean
object-oriented design.


---

Repository Structure

assignment2-vehicle-system/
├── src/
│   ├── Vehicle.java
│   ├── Car.java
│   ├── Motorcycle.java
│   ├── Truck.java
│   ├── Driver.java
│   └── Main.java
├── docs/
│   └── screenshots/
├── README.md
└── .gitignore


---

Author

Madi
