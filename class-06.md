# Problem Domain, Objects, and the DOM

## Understanding The Problem Domain Is The Hardest Part Of Programming

![problem domain](https://texavi.com/blog/wp-content/uploads/2011/09/Problems_vs_Solutions_Model_TexaviInnovativeSolutions.png)

**If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:**

1. Make the problem domain easier.
2. Get better at understanding the problem domain.

You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

## Objects

Objects group together a set of variables and functions to create a model of a something you would recognize from the 
real world. In an object, variables and functions take on new names.
To access a property of this object, the object name
is followed by a dot (the period symbol) and the name of the property that you want.
Similarly, to use the method , you can use the object name followed by the method name.

### JavaScript Object Literal

A JavaScript object literal is a comma-separated list of name-value pairs wrapped in curly braces. Object literals encapsulate data, enclosing it in a tidy package. This minimizes the use of global variables which can cause problems when combining code.

The following demonstrates an example object literal:

`var myObject = {`
    `sProp: 'some string value',`
    `numProp: 2,`
    `bProp: false`
`};`

### Object Literal Syntax

Object literals are defined using the following syntax rules:

1. A colon separates property name from value.
2. A comma separates each name-value pair from the next.
3. A comma after the last name-value pair is optional.

If any of the syntax rules are broken, such as a missing comma or colon or curly brace, a JavaScript error will be triggered. Browser error messages are helpful in pointing out the general location of object literal syntax errors, but they will not necessarily be completely accurate in pointing out the nature of the error.

### Why and How We Use Object Literals

Several JavaScripts from dyn-web use object literals for setup purposes. Object literals enable us to write code that supports lots of features yet still provide a relatively straightforward process for implementers of our code. No need to invoke constructors directly or maintain the correct order of arguments passed to functions. Object literals are also useful for unobtrusive event handling; they can hold the data that would otherwise be passed in function calls from HTML event handler attributes.

There is one drawback: if you are unfamiliar with the syntax, it can be very easy to introduce errors which cause the code to stop working.

## [Document Object Model](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)

![DOM](https://devopedia.org/images/article/282/9041.1597665465.jpg)


* The browser represents the page using a DOM tree.

* DOM trees have four types of nodes: document nodes,
element nodes, attribute nodes, and text nodes.

* You can select element nodes by their id or class
attributes, by tag name, or using CSS selector syntax.

* Whenever a DOM query can return more than one
node, it will always return a Nadel i st.

* From an element node, you can access and update its
content using properties such as textContent and
innerHTML or using DOM manipulation techniques.

* An element node can contain multiple text nodes and
child elements that are siblings of each other.

* In older browsers, implementation of the DOM is
inconsistent (and is a popular reason for using jQuery).
Browsers offer tools for viewing the DOM tree.

![DOM](https://vikaswebclasses.com/wp-content/uploads/2020/11/screenshot-www.youtube.com-2020.11.03-16_08_39-768x354.png)

### Resources used in this reading

1. Javascript_and_jquery_interactive_jon_du.
2. <https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction>.
3. <http://dyn-web.com/tutorials/object-literal/>.
