# HTML Tables; JS Constructor Functions

## Domain Modeling

Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

Generate random numbers
To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

EpicFailVideo.prototype.generateRandom = function(min, max) {
  return Math.floor(Math.random() * (max - min + 1)) + min;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail.generateRandom(1, 5));
console.log(corgiFail.generateRandom(1, 5));

some tips to follow when building your own domain models.

1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside.

## Basic Table Structure

![html table](https://cf2.ppt-online.org/files2/slide/x/x03e9GTk5pRrMdEywnDSZbjBHJ2zoYaFmfuKsh/slide-4.jpg)

The `<table>` element is used
to create a table. The contents
of the table are written out row
by row.
You indicate the start of each
row using the opening `<tr>` tag.
(The tr stands for table row.)
It is followed by one or more
`<td>` elements (one for each cell
in that row).
At the end of the row you use a
closing `</tr>` tag.
Each cell of a table is
represented using a `<td>`
element. (The td stands for
table data.)
At the end of each cell you use a
closing `</td>` tag.

The `<th>` element is used just
like the `<td>` element but its
purpose is to represent the
heading for either a column or
a row. (The th stands for table
heading.)
The colspan attribute can be
used on a `<th>` or `<td>` element
and indicates how many columns
that cell should run across.

The rowspan attribute can be
used on a `<th>` or `<td>` element
to indicate how many rows a cell
should span down the table.

There are three elements that
help distinguish between the
main content of the table and
the first and last rows (which can
contain different content).

The headings of the table should
sit inside the `<thead>` element.

The body should sit inside the
`<tbody>` element.

The footer belongs inside the
`<tfoot>` element.
The width attribute was used
on the opening `<table>` tag to
indicate how wide that table
should be and on some opening
`<th>` and `<td>` tags to specify
the width of individual cells.
The value of this attribute is
the width of the table or cell in
pixel
The border attribute was used
on both the `<table>` and `<td>`
elements to indicate the width of
the border in pixels.

## [objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Working_with_Objects?retiredLocale=ar)

![object img](https://miro.medium.com/max/700/1*iKJx57JU9sKdff-Os7upyA.png)
Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

|METHOD                      |   DESCRIPTION                |
|-------------               |  ----------------------------|
|toUpperCase ()              | Changes string to uppercase characters|
|tolowerCase ()| Changes string to lowercase characters        |
|charAt ()|Takes an index number as a parameter, and returns the character found at that position  |
|indexOf() |Returns index number of the first time a character or set of characters is found within the string|
|lastlndexOf() |Returns index number of the last time a character or set of characters is found within the string|
|substring()|Returns characters found between two index numbers where the character for the first index number is included and the character for the last index number is not included|
|split()|When a character is specified, it splits the string each time it is found, then stores each individual part in an array|
|trim()|Removes whitespace from start and end of string|
|replace()|Like find and replace, it takes one value that should be found, and another to replace it (by default, it only replaces the first match it finds)|

SIMPLE OR PRIMITIVE DATA TYPES
JavaScript has five simple (or primitive) data types:

1. String
2. Number
3. Boolean
4. Undefined (a variable that has been declared, but
no value has been assigned to it yet)
5. Null (a variable with no value - it may have had
one at some point, but no longer has a value)

JavaScript also defines a complex data type:
6. 0bject

COMMONLY USED TERMS:

* An integer is a whole number (not a fraction).
* A real number is a number that can contain a fractional part.
* A floating point number is a real number that uses decimals to represent a fraction. The term floating point
refers to the decimal point.
* Scientific notation is a way of writing numbers that are too big or too small to be convenient ly written in
decimal form. For example: 3,750,000,000 can be represented as 3.75 x109 or 3.75e+12.

JavaScript Object Literal

A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

The following demonstrates an example object literal:

var myObject = {
    sProp: 'some string value',
    numProp: 2,
    bProp: false
};
Object literal property values can be of any data type, including array literals, functions, and nested object literals.

## [Object constructor](https://developer.mozilla.org/en-US/docs/Web/JavaScript/ReferenceGlobal_Objects/Object/constructor?retiredLocale=ar)

The constructor property returns a reference to the Object constructor function that created the instance object. Note that the value of this property is a reference to the function itself, not a string containing the function's name.
In JavaScript, a constructor function is used to create objects. For example,

// constructor function
function Person () {
    this.name = 'John',
    this.age = 23
}

// create an object
const person = new Person();

Resources:

1. Javascript_and_jquery_interactive_jon_du

2. duckett_html
