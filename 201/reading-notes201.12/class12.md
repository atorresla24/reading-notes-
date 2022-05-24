# Class 12 reading notes

## Chart.js

Example to creating a chart:
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <!-- import plugin script -->
        <script src='Chart.min.js'></script>
    </head>
    <body>
        <!-- line chart canvas element -->
        <canvas id="buyers" width="600" height="400"></canvas>
        <!-- pie chart canvas element -->
        <canvas id="countries" width="600" height="400"></canvas>
        <!-- bar chart canvas element -->
        <canvas id="income" width="600" height="400"></canvas>
        <script>
            // line chart data
            var buyerData = {
                labels : ["January","February","March","April","May","June"],
                datasets : [
                {
                    fillColor : "rgba(172,194,132,0.4)",
                    strokeColor : "#ACC26D",
                    pointColor : "#fff",
                    pointStrokeColor : "#9DB86D",
                    data : [203,156,99,251,305,247]
                }
            ]
            }
            // get line chart canvas
            var buyers = document.getElementById('buyers').getContext('2d');
            // draw line chart
            new Chart(buyers).Line(buyerData);
            // pie chart data
            var pieData = [
                {
                    value: 20,
                    color:"#878BB6"
                },
                {
                    value : 40,
                    color : "#4ACAB4"
                },
                {
                    value : 10,
                    color : "#FF8153"
                },
                {
                    value : 30,
                    color : "#FFEA88"
                }
            ];
            // pie chart options
            var pieOptions = {
                 segmentShowStroke : false,
                 animateScale : true
            }
            // get pie chart canvas
            var countries= document.getElementById("countries").getContext("2d");
            // draw pie chart
            new Chart(countries).Pie(pieData, pieOptions);
            // bar chart data
            var barData = {
                labels : ["January","February","March","April","May","June"],
                datasets : [
                    {
                        fillColor : "#48A497",
                        strokeColor : "#48A4D1",
                        data : [456,479,324,569,702,600]
                    },
                    {
                        fillColor : "rgba(73,188,170,0.4)",
                        strokeColor : "rgba(72,174,209,0.4)",
                        data : [364,504,605,400,345,320]
                    }
                ]
            }
            // get bar chart canvas
            var income = document.getElementById("income").getContext("2d");
            // draw bar chart
            new Chart(income).Bar(barData);
        </script>
    </body>
</html>

## Basic Usage

### Canvas Element

* Canvas element is similar to img but it has a width and height attribute rather than a src and alt
* Canvas element supports fallback content
* Canvas creates a fixed-sized drawing surface that exposes one or more rendering contexts
* Method, getContext, is used to obtain the rendering context and its drawing functions

## Drawing shapes with canvas

### Drawing shapes with canvas

* Before starting to draw a canvas grid and coordinate space is needed
* Three functions that draw rectangles:
  - fillRect(x,y, width, height) draws a filled rectangle
  - strokeRect(x,y,width, height) draws a rectangular outline
  - clearRect(x, y, width, height) draws a clear rectangle
* A path is a list of points
begin:
  - beginPath() - creates a new path
  - path methods - methods to set different paths for objects
  - closePath() - adds a straight line to the path
  - stroke() - draws a shape by stroking its outline
  - fill() - draws a solid shape by filling the path's content area
* Next step is calling the methods
* Third step is to call closePath()
Example of drawing a triangle:

function draw() {
  var canvas = document.getElementById('canvas');
  if (canvas.getContext) {
    var ctx = canvas.getContext('2d');

    ctx.beginPath();
    ctx.moveTo(75, 50);
    ctx.lineTo(100, 75);
    ctx.lineTo(100, 25);
    ctx.fill();
  }
}

## Applying styles and colors

Two important properties to apply colors to shapes:
  - fillStyle = color which sets style used when filling shapes
  - strokeStyle = color which sets the style for shapes' outlines
globalAlpha = transparencyValue can determine a shapes' level of opauqe (value can be between 0.0 and 1.0)

Line styles:

lineWidth = value
Sets the width of lines drawn in the future.

lineCap = type
Sets the appearance of the ends of lines.

lineJoin = type
Sets the appearance of the "corners" where lines meet.

miterLimit = value
Establishes a limit on the miter when two lines join at a sharp angle, to let you control how thick the junction becomes.

getLineDash()
Returns the current line dash pattern array containing an even number of non-negative numbers.

setLineDash(segments)
Sets the current line dash pattern.

lineDashOffset = value
Specifies where to start a dash array on a line.

lineJoin property determines how connecting segments curve*
* They can either be round, bevel, or miter

Gradiants can be defined by either being linear, radial, or conic:

createLinearGradient(x1, y1, x2, y2)
Creates a linear gradient object with a starting point of (x1, y1) and an end point of (x2, y2).

createRadialGradient(x1, y1, r1, x2, y2, r2)
Creates a radial gradient. The parameters represent two circles, one with its center at (x1, y1) and a radius of r1, and the other with its center at (x2, y2) with a radius of r2.

createConicGradient(angle, x, y)
Creates a conic gradient object with a starting angle of angle in radians, at the position (x, y).

Color can also be assigned with the method addColorStop(position, color)

Shadows involves four properties:

shadowOffsetX = float
Indicates the horizontal distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.

shadowOffsetY = float
Indicates the vertical distance the shadow should extend from the object. This value isn't affected by the transformation matrix. The default is 0.

shadowBlur = float
Indicates the size of the blurring effect; this value doesn't correspond to a number of pixels and is not affected by the current transformation matrix. The default value is 0.

shadowColor = color
A standard CSS color value indicating the color of the shadow effect; by default, it is fully-transparent black.

## drawing text

Drawing text:

fillText(text, x, y [, maxWidth])
Fills a given text at the given (x,y) position. Optionally with a maximum width to draw.

strokeText(text, x, y [, maxWidth])
Strokes a given text at the given (x,y) position. Optionally with a maximum width to draw.

Styling text:

font = value
The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

textAlign = value
Text alignment setting. Possible values: start, end, left, right or center. The default value is start.

textBaseline = value
Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

direction = value
Directionality. Possible values: ltr, rtl, inherit. The default value is inherit.

## Things I want to know more about

I want to be able to utilize this information to relay information on my websites especially charts