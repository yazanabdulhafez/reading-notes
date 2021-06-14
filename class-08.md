# More CSS Layout
CSS treats each HTML element as if it is in its
own box. This box will either be a block-level
box or an inline box.
CSS has the following positioning schemes that allow you to control
the layout of a page: normal flow, relative positioning, and absolute
positioning. You specify the positioning scheme using the position
property in CSS. You can also float elements using the float property.

1. Normal flow
Every block-level element
appears on a new line, causing
each item to appear lower down
the page than the previous one.
Even if you specify the width
of the boxes and there is space
for two elements to sit side-byside,
they will not appear next
to each other. This is the default
behavior (unless you tell the
browser to do something else).

2. Relative Positioning
This moves an element from the
position it would be in normal
flow, shifting it to the top, right,
bottom, or left of where it
would have been placed. This
does not affect the position of
surrounding elements; they stay
in the position they would be in
in normal flow.

3. Absolute positioning
This positions the element
in relation to its containing
element. It is taken out of
normal flow, meaning that it
does not affect the position
of any surrounding elements
(as they simply ignore the
space it would have taken up).
Absolutely positioned elements
move as users scroll up and
down the page.

* Fixed positioning is a type
of absolute positioning that
requires the position property
to have a value of fixed.

* The float property allows you
to take an element in normal
flow and place it as far to the
left or right of the containing
element as possible.

* The clear property allows you
to say that no element (within
the same containing element)
should touch the left or righthand
sides of a box. It can take
the following values:

1. left
The left-hand side of the box
should not touch any other
elements appearing in the same
containing element.

2. right
The right-hand side of the
box will not touch elements
appearing in the same containing
element.

3. both
Neither the left nor right-hand
sides of the box will touch
elements appearing in the same
containing element.

4. none
Elements can touch either side

Another properties:
* width
This sets the width of the
columns.
* float
This positions the columns next
to each other.
* margin
This creates a gap between the
columns.

## Resolution
refers to the number of dots a screen shows per inch. Some
devices have a higher resolution than desktop computers and most
operating systems allow users to adjust the resolution of their screens.

Because screen sizes and display resolutions vary so much, web
designers often try to create pages of around 960-1000 pixels wide
(since most users will be able to see designs this wide on their screens).

Fixed width layout
designs do not
change size as the
user increases
or decreases
the size of their
browser window.
Measurements tend
to be given in pixels.

Liquid layout designs stretch and contract as the user increases or decreases the
size of their browser window. They tend to use percentages.

### Grids

![css grids](https://webkit.org/wp-content/uploads/grid-concepts.svg)
Grids set consistent proportions
and spaces between items which
helps to create a professional
looking design.

### CSS frameworks

![wireframe in css](https://i.stack.imgur.com/RRixc.png)

 aim to make your life easier by providing the code for
common tasks, such as creating layout grids, styling forms, creating
printer-friendly versions of pages and so on.

* You can include multiple CSS files in one page.

### Resources used in this reading

1. duckett_html

2. <https://www.w3schools.com/css/default.asp>
