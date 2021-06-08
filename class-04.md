# HTML Links, CSS Layout, JS Functions

## [HTML Links](https://www.w3schools.com/html/html_links.asp)

Links are the defining feature of the web because they allow you to move from one web page to another — enabling the
very idea of browsing or surfing.

Links are created using the `<a>` element . Users can click on anything between the opening `<a>` tag and the closing `<a>` tag. You specify which page you want to link to using the href attribute.

Links are created using the `<a>` element which has an attribute called href. The value of the href attribute is the page that you want people to go to when they click on the link.Users can click on anything that appears between the opening
`<a>`tag and the closing `</a>` tag and will be taken to the page specified in the href attribute.

Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files.

* Use the `<a>` element to define a link.
* Use the href attribute to define the link address.
* Use the target attribute to define where to open the linked document.
* Use the `<img>` element (inside `<a>`) to use an image as a link.
* Use the mailto: scheme inside the href attribute to create a link that opens the user's email program.

## [CSS Layout](https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout)

![layout pic](https://sparkbox.com/uploads/article_uploads/cssgrid_codepen_step1.png)

CSS treats each HTML element as if it is in its own box. This box will either be a block-level box or an inline box.
If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.

* `<div>` elements are often used as containing elements to group together sections of a page.
* Browsers display pages in normal flow unless you specify relative, absolute, or fixed positioning.
* The float property moves content to the left or right of the page and can be used to create multi-column
layouts. (Floated items require a defined width).
* Pages can be fixed width or liquid (stretchy) layouts.
* You can include multiple CSS files in one page.

### Floats

Originally for floating images inside blocks of text, the float property became one of the most commonly used tools for creating multiple column layouts on webpages. With the advent of Flexbox and Grid it has now returned to its original purpose, as this article explains.

### Grids

CSS Grid Layout is a two-dimensional layout system for the web. It lets you lay content out in rows and columns, and has many features that make building complex layouts straightforward. This article will give you all you need to know to get started with page layout, then test your grid skills before moving on.

### Responsive design

As more diverse screen sizes have appeared on web-enabled devices, the concept of responsive web design (RWD) has appeared: a set of practices that allows web pages to alter their layout and appearance to suit different screen widths, resolutions, etc. It is an idea that changed the way we design for a multi-device web, and in this article we'll help you understand the main techniques you need to know to master it.

## Functions, Methods, and Objects

![function img](https://www.infragistics.com/community/cfs-filesystemfile/__key/CommunityServer.Blogs.Components.WeblogFiles/dhananjay_5F00_kumar.objectinheritance/3173.pic1.PNG)

In JavaScript, functions are first-class objects, because they can have properties and methods just like any other object. What distinguishes them from other objects is that functions can be called. In brief, they are Function objects.

Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of statements).

The location where you declare a variable will affect where it can be used within your code. If you declare it within a function, it can only be used within that function. This is known as the variable's scope.

* **LOCAL VARIABLES: When a variable is created inside a function using the var keyword, it can only be used in that function.**

* **GLOBAL VARIABLES: If you create a variable outside of a function, then it can be used anywhere within the script. It is called a global variable and has global scope.**

An object is a series of variables and functions that represent something from the world around you.

Objects group together a set of variables and functions to create a model of a something you would recognize from the real world. In an object, variables and functions take on new names.

If a variable is part of an object, it is called a property. Properties te ll us about the object.

If a function is part of an object, it is called a method. Methods represent tasks that are associated with the object.

## How does [pair programming](https://www.codefellows.org/blog/6-reasons-for-pair-programming/) work?

While there are many different styles, pair programming commonly involves two roles: the Driver and the Navigator. The Driver is the programmer who is typing and the only one whose hands are on the keyboard. Handling the “mechanics” of coding, the Driver manages the text editor, switching files, version control, and—of course writing—code. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. The Navigator thinks about the big picture, what comes next, how an algorithm might be converted in to code, while scanning for typos or bugs. The Navigator might also utilize their computer as a second screen to look up solutions and documentation, but should not be writing any code.

## Why pair program?

1. Greater efficiency
2. Engaged collaboration
3. Learning from fellow students
4. Social skills
5. ob interview readiness
6. Work environment readiness

Resources used in this reading.

1. `https://www.w3schools.com/html/html_links.asp`
2. `https://developer.mozilla.org/en-US/docs/Learn/CSS/CSS_layout`
3. Duckett HTML book
4. `https://www.codefellows.org/blog/6-reasons-for-pair-programming/`
5. Duckett JS book
