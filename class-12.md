## Reading 12 - June 15 <sup>th</sup>

### Chart.js API
- JavaScript plugin that uses HTML5 canvas element to draw graph 
  - Download Chart.js
  - copy Chart.min.js out of unzipped folder and into working directory
  - create new HTML page and import script
- Line chart
  - create canvas element in HTML
    - **canvas element** used to draw graphics on the go via scripts
  - write a script that will retrieve context of the canvas, add to foot of body element
  - inside same script tage, create data
    - can be object that contains labels for base of chart and datasets
- Pie chart and bar graph
- See details at https://www.webdesignerdepot.com/2013/11/easily-create-stunning-animated-charts-with-chart-js/

### Canvas API

#### Basic Usage

\<canvas id="example" width="200" height="200"\> fallback content \</canvas\>

- if not width height specified, canvas defaults to 300px wide and 150px high
- can be styled like any image, but without any its initially fully transparent
- browsers that dont support canvas will render fallback content
  - can also use image tag as fallback content
- content is blank, to display something you need script to access rendering context and draw on it
  1. var canvas = document.getElementById('example');
  2. var ctx = canvas.getContext('2d');
    - getContext() takes 1 parameter, type of context
    - specifying "2d" gets CanvasRenderingContext2D


#### Drawing shapes with canvas
- *Working with paths is essential when drawing objects onto the canvas*
- **The grid**
  - origin of grid positioned in top left corner, 1 unit is 1 px
    - all elements placed relative to this origin
  - simple to draw rectangles
  - can draw a path and then fill it (like for triangles)
    - moveTo() function is like lifting a pen from one spot and moving to another
    - lineTo() method draws straight line
    - arc() or arcTo() for arcs or circles
    - quadraticCurveTo(cp1x, cp1y, x, y)
    - bezierCurveTo(cp1x, cp1y, cp2y, x, y)
  - **this is the stuff of PacMan!)
- can combine all these for tons of possiblities!
- Path2D object lets you cache drawing commands to play back paths quickly

- See examples here: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes


#### Applying styles and colors
- Can set **fillStyle = color** for filling shapes and **strokeStyle = color** for outline
- Default is black (#000)00)
- Can mess with transparency as well using rgba or globalAlpha = transparencyValue
- Line styles have their own properties
  - lineWidth = value
  - lineCap = type
  - lineJoin = type
  - miterLimit = value
  - getLineDash()
  - setLineDash(segments)
  - lineDashOffset = value
- Can fill and stroke shapes using *linear and radial gradients* as well
  - createLinearGradient(x1, y1, x2, y2)
    - creates linear gradient object with starting point of (x1, y1) and end point of (x2,y2)
  - createRadialGradient(x1, y1, r1, x2, y2, r2)
    - creates radial gradient, parameters represent two circles, one with center at (x1, y1) and radius of r1, other with center at (x2, y2) with radius of r2
- Can use createPattern() method to create a pattern of images, instead of using for loop
- Can create shadows using four properties

- Review this more, LOTS of info: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Applying_styles_and_colors


#### Drawing text
- Can use **fillText(text, x, y [, maxWidth])**
  - fills text at given x,y position
  - optional maximum width to draw
- **strokeText(text, x, y [, maxWidth])**
  - strokes a given text at the given x,y position
- several properties to style text
  - font = value
  - textAlign = value
  - textBaseline = value (this is an interesting one!)
  - more examples here: https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_text



[Back to Home](README.md)