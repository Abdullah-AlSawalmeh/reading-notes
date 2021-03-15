# Chart.js, Canvas

Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with charts is with Chart.js, a JavaScript plugin that uses HTML5’s canvas element to draw the graph onto the page. It’s a well documented plugin that makes using all kinds of bar charts, line charts, pie charts and more, incredibly easy.

# What is HTML Canvas?
The HTML < canvas > element is used to draw graphics, on the fly, via JavaScript.

The < canvas> element is only a container for graphics. You must use JavaScript to actually draw the graphics.

Canvas has several methods for drawing paths, boxes, circles, text, and adding images.

# CHART.JS
Charts are far better for displaying data visually than tables and have the added benefit that no one is ever going to press-gang them into use as a layout tool. They’re easier to look at and convey data quickly, but they’re not always easy to create.

Setting up : The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:
<!DOCTYPE html>
<html lang="en">
    <head>
        <meta charset="utf-8" />
        <title>Chart.js demo</title>
        <script src='Chart.min.js'></script>
    </head>
    <body>
    </body>
</html>


# Required tag
In the Apple Safari implementation, is an element implemented in much the same way  is; it does not have an end tag. However, for to have widespread use on the web, some facility for fallback content must be provided. Therefore, Mozilla’s implementation requires an end tag ().

If fallback content is not needed, a simple <canvas id="foo" ...> will be fully compatible with both Safari and Mozilla – Safari will simply ignore the end tag.

If fallback content is desired, some CSS tricks must be employed to mask the fallback content from Safari (which should render just the canvas), and also to mask the CSS tricks themselves from IE (which should render the fallback content).

# The rendering context
creates a fixed size drawing surface that exposes one or more rendering contexts, which are used to create and manipulate the content shown. We’ll focus on the 2D rendering context. Other contexts may provide different types of rendering; for example, there is a 3D context (“experimental-webgl”) based on OpenGL ES.

The is initially blank, and to display something a script first needs to access the rendering context and draw on it. The canvas element has a DOM method called getContext, used to obtain the rendering context and its drawing functions. getContext() takes one parameter, the type of context.


