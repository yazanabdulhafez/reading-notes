# Maps, primitives, File I/O

## Primitives vs. Objects

### Java Type System

* Every object contains a single value of the corresponding primitive type.

* The wrapper classes are immutable so that their state can't change once the object is constructed and can't inherit from them.

* autoboxing:The process of converting a primitive type to a reference one and the opposite process is called unboxing

### Pros and Cons

The decision what object is to be used is based on:

1. what application performance we try to achieve.
2. how much available memory we have.
3. The amount of available memory.
4. what default values we should handle.

### Single Item Memory Footprint

* Primitive Types and Values live in the stack and hence are accessed fast.
* The reference types are objects, they live on the heap and are relatively slow to access

### Memory Footprint for Arrays

single-element arrays of primitive types are almost always more expensive (except for long and double) than the corresponding reference type.

### Performance

The performance of java code depends on:

1. the hardware that the code run on.
2. the compiler.
3. the state of the virtual machine.
4. the activity of other processes in the operating system.

The operations for primitive types are faster than those for wrapper classes.

### Default Values

Default values of the primitive types are 0,false for the boolean type,while the reference types might acquire a value (null).

### Usage

* The primitive types are much faster and need less memory so its might prefered to use.

* When need collections with a large number of elements, we should use arrays with “economical” type to save memory.

## Exceptions in Java

* An exceptionit is an event  occurs during the execution of a program that disrupts the normal flow of instructions.

* The Java uses exceptions to handle errors and other exceptional events.

* A program can catch exceptions by using a combination of the try, catch, and finally blocks.

In Java there are three types of exceptions namely:

![exceptions](https://static.javatpoint.com/core/images/types-of-exception-handling.png)

## Using Scanner to read in a file in Java

Scanner are useful for breaking down formatted input into tokens and translating individual tokens according to their data type.

By default, a scanner uses white space to separate tokens.

## Resources used in this reading

1. [Primitives vs. Objects](https://www.baeldung.com/java-primitives-vs-objects)
2. [Exceptions](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)
3. [Scanner](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)