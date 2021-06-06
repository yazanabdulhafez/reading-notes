# HTML Text, CSS Introduction, and Basic JavaScript Instructions

When creating a web page, you add tags
(known as markup) to the contents of the
page. These tags provide extra meaning
and allow browsers to show users the
appropriate structure for the page.

* Structural markup: the elements that you can use to
describe both headings and paragraphs

* Semantic markup: which provides extra information; such
as where emphasis is placed in a sentence, that something
you have written is a quotation (and who said it), the
meaning of acronyms, and so on

HTML has six "levels" of
headings:
**`<h1>`** is used for main headings
**`<h2>`** is used for subheadings
If there are further sections
under the subheadings then the
**`<h3>`** element is used, and so
on.
To create a paragraph, surround
the words that make up the
paragraph with an opening `<p>`
tag and closing `</p>` tag.
By default, a browser will show
each paragraph on a new line
with some space between it and
any subsequent paragraphs.

By enclosing words in the tags
`<b>` and `</b>` we can make
characters appear bold.

By enclosing words in the tags
`<i>` and `</i>` we can make
characters appear italic.
As you have already seen, the
browser will automatically show
each new paragraph or heading
on a new line. But if you wanted
to add a line break inside the
middle of a paragraph you can
use the line break tag `<br />`.

To create a break between
themes — such as a change of
topic in a book or a new scene
in a play — you can add a
horizontal rule between sections
using the `<hr />` tag.

There are some text elements that are not intended to affect the
structure of your web pages, but they do add extra information to the
pages — they are known as semantic markup.

The use of the`<strong>`
element indicates that its
content has strong importance.

The `<em>` element indicates
emphasis that subtly changes
the meaning of a sentence.

## Introducing CSS
CSS allows you to create rules that specify how the content of
an element should appear.

CSS works by associating rules with HTML elements. These rules govern
how the content of specified elements should be displayed. A CSS rule
contains two parts: a selector and a declaration.

CSS declarations sit inside curly brackets and each is made up of two
parts: a property and a value, separated by a colon. You can specify
several properties in one declaration, each separated by a semi-colon.

The `<link>` element can be used
in an HTML document to tell the
browser where to find the CSS
file used to style the page. It is an
empty element (meaning it does
not need a closing tag), and it
lives inside the `<head>` element.
It should use three attributes:

* href : This specifies the path to the
CSS file (which is often placed in
a folder called css or styles).
* type : This attribute specifies the type
of document being linked to. The
value should be text/css.
* rel : This specifies the relationship
between the HTML page and
the file it is linked to. The value
should be stylesheet.

You can also include CSS rules
within an HTML page by placing
them inside a `<style>` element,
which usually sits inside the
`<head>`element of the page.


* There are many different types
of CSS selector that allow you to
target rules to specific elements
in an HTML document.


|Selector          |    Meaning      |            Example|
|------------------|-----------------|-------------------|
|Universal Selector|Applies to all elements in the document|* {}Targets all elements on the page|

|Type Selector|Matches element names|h1 {} Targets the `<h1>` elements|

|Class Selector|Matches an element whose class attribute has a value that matches the one specified after the period (or full stop) symbol|.note {} |

|ID Selector|Matches an element whose id attribute has a value that matches the one specified after the pound or hash symbol|#introduction {} |
## Java script
**A script is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
Statements should end with a semicolon.**

You should write comments to explain what your code does.
They help make your code easier to read and understand.
This can help you and others who read your code.

A script will have to temporarily
store the bits of information it
needs to do its job. It can store this
data in variables.

## DATA TYPES
1. NUMERIC DATA TYPE
The numeric data type handles
numbers.

2. STRING DATA TYPE
The strings data type consists of
letters and other characters.

3. BOOLEAN DATA TYPE
Boolean data types can have one
of two va lues: true or false.


Here are six rules you must always follow when giving a variable a name:
1. The name must begin with
a letter, dollar sign ($),or an
underscore (_). It must not start
with a number.
2. The name can contain letters,
numbers, dollar sign ($), or an
underscore (_). Note that you
must not use a dash(-) or a
period (.) in a variable name.
3. You cannot use keywords or
reserved words.
4. All variables are case sensitive.
5. Use a name that describes the
kind of information that the
variable stores.
6. If your variable name is made
up of more than one word, use a
capital letter for the first letter of
every word after the first word.

 ## ARRAYS
 An array is a special type of variable. It doesn't
just store one value; it stores a list of values.Values in an array are accessed as if they are in a numbered list. It is important to know that the numbering of this list starts at zero (not one).

## EXPRESSIONS
An expression evaluates into (results in) a single value. Broadly speaking
there are two types of expressions.
1. EXPRESSIONS THAT JUST ASSIGN A
VALUE TO A VARIABLE.
2. EXPRESSIONS THAT USE TWO OR
MORE VALUES TO RETURN A
SINGLE VALUE.

## OPERATORS
Expressions rely on things called operators; they allow programmers to create a single value from one or more values.
* ASSIGNMENT OPERATORS
Assign a value to a variable
color = 'beige';
The value of co 1 or is now beige.

* ARITHMETIC OPERATORS
Perform basic math
area = 3 * 2;
The value of area is now 6.

* STRING OPERATORS
Combine two strings
greeting= 'Hi 1 + 'Mol ly';
The value of greeting is now Hi Molly.


* COMPARISON OPERATORS
Compare two values and return true or fa 1 se
buy = 3 > 5;
The value of buy is false.

* LOGICAL OPERATORS
Combine expressions and return true or fa 1 se
buy= (5 > 3) && (2 < 4);
The value of buy is now true.
## LOOPS
There are also many
occasions where you will
want to perform the same
set of steps repeatedly.

Conditional statements allow your code to make
decisions about what to do next.
Comparison operators (===, ! ==, ==, ! =, <, >, <=, =>)
are used to compare two operands.
Logical operators allow you to combine more than one
set of comparison operators.
if ... else statements allow you to run one set of code
if a condition is true, and another if it is false.
if ...else statement al lows you
to provide two sets of code:
1. one set if the condition evaluates to true.
2. another set if the condition is
false.
## [Why good commit messages matter](https://chris.beams.io/posts/git-commit/)
The contributors to these repositories know that a well-crafted Git commit message is the best way to communicate context about a change to fellow developers (and indeed to their future selves). A diff will tell you what changed, but only the commit message can properly tell you why.
The seven rules of a great Git commit message:
1. Separate subject from body with a blank line.
2. Limit the subject line to 50 characters.
3. Capitalize the subject line.
4. Do not end the subject line with a period.
5. Use the imperative mood in the subject line.
6. Wrap the body at 72 characters.
7. Use the body to explain what and why vs. how.
