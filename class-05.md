# HTML Images; CSS Color & Text

![image tag](https://d2h0cx97tjks2p.cloudfront.net/blogs/wp-content/uploads/sites/2/2020/07/html-images-df.jpg)

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

The color property allows you to specify the color of text inside an element. You can specify any color in CSS in one of three ways:

1. rgb values
These express colors in terms of how much red, green and blue are used to make it up. For example: rgb(100,100,90).
2. hex codes
These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign. For example: #ee3e80.
3. color names
There are 147 predefined color names that are recognized by browsers. For example:
DarkCyan.

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

* Those that directly affect the font and its appearance
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

## [JPEG vs PNG vs GIF — which image format to use and when?](https://blog.imagekit.io/jpeg-vs-png-vs-gif-which-image-format-to-use-and-when-c8913ae3e01d)

### Compression

* JPEG is a lossy compression specification that takes advantage of human perception. It can achieve compression ratios of 1:10 without any perceivable difference in quality.

* PNG is a lossless image format using DEFLATE compression. No data is lost during compression and no compression artefacts are introduced in the image. For this reason, a PNG image would retain higher quality than an image than JPEG and would look a lot sharper, it would also occupy more space on the disk. This makes it unsuitable for storing or transferring high-resolution digital photographs but a great choice for images with text, logos and shapes with sharp edges.

* GIF is also a lossless image format that uses LZW compression algorithm. It was favoured over PNG for simple graphics in websites in its early days because the support of PNG was still growing. Given that PNG is now supported across all major devices and that PNG compression is about 5–25% better than GIF compression, GIF images are now mainly used only if the image contains animations.

### Transparency

In a simple form, transparency indicates something that is completely invisible.
JPEG images don’t support transparency and are hence not usable for such cases.
PNG images support transparency in two ways , GIF is unsuitable for images with transparent backgrounds.

### Colours

There is a significant difference in the number of colours that can be supported by these 3 formats.

* JPEG images can support around 16 million colours. This is what makes them suitable for storing images of natural scenes.

* PNG images mainly have two modes — PNG8 and PNG24. PNG8 can support upto 256 colours whereas PNG24 can handle upto 16 million colours like a JPEG image. GIF images are limited to 256 colours.

* Of these 3 formats, only GIF supports animation. This capability makes GIF format suitable for delivering engaging ads and banners.

#### summary

Use JPEG format for all images that contain a natural scene or photograph where variation in colour and intensity is smooth. Use PNG format for any image that needs transparency or for images with text & objects with sharp contrast edges like logos. Use GIF format for images that contain animations.

REFRENCES:

1. Javascript_and_jquery_interactive_jon_du.

2. duckett_html.
