# Dynamic web pages with JavaScript
## [Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators)

Operators
JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.

- Assignment operators

- Comparison operators

- Arithmetic operators

- Bitwise operators

- Logical operators

- String operators

- Conditional (ternary) operator

- Comma operator

- Unary operators

- Relational operators


## 1. Assignment operators
***An assignment operator assigns a value to its left operand based on the value of its right operand. The simple assignment operator is equal (=), which assigns the value of its right operand to its left operand. That is, x = y assigns the value of y to x.***

There are also compound assignment operators that are shorthand for the operations listed in the following table:

Return value and chaining
Like most expressions, assignments like x = y have a return value. It can be retrieved by e.g. assigning the expression or logging it:

const z = (x = y); // Or equivalently: const z = x = y;

console.log(z); // Log the return value of the assignment x = y.
console.log(x = y); // Or log the return value directly.

## 2. Comparison operators
**A comparison operator compares its operands and returns a logical value based on whether the comparison is true.** The operands can be numerical, string, logical, or object values. Strings are compared based on standard lexicographical ordering, using Unicode values. In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. This behavior generally results in comparing the operands numerically. The sole exceptions to type conversion within comparisons involve the === and !== operators, which perform strict equality and inequality comparisons. 

## 3. Arithmetic operators
**An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value.** The standard arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). 

### String operators
In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

For example,

console.log('my ' + 'string'); // console logs the string "my string".

JavaScript Operators:
The assignment operator (=) assigns a value to a variable.

### JavaScript Arithmetic Operators
Arithmetic operators are used to perform arithmetic on numbers:

|	Description| Operator|
|------|-------|
|	Addition |+|
|Subtraction| -|
|	Multiplication| *|
|	Exponentiation |**|
|	Division|/|
|	Modulus (Division Remainder)|%|
|Increment |++|
|	Decrement |--|

JavaScript String Operators
The + operator can also be used to add (concatenate) strings.

Example
var txt1 = "John";
var txt2 = "Doe";
var txt3 = txt1 + " " + txt2;

The result of txt3 will be:
John Doe

### JavaScript Comparison Operators:

|Comparison Operators|symbol|
|------|--------|
	| equal to| ==|
	| equal value and equal type| ===|	
	 |not equal |!=|
	 |not equal value or not equal type| !==|
	 |greater than| >|
   |less than |<|	
	 |greater than or equal to |>=|
	|less than or equal to| <=|
	| ternary operator |?|

### JavaScript Logical Operators

|JavaScript Logical Operators|Operator	Description|
|-----------|----------------|
|&&	       | logical and | 
| &#124;&#124;   | logical or  |
|!	       | logical not |


## [Control flow](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling)

The control flow is the order in which the computer executes statements in a script.
Code is run in order from the first line in the file to the last line, unless the computer runs across the (extremely frequent) structures that change the control flow, such as conditionals and loops.

An if statement looks like this:

**if (condition) {
  statement_1;
} else {
  statement_2;
}**

*A typical script in JavaScript or PHP (and the like) includes many control structures, including conditionals, loops and functions. Parts of a script may also be set to execute when events occur.
Control flow means that when you read a script, you must not only read from start to finish but also look at program structure and how it affects order of execution.*

<<<<<<< HEAD
=======
Arithmetic operators
An arithmetic operator takes numerical values (either literals or variables) as their operands and returns a single numerical value. The standard arithmetic operators are addition (+), subtraction (-), multiplication (*), and division (/). 

String operators
In addition to the comparison operators, which can be used on string values, the concatenation operator (+) concatenates two string values together, returning another string that is the union of the two operand strings.

For example,

console.log('my ' + 'string'); // console logs the string "my string".

