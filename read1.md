# Java Basics

## Language Basics

### Variables

Java  defines the following kinds of variables:

* Instance Variables (Non-Static Fields)
* Class Variables (Static Fields)
* Local Variables
* Parameters

#### Naming

The rules and conventions for naming variables in  Java :

* Variable names are case-sensitive.
* Subsequent characters may be letters, digits, dollar signs, or underscore characters.
* If the name you choose consists of only one word, spell that word in all lowercase letters.

### Operators

Operators are special symbols that perform specific operations and then return a result.

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

An expression is a construct made up of variables, operators, and method invocations.

```java
//example of expressions

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

 Control flow statements break up the flow of execution by employing decision making, looping, and branching, enabling  program to conditionally execute particular blocks of code.

![control flow statments](https://1.bp.blogspot.com/-CPYEexud4bY/XbgOqC_PPdI/AAAAAAAADKg/i7XJ_xqEYFM_7Yw0eZq6dFhDaub1s0c-gCLcBGAsYHQ/s1600/java-control-flow-statement.png)

## Compiling

![compiling](https://miro.medium.com/max/1000/1*Qbm5_d5EYIbYa1-jN4JmSg.jpeg)

Its the process of converting the program that human wrote into the program the computer can understand and make the code executable.

## Making Sense of Java’s API Documentation

You can find things in the API documentation in a number of different ways.

1. Using the index.
2. Using the list of classes.

you can use the javadoc program to create your own documentation. When you download the JDK, you get the javadoc program as part of the deal.

### Resources used in this reading

1. <https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html>
2. <https://www.reddit.com/r/explainlikeimfive/comments/233dq5/eli5_what_does_it_mean_to_compile_code/>
3. <https://www.dummies.com/programming/java/making-sense-of-javas-api-documentation/>
