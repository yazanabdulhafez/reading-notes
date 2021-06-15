# Forms and Events

![form](https://www.htmlgoodies.com/wp-content/uploads/2021/04/HTML-Form.png)

An HTML form is used to collect user input. The user input is most often sent to a server for processing.
The `<form>` element is a container for different types of input elements, such as: text fields, checkboxes, radio buttons, submit buttons, etc.

* Whenever you want to collect information from
visitors you will need a form, which lives inside a
`<form>` element.
* Information from a form is sent in name/value pairs.
* Each form control is given a name, and the text the
user types in or the values of the options they select
are sent to the server.
* HTML5 introduces new form elements which make it
easier for visitors to fill in forms.

## CSS Bordered Inputs

### lists CSS

Different List Item Markers
The list-style-type property specifies the type of list item marker.


An Image as The List Item Marker
The list-style-image property specifies an image as the list item marker

Position The List Item Markers
The list-style-position property specifies the position of the list-item markers (bullet points).

Remove Default Settings
The list-style-type:none property can also be used to remove the markers/bullets. Note that the list also has default margin and padding. To remove this, add margin:0 and padding:0 to `<ul>` or `<ol>`.

List - Shorthand property

The list-style: property is a shorthand property. It is used to set all the list properties in one declaration.

When using the shorthand property, the order of the property values are:

1. list-style-type (if a list-style-image is specified, the value of this property will be displayed if the image for some reason cannot be displayed)
2. list-style-position (specifies whether the list-item markers should appear inside or outside the content flow)
3. list-style-image (specifies an image as the list item marker)

If one of the property values above are missing, the default value for the missing property will be inserted, if any.

### CSS Tables

The following example shows some of the available list item markers
CSS Tables

* Table Borders :To specify table borders in CSS, use the border property.

* Full-Width Table
The table above might seem small in some cases. If you need a table that should span the entire screen (full-width), add width: 100% to the `<table>` element.

The border-collapse property sets whether the table borders should be collapsed into a single border

### Table Padding

To control the space between the border and the content in a table, use the padding property on <td> and <th> elements

Hoverable Table
Use the :hover selector on `<tr>` to highlight table rows on mouse over.

* Use the border property to change the border size and color, and use the border-radius property to add rounded corners:for forms

* Padded Inputs
Use the padding property to add space inside the text field.

Tip: When you have many inputs after each other, you might also want to add some margin, to add more space outside of them

* Colored Inputs
Use the background-color property to add a background color to the input, and the color property to change the text color
* Focused Inputs
By default, some browsers will add a blue outline around the input when it gets focus (clicked on). You can remove this behavior by adding outline: none; to the input.
* Input with icon/image
If you want an icon inside the input, use the background-image property and position it with the background-position property. Also notice that we add a large left padding to reserve the space of the icon

Use the :focus selector to do something with the input field when it gets focus

## Events

Events are the browser's way of indicating when
something has happened (such as when a page has
finished loading or a button has been clicked).

![evwnts](https://cope-ali.github.io/cope-ali261.github.io/img/HTMLevents.png)

Binding is the process of stating which event you are
waiting to happen, and which element you are waiting
for that event to happen upon.

When an event occurs on an element, it can trigger a
JavaScript function. When this function then changes
the web page in some way, it feels interactive because
it has responded to the user.

![events in js](https://cf.ppt-online.org/files1/slide/f/fqUhbIKJBalrm6FYzyjCWpQE4ATOSu1GgHZcv5XN7D/slide-27.jpg)

You can use event delegation to monitor for events
that happen on all of the children of an element.

The most commonly used events are W3C DOM
events, although there are others in the HTMLS
specification as well as browser-specific events.

## Resourses used in this reading

1. the Duckett HTML book
2. Javascript_and_jquery_interactive_jon_du
