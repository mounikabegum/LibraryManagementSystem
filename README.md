#Library Management System – Java
Project Overview

This is a console-based Library Management System built using Java and Object-Oriented Programming (OOP) concepts.
The system allows managing books, members, issuing and returning books, and calculating fines for late returns.

The application uses the Strategy Design Pattern to handle fine calculation, making the system flexible and easy to extend.

##Tech Stack

Language:

Java (Core Java)

Concepts & Tools:

Object-Oriented Programming (OOP)

Strategy Design Pattern

Java Collections Framework

##Features

Add books to the library

Register members

Issue books to members

Return books

View available books

Fine calculation for late returns

Clean and modular code structure

##Entities & Responsibilities
------------------------------------------------------------
Entity           |	Responsibility
------------------------------------------------------------
BookItem    |   Represents a physical book
Member	    |   Represents a library member
Loan	    |   Stores issued book details
Library	    |   Manages core operations
FineStrategy|	Defines fine calculation logic

##How to Run the Project
Compile
javac src/Main.java src/model/*.java src/service/*.java src/strategy/*.java

Run
java -cp src Main

##Explanation

Book availability is tracked using status (AVAILABLE / ISSUED)

When a book is issued, its status changes to ISSUED

When returned, the status changes back to AVAILABLE

The Library class manages all operations

Fine calculation is handled using the Strategy Pattern, allowing easy rule changes

##Sample Output
Issued The Alchemist: true
Issued Clean Code: true

Available books after issuing:
Design Patterns

Returned The Alchemist. Fine: 0.0

Available books after returning:
The Alchemist
Design Patterns

##Future Enhancements

Menu-driven console interface

Database integration

GUI / Web interface

JUnit test cases

Real-time date-based fine calculation

##Author

Mounika
