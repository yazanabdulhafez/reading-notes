# [HTML Lists](https://www.w3schools.com/html/html_lists.asp), CSS Boxes, JS Control Flow

There are lots of occasions when we need to use lists. HTML provides us with three different types:

* Ordered lists are lists where each item in the list is numbered. For example, the list might be a set of steps fora recipe that must be performed in order, or a legal contract where each point needs to be identified by a section
number.

* Unordered lists are lists that begin with a bullet point (rather than characters that indicate order).

* Definition lists are made up of a set of terms along with the definitions for each of those terms.

![types of lists](https://disenowebakus.net/en/images/articles/html-lists-without-order-ul-ordinates-ol-definition-dl.jpg)

* `<ol>`: The ordered list is created with the `<ol>` element.

* `<li>`: Each item in the list is placed between an opening `<li>` tag and a closing `</li>` tag. (The li stands for list item).

* `<ul>`: The unordered list is created with the `<ul>` element.

* The definition list is created with the `<dl>` element and usually consists of a series of terms and their definitions.
Inside the `<dl>` element you will usually see pairs of `<dt>` and `<dd>` elements.

* `<dt>`: This is used to contain the term being defined (the definition term).

* `<dd>`: This is used to contain the definition.

You can put a second list inside an `<li>` element to create a sublist or nested list.

CSS treats each HTML element as if it has its own box.

The border property allows you to specify the width, style and color of a border in one property (and the values should be coded in that specific order).

The padding property allows you to specify how much space should appear between the content of an element and its border.

The margin property controls the gap between boxes. Its value is commonly given in pixels, although you may also use
percentages or ems.

The display property allows you to turn an inline element into a block-level element or vice versa, and can also be used to hide an element from the page.
The values this property can take are:

1. inline:
This causes a block-level element to act like an inline element.

2. block:
This causes an inline element to act like a block-level element.

3. inline-block:
This causes a block-level element to flow like an inline element, while retaining other features of a block-level element.

4. none:
This hides an element from the page. In this case, the element acts as though it is not on the page at all (although a user could still see the content of the box if they used the view source option in their browser).

The visibility property allows you to hide boxes from users but It leaves a space where the element would have been.

The box-shadow property allows you to add a drop shadow around a box.

The border-image property applies an image to the border of any box. It takes a background image and slices it into nine
pieces.

* You can use CSS to control the dimensions of a box.

* You can also control the borders, margin and padding for each box with CSS.
* It is possible to hide elements using the display and visibility properties.
* Block-level boxes can be made into inline boxes, and inline boxes made into block-level boxes.
* Legibility can be improved by controlling the width of boxes containing text and the leading.
* CSS3 has introduced the ability to create image borders and rounded borders.

------
An array is a special type of variable. It doesn't just store one value; it stores a list of values.

You create an array and give it a name just like you would anyother variable (using the var keyword followed by the name ofthe array).
The values are assigned to the array inside a pair of square brackets, and each value is separated by a comma. The
values in the array do not need to be the same data type, so you can store a string, a number and a Boolean all in the same array.

Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).

To access a value from an array, after the array name you specify the index number for that value inside square brackets.
You can change the value of an item an array by selecting it and assigning it a new value just as you would any other variable(using the equals sign and the new value for that item).

------

## [Control Flow](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Control_flow_and_error_handling?retiredLocale=ar)

An if ... else statement runs one set of code if the condition is true or a different set if it is false.

![ifcond img](https://www.bookofnetwork.com/images/javascript-images/JS_else()_24Feb17_1750.png)

A switch statement starts with a variable called the switch value.Each case indicates a possible value for this variable and the code that should run if the variable matches that value.

![the switch img](https://www.bookofnetwork.com/images/javascript-images/JS_else()_24Feb17_1750.png)

JavaScript can convert data types behind the scenes to complete an operation. This is known as type coercion.

JavaScript is said to use weak typing because the data type for a value can change. Some other languages require that you
specify what data type each variable will be. They are said to use strong typing.

break
This keyword causes the termination of the loop and tells the interpreter to go onto the next statement of code outside
of the loop.

continue
This keyword tells the interpreter to continue with the current iteration, and then check the condition again. (If it is true, the code runs again.)

A for loop is often used to loop through the items in an array.

![for loop](https://www.bookofnetwork.com/images/javascript-images/JS_For-loop-example_20Sep16_1241.png)

The loop starts with the for keyword, then contains the condition inside the parentheses. As long as the counter is less
than the total number of items in the array, the contents of the curly braces will continue to run. Each time the loop runs, the round number is increased by 1.

Inside the curly braces are rules that write the round number and the score to the msg variable. Thevariables declared outside of the loop are used within the loop.

The key difference between a while loop and a do while loop is that the statements in the code block come before the
condition. This means that those statements are run once whether or not the condition is met.

![while loop](https://www.bookofnetwork.com/images/javascript-images/JS_While-loop-example_20Sep16_1243.png)

## The recourses used in this file

1. Duckett HTML book.

2. Duckett JS book.

3. different sites for pictuers.
