# Docs for the HTML `<canvas>` Element & Chart.js

![canvas](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors/canvas_radialgradient.png)

Drawing shapes with canvas
The HTML `<canvas>` element is used to draw graphics on a web page.

The graphic to the left is created with `<canvas>`. It shows four elements: a red rectangle, a gradient rectangle, a multicolor rectangle, and a multicolor text.

Canvas Examples

1. A canvas is a rectangular area on an HTML page. By default, a canvas has no border and no content.
The markup looks like this:
`<canvas id="myCanvas" width="200" height="100"></canvas>`
2. Drawing paths: Here are the functions used to perform these steps:
beginPath()
Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
Path methods
Methods to set different paths for objects.
closePath()
Adds a straight line to the path, going to the start of the current sub-path.
stroke()
Draws the shape by stroking its outline.
fill()
Draws a solid shape by filling the path's content area.

## Colors

![colors](https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors/canvas_fillstyle.png)

 If we want to apply colors to a shape, there are two important properties we can use: fillStyle and strokeStyle.

1. fillStyle = color
Sets the style used when filling shapes.
2. strokeStyle = color
Sets the style for shapes' outlines.

### Transparency

In addition to drawing opaque shapes to the canvas, we can also draw semi-transparent (or translucent) shapes. This is done by either setting the globalAlpha property or by assigning a semi-transparent color to the stroke and/or fill style.

globalAlpha = transparencyValue
Applies the specified transparency value to all future shapes drawn on the canvas. The value must be between 0.0 (fully transparent) to 1.0 (fully opaque). This value is 1.0 (fully opaque) by default.

### Line styles

There are several properties which allow us to style lines.

* lineWidth = value
Sets the width of lines drawn in the future.
* lineCap = type
Sets the appearance of the ends of lines.
* lineJoin = type
Sets the appearance of the "corners" where lines meet.
* miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.
* getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.
* setLineDash(segments)
Sets the current line dash pattern.
* lineDashOffset = value
Specifies where to start a dash array on a line.

### Gradients

Just like any normal drawing program, we can fill and stroke shapes using linear, radial and conic gradients. We create a CanvasGradient object by using one of the following methods. We can then assign this object to the fillStyle or strokeStyle properties.

* createLinearGradient(x1, y1, x2, y2)
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).
* createRadialGradient(x1, y1, r1, x2, y2, r2)
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.
* createConicGradient(angle, x, y)
Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

### Patterns

In one of the examples on the previous page, we used a series of loops to create a pattern of images. There is, however, a much simpler method: the createPattern() method.

createPattern(image, type)
Creates and returns a new canvas pattern object. image is a CanvasImageSource (that is, an HTMLImageElement, another canvas, a `<video>` element, or the like. type is a string indicating how to use the image.
The type specifies how to use the image in order to create the pattern, and must be one of the following string values:

* repeat
Tiles the image in both vertical and horizontal directions.
* repeat-x
Tiles the image horizontally but not vertically.
* repeat-y
Tiles the image vertically but not horizontally.
* no-repeat
Doesn't tile the image. It's used only once.

### Shadows

Using shadows involves just four properties:

* shadowOffsetX = float
Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
* shadowOffsetY = float
Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.
* shadowBlur = float
Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.
* shadowColor = color
A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

### Drawing text

The canvas rendering context provides two methods to render text:

* fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.
* strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

## Chart.js

![barchart](https://www.geeksforgeeks.org/wp-content/uploads/Screenshot-from-2018-07-03-12-00-44.png)

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

1. Drawing a line chart

`<canvas id="buyers" width="600" height="400"></canvas>`

* write a script that will retrieve the context of the canvas, so add this to the foot of your body element
`<script>`
    `var buyers = document.getElementById('buyers').getContext('2d');`
    `new Chart(buyers).Line(buyerData);`
`</script>`
* Inside the same script tags we need to create our data, in this instance it’s an object that contains labels for the base of our chart and datasets to describe the values on the chart.

2. Drawing a pie chart

* `<canvas id="countries" width="600" height="400"></canvas>`
* `var countries= document.getElementById("countries").getContext("2d");`
`new Chart(countries).Pie(pieData, pieOptions);`
* Next we need to create the data. This data is a little different to the line chart because the pie chart is simpler, we just need to supply a value and a color for each section
`var pieData = [{ value: 20, color:"#878BB6"},{value:40,color:"#4ACAB4"}];`

3. Drawing a bar chart

* `<canvas id="income" width="600" height="400"></canvas>`
* we retrieve the element and create the graph
`var income = document.getElementById("income").getContext("2d");`
`new Chart(income).Bar(barData);`
* we add in the bar chart’s data
`var barData={labels : ["January","February","March","April","May","June"],`
`datasets : [{fillColor : "#48A497",strokeColor : "#48A4D1",data : [456,479,324,569,``702,600]},{fillColor:"rgba(73,188,170,0.4)",strokeColor:"rgba(72,174,209,0.4)",`
`data:[364,504,605,400,345,320]}]}`

### Resources used in this reading

1. <https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors>
2.<https://www.w3schools.com/html/html5_canvas.asp>
