# HTML Images; CSS Color & Text

To add an image into the page you need to use an `<img>` element. This is an empty element (which means there is
no closing tag). It must carry the following two attributes:

1. src : This tells the browser where it can find the image file. This will
 usually be a relative URL pointing to an image on your own site.

2. alt : This provides a text description of the image which describes the image if you cannot see it.

title : You can also use the title attribute with the `<img>` element to provide additional information
about the image. Most browsers will display the content of this attribute in a tootip when the user hovers over the image.

height : This specifies the height of the image in pixels.

width : This specifies the width of the image in pixels

Where an image is placed
in the code will affect how it
is displayed. Here are three
examples of image placement
that produce different results:

1. before a paragraph
The paragraph starts on a new
line after the image.
2. inside the start of a
paragraph
The first row of text aligns with
the bottom of the image.
3. in the middle of a
paragraph
The image is placed between the
words of the paragraph that it
appears in.

The align attribute was
commonly used to indicate how
the other parts of a page should
flow around an image
left
This aligns the image to the left
(allowing text to flow around its
right-hand side).
right
This aligns the image to the right
(allowing text to flow around its
left-hand side).
There are three values that the
align attribute can take that
control how the image should
align vertically with the text that
surrounds it:
top
This aligns the first line of the
surrounding text with the top of
the image.
middle
This aligns the first line of the
surrounding text with the middle
of the image.
bottom
This aligns the first line of the
surrounding text with the bottom
of the image.

You should save images at the size you will be using
them on the web page and in the appropriate format.

* Photographs are best saved as JPEGs; illustrations or
logos that use flat colors are better saved as GIFs.

## [CSS Color](https://developer.mozilla.org/en-US/docs/Web/CSS/color_value)

![colors](https://planet-www.com/ar/wp-content/uploads/2015/07/11.png)

The color property allows you
to specify the color of text inside
an element. You can specify any
color in CSS in one of three ways:
rgb values
These express colors in terms
of how much red, green and
blue are used to make it up. For
example: rgb(100,100,90)
hex codes
These are six-digit codes that
represent the amount of red,
green and blue in a color,
preceded by a pound or hash #
sign. For example: #ee3e80
color names
There are 147 predefined color
names that are recognized
by browsers. For example:
DarkCyan

Color pickers can help you find the color you want.

* It is important to ensure that there is enough contrast
between any text and the background color (otherwise
people will not be able to read your content).
* CSS3 has introduced an extra value for RGB colors to
indicate opacity. It is known as RGBA.
* CSS3 also allows you to specify colors as HSL values,
with an optional opacity value. It is known as HSLA.

## [CSS Text](https://developer.mozilla.org/en-US/docs/Learn/CSS/Styling_text/Fundamentals)

Text Color : The color property is used to set the color of the text.
The Text Background-Color is used to set the color of the Background.
The properties that allow you to control
the appearance of text can be split into
two groups:
Those that directly affect t ●● he font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)

* Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)

* There are properties to control the choice of font, size,
weight, style, and spacing.

* There is a limited choice of fonts that you can assume
most people will have installed.

* If you want to use a wider range of typefaces there are
several options, but you need to have the right license
to use them.

* You can control the space between lines of text,
individual letters, and words. Text can also be aligned
to the left, right, center, or justified. It can also be
indented.

* You can use pseudo-classes to change the style of an
element when a user hovers over or clicks on text, or
when they have visited a link.

REFRENCES:

1. Javascript_and_jquery_interactive_jon_du.

2. duckett_html.
