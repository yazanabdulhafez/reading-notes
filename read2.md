# Arrays, Loops, Imports

## A Guide to Java Loops

![loops](https://static.javatpoint.com/images/java-loops.png)

In programming languages, looping is a feature which facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.

Java provides different types of loops:

1. For Loop:A for loop is a control structure that allows us to repeat certain operations by incrementing and evaluating a loop counter.

The syntax of the for loop is:

```java
for (initialization; Boolean-expression; step) 
  statement;
```

2. While Loop: It repeats a statement or a block of statements while its controlling Boolean-expression is true.

The syntax of the while loop is:

```java
while (Boolean-expression) 
    statement;
```

3. Do-While Loop:The do-while loop works just like the while loop except for the fact that the first condition evaluation happens after the first iteration of the loop.

The syntax of the do-while loop is:

```java
do {
    statement;
} while (Boolean-expression);
```

## Packages and Import

### Packages

A package name is the same as the directory (folder) name which contains the .java files.

The first statement, other than comments, in a Java source file, must be the package declaration.

#### Package declaration syntax

The statement order is as follows. Comments can go anywhere.

1. Package statment (optional).
2. Imports (optional).
3. Class or interface definitions.

```java
// This source file must be Drawing.java in the illustration directory.

package illustration;

import java.awt.*;

public class Drawing {
    . . .
}
```

### Import: three options

* Make all classes visible altho only one is used.
* Make a single class visible.
* The fully qualified class name without an import.

#### Common imports

There are 166 packages containing 3279 classes and interfaces in Java 5. However, only a few packages are used.

|import|usage                           |
|------------------|--------------------|
|import java.awt.*;|Common GUI elements.|
|import java.awt.event.*;|The most common GUI event listeners.|
|import javax.swing.*;|More common GUI elements. Note "javax".|
|import java.util.*;|Data structures (Collections), time, Scanner, etc classes.|
|import java.io.*;|Input-output classes.|
|import java.text.*;|Some formatting classes.|
|import java.util.regex.*;|Regular expression classes.|

 Just right click on the source file and choose Fix Imports. It will add all necessary import statements.

## Resources using in this reading

1. <https://www.baeldung.com/java-loops>
2. <https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html>
