# OO Design

## SOLID Principles

* The SOLID Principles are five principles of Object-Oriented class design. These principles developers create and maintain a codebase that is strong but flexible to grow and change with minimal difficulty.

* The SOLID Principles are:
   
   1. **S** : Single-responsiblity Principle.

   2. **O** : Open-closed Principle.

   3. **L** : Liskov Substitution Principle.

   4. **I** : Interface Segregation Principle.

   5. **D** : Dependency Inversion Principle.

## The Single Responsibility Principle (SRP)

* A class should have one, and only one, reason to change that means the class should have only one job.

## The Open Closed Principle (OCP)

* We should be able to extend a classes behavior, without modifying.

## The Liskov Substitution Principle (LSP)

* Derived classes must be substitutable for their base classes. That means when we create a new derived class from a base class we should not have to modify code to work this derived class.

## The Interface Segregation Principle (ISP) 

* Clients should not be forced to depend upon interfaces that they do not use. This is all about building multiple interfaces that will provide only the methods that a client needs. Simple put it’s better to have two smaller interfaces than one large fat interface.

## The Dependency Inversion Principle (DIP)

* Depend on abstraction, not on concretions. That means our class should depends on interfaces or acstract class insted of concretions classes and functions.