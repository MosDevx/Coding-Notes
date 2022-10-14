==================DESIGN PATTERNS========================




========CREATIONAL=========

## 1.Factory Method

Pattern that provides an interface for creating objects in a superclass,but allows subclasses to define type of object that will be created.
You replace direct object construction calls(using new method)  with calls to a factory method -- you overide the factory method in subclasses which then reurn what object you need(via calling new of course)
The objects returnred form factory methods are called products
The subclasses must have a common interface or base class && the factoryy method in the base class should have its return to be this interface

--- so we have two inheritance hierachies
	1. The products inheriting from common interface.
	2. The Creator class. It has the factory method(can be abstract to force all subclasses to have an implementation) whose return type is the aforementioned interface. Its subclasses are responsible for return a new product

Note: Cretor class has buisness logic to it. Its main purpose isnt creating products.


## 2.Abstract Factory 
lets you produce families of related objects without specifying their concrete classes


//from HeadFirst
======================= BEHAVIORAL =================

## 1.Strategy Pattern
	Defines a family of algorithms encapsulates each one and makes them interchangeable. Strategy lets the algorithm
	vary independently from clients that use it.

	Some Design principles applied:
	1. Identify aspects that vary and separate them from what stays the same
	2. Program to an interface not an implementation
	3. Favor composition over inheritance

