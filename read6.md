# Inheritance and Interfaces

## Classes

A class is a blueprint or prototype we can create objects from it. It represents a set of properties or methods that are common to all objects of one type.

A class in Java can contain:

1. Fields
2. Methods
3. Constructors
4. Blocks
5. Nested class and interface

## Object

It is a basic unit of Object-Oriented Programming and represents the real life entities.the object is an instance of a class and have state and behavior.

An object consists of :

1. State: It is represented by attributes of an object.
2. Behavior: It is represented by methods of an object.
3. Identity: this typically implemented via a unique ID. The value of the ID is not visible to the external user. However, it is used internally by the JVM.

## Inheritance

It the process of taking all of the properties and behaviors of a parent class and extend it to a child class.

### Terms used in Inheritance

1. Sub Class: its a class which inherits the other class. It is also called a derived class, extended class, or child class.
2. Super Class: its the class from where a subclass inherits the features. It is also called a base class or a parent class.

we use the keyword of **extends** to make the inheritance in Java.

## Interfaces

An interface is a reference type, similar to a class, that can contain only constants, method signatures, default methods, static methods, and nested types.

we can declare an interface by using the interface keyword.

### Differences between Interface and Class in Java

1. Unlike a class, you cannot instantiate or create an object of an interface.
2. All the methods in an interface should be declared as abstract.
3. An interface does not contain any constructors, but a class can.

The class can extends another class,interface can extends another interface,But an interface can not be extended or inherited by a class; it is implemented by a class.

## Package

Its the main dirctory that contain a group of classes,interfaces and sub-packages.
In java there are two forms of packages:

1. built-in packages.
2. user defind packages.

The Java platform provides an enormous class library (a set of packages) suitable for use in your own applications. This library is known as the "Application Programming Interface", or "API".

## Resources used in this reading

1. [Object and Class](https://docs.oracle.com/javase/tutorial/java/concepts/object.html)
1. [Inheritance & Interfaces](https://docs.oracle.com/javase/tutorial/java/IandI/createinterface.html)
