# Basic usage of canvas
* Let's start this tutorial by looking at the < canvas> HTML element itself. At the end of this page, you will know how to set up a canvas 2D context and have drawn a first example in your browser.
* The < canvas> element:

```
<canvas id="tutorial" width="150" height="150"></canvas>
```
* Copy to Clipboard
At first sight a < canvas> looks like the < img> element, with the only clear difference being that it doesn't have the src and alt attributes. Indeed, the < canvas> element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size: if the CSS sizing doesn't respect the ratio of the initial canvas, it will appear distorted.

<img src="https://miro.medium.com/max/1006/0*y7IF3MXZ0BjfUHp7" alt="summary" width="600"/>

* A skeleton template:

```
<!DOCTYPE html>
<html>
  <head>
    <meta charset="utf-8"/>
    <title>Canvas tutorial</title>
    <script type="text/javascript">
      function draw() {
        var canvas = document.getElementById('tutorial');
        if (canvas.getContext) {
          var ctx = canvas.getContext('2d');
        }
      }
    </script>
    <style type="text/css">
      canvas { border: 1px solid black; }
    </style>
  </head>
  <body onload="draw();">
    <canvas id="tutorial" width="150" height="150"></canvas>
  </body>
</html>
```
* A simple example:

```
<!DOCTYPE html>
<html>
 <head>
  <meta charset="utf-8"/>
  <script type="application/javascript">
    function draw() {
      var canvas = document.getElementById('canvas');
      if (canvas.getContext) {
        var ctx = canvas.getContext('2d');

        ctx.fillStyle = 'rgb(200, 0, 0)';
        ctx.fillRect(10, 10, 50, 50);

        ctx.fillStyle = 'rgba(0, 0, 200, 0.5)';
        ctx.fillRect(30, 30, 50, 50);
      }
    }
  </script>
 </head>
 <body onload="draw();">
   <canvas id="canvas" width="150" height="150"></canvas>
 </body>
</html>
```
**Drawing shapes with canvas:**
* The grid:
- Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high.

<img src="https://developer.mozilla.org/en-US/docs/Web/API/Canvas_API/Tutorial/Drawing_shapes/canvas_default_grid.png" alt="summary" width="600"/>

### Drawing paths

Now let's look at paths. A path is a list of points, connected by segments of lines that can be of different shapes, curved or not, of different width and of different color. A path, or even a subpath, can be closed. To make shapes using paths, we take some extra steps:

1. First, you create the path.
2. Then you use drawing commands to draw into the path.
3. Once the path has been created, you can stroke or fill the path to render it.

Here are the functions used to perform these steps:

+ beginPath()
    Creates a new path. Once created, future drawing commands are directed into the path and used to build the path up.
+ Path methods
    Methods to set different paths for objects.

**Applying styles and colors**
* Colors

Up until now we have only seen methods of the drawing context. If we want to apply colors to a shape, there are two important properties we can use:


- fillStyle = color
    Sets the style used when filling shapes.
- strokeStyle = color
    Sets the style for shapes' outlines. 

## A fillStyle example

 ```
 function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  for (var i = 0; i < 6; i++) {
    for (var j = 0; j < 6; j++) {
      ctx.fillStyle = 'rgb(' + Math.floor(255 - 42.5 * i) + ', ' +
                       Math.floor(255 - 42.5 * j) + ', 0)';
      ctx.fillRect(j * 25, i * 25, 25, 25);
    }
  }
}
```
<img src="https://cdn.mos.cms.futurecdn.net/S5bicwPe8vbP9nt3iwAwwi.jpg" alt="summary" width="600"/>

## Drawing text

The canvas rendering context provides two methods to render text:

`fillText(text, x, y [, maxWidth])`

`strokeText(text, x, y [, maxWidth])`

## Styling text

the canvas:

+ font = value
    The current text style being used when drawing text. This string uses the same syntax as the CSS font property. The default font is 10px sans-serif.

+ textAlign = value
    Text alignment setting. Possible values: start, end, left, right or center. The default value is start.

+ textBaseline = value
 Baseline alignment setting. Possible values: top, hanging, middle, alphabetic, ideographic, bottom. The default value is alphabetic.

*Advanced text measurements*

In the case you need to obtain more details about the text, the following method allows you to measure it.

`measureText()`
    Returns a TextMetrics object containing the width, in pixels, that the specified text will be when drawn in the current text style. 

```
    function draw() {
  var ctx = document.getElementById('canvas').getContext('2d');
  var text = ctx.measureText('foo'); // TextMetrics object
  text.width; // 16;
}
```

visit this link for more information :
   [Vedio](https://www.w3schools.com/ai/ai_chartjs.asp)