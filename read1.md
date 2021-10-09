# Java Basics

## Language Basics

### Variables

The Java programming language defines the following kinds of variables:

* .Instance Variables (Non-Static Fields)
* .Class Variables (Static Fields)
* .Local Variables
* .Parameters

#### Naming

The rules and conventions for naming variables in the Java programming language can be summarized as follows:

* .Variable names are case-sensitive.
* .Subsequent characters may be letters, digits, dollar signs, or underscore characters.
* .If the name you choose consists of only one word, spell that word in all lowercase letters.

### Operators

Operators are special symbols that perform specific operations on one, two, or three operands, and then return a result.

| Operators            | Precedence                    |
| -------------------- | ----------------------------- |
| postfix              | expr++ expr--                 |
| unary                | ++expr --expr +expr -expr ~ ! |
| multiplicative       | \* / %                        |
| additive             | + -                           |
| shift                | << >> >>>                     |
| relational           | < > <= >= instanceof          |
| equality             | == !=                         |
| bitwise AND          | &                             |
| bitwise exclusive OR | ^                             |
| bitwise inclusive OR | \|                            |
| logical AND          | &&                            |
| logical OR           | \|\|                          |
| ternary              | ? :                           |
| assignment           | = += -= \*= /= %= &= ^=       |

### Expressions, Statements, and Blocks

#### Expressions

An expression is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value.

```java
//examole of exprissions
int cadence = 0;
anArray[0] = 100;
System.out.println("Element 1 at index 0: " + anArray[0]);

int result = 1 + 2; // result is now 3
if (value1 == value2) 
    System.out.println("value1 == value2");

```

#### Statements

Statements are roughly equivalent to sentences in natural languages. A statement forms a complete unit of execution.

 Here are some examples of expression statements.

```java

// assignment statement
aValue = 8933.234;
// increment statement
aValue++;
// method invocation statement
System.out.println("Hello World!");
// object creation statement
Bicycle myBike = new Bicycle();
```

#### Blocks

A block is a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed.

The following example, BlockDemo, illustrates the use of blocks:

```java
class BlockDemo {
     public static void main(String[] args) {
          boolean condition = true;
          if (condition) { // begin block 1
               System.out.println("Condition is true.");
          } // end block one
          else { // begin block 2
               System.out.println("Condition is false.");
          } // end block 2
     }
}
```

### Control Flow Statements

The statements inside the source files are generally executed from top to bottom, in the order that they appear. Control flow statements, however, break up the flow of execution by employing decision making, looping, and branching, enabling  program to conditionally execute particular blocks of code.

The decision-making statements (if-then, if-then-else, switch), the looping statements (for, while, do-while), and the branching statements (break, continue, return) supported by the Java programming language.

## Compiling

When you compile code, the compilor (usually another program) takes the program the human wrote, and converts it into the program the computer can understand (i.e. converts from Java to machine language). The very short version could be, yes, compile means to make the code executable.

## Making Sense of Java’s API Documentation

You can find things in the API documentation in a number of different ways.

1. Using the index.
2. Using the list of classes.

To create the API documentation, the captains of Java ran a program called javadoc. The javadoc program took lines like these right out of the PrintStream.java file and used the lines to make the documentation that you see in your web browser.

you can use the javadoc program to create your own documentation. When you download the JDK, you get the javadoc program as part of the deal.

### Resources used in this reading

1. <https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html>
2. <https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/>
3. <https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/>
