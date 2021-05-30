# [Operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators) and [Loops](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)
Operators
JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

* Assignment operators
* Comparison operators
* Arithmetic operators
* Bitwise operators
* Logical operators
* String operators
* Conditional (ternary) operator
* Comma operator
* Unary operators
* Relational operators

## Assignment operators
An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = y assigns the value of y to x.

## Comparison operators
A comparison operator compares its operands and returns a logical value based on whether the comparison is true. The operands can be numerical, string, logical, or object values. 

## Arithmetic operators
An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value. The standard arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). 

## Bitwise operators
A bitwise operator treats their operands as a set of 32 bits (zeros and ones), rather than as decimal, hexadecimal, or octal numbers. 
Bitwise operator examples

|Expression|	Result|	Binary Description|
|----|------|-----|------|
|15 & 9|	9|	1111 & 1001 = 1001|
|15 &#124 9|	15|	1111 &#124 1001 = 1111|
|15 ^ 9	|6	|1111 ^ 1001 = 0110|
|~15	|-16|	~ 0000 0000 ... 0000 1111 = 1111 1111 ... 1111 0000|

## Logical operators
Logical operators are typically used with Boolean (logical) values; when they are, they return a Boolean value. However, the && and || operators actually return the value of one of the specified operands, so if these operators are used with non-Boolean values, they may return a non-Boolean value. 

## String operators
In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

For example,

console.log('my ' + 'string'); // console logs the string "my string".


Loops and iteration
======
There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. (Note that it's possible that number could be zero!)

The various loop mechanisms offer different ways to determine the start and end points of the loop. There are various situations that are more easily served by one type of loop over the others.

The statements for loops provided in JavaScript are:

* for statement
* do...while statement
* while statement
* labeled statement
* break statement
* continue statement
* for...in statement
* for...of statement

## for statement
A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop.

A for statement looks as follows:

***for ([initialExpression]; [conditionExpression]; [incrementExpression])***

 ***{ statement}***

When a for loop executes, the following occurs:

1. The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
3. The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
4. If present, the update expression incrementExpression is executed.
5. Control returns to Step 2.

## while statement
A while statement executes its statements as long as a specified condition evaluates to true. A while statement looks as follows:

***while (condition){***

  ***statement}***

If the condition becomes false, statement within the loop stops executing and control passes to the statement following the loop.

The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.

To execute multiple statements, use a block statement ({ ... }) to group those statements.
## break statement
Use the break statement to terminate a loop, switch, or in conjunction with a labeled statement.

When you use break without a label, it terminates the innermost enclosing while, do-while, for, or switch immediately and transfers control to the following statement.
When you use break with a label, it terminates the specified labeled statement.
The syntax of the break statement looks like this:

**break;**

**break [label];**

1. The first form of the syntax terminates the innermost enclosing loop or switch.
2. The second form of the syntax terminates the specified enclosing labeled statement.