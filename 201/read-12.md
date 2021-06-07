# Chart.js, Canvas

## Charts.Js

![chart.js](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQtYtCyxLyC-xC8XFNG1JQnw8pLQTJ5AyiHkNRvZJP6jg710BgkO5XZvAFpRGBdm-bhHAo&usqp=CAU)

Charts are far netter for displaying data visually than tables,they’re easier to look at and convey data quickly, but they’re not always easy to create.

A great way to get started with Chart.js, a JavaSript plugin that uses HTML5 `<canvas>` element to draw the graph onto the page.

## Setting up

The first thing we need to do is download Chart.js. Copy the Chart.min.js out of the unzipped folder and into the directory you’ll be working in. Then create a new html page and import the script:

```html
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
```

## Drawing a line chart

![lineC](https://i.stack.imgur.com/SY5hu.png)

To draw a line chart, the first thing we need to do is create a canvas element in our HTML in which Chart.js can draw our chart. So add this to the body of our HTML page:

```html
<canvas id="buyers" width="600" height="400"></canvas>

<!-- Next, we need to write a script that will retrieve the context of the canvas, so add this to the foot of your body element: -->

<script>
    var buyers = document.getElementById('buyers').getContext('2d');
    new Chart(buyers).Line(buyerData);
</script>
```

## Drawing a pie chart

![pieC](https://user-images.githubusercontent.com/4536038/44617385-2caea980-a859-11e8-9e15-5cfc83f15aec.png)

Our line chart is complete, so let’s move on to our pie chart. First, we need the canvas element:

```html
<canvas id="countries" width="600" height="400"></canvas>

<!-- Next, we need to get the context and to instantiate the chart: -->

var countries= document.getElementById("countries").getContext("2d");
new Chart(countries).Pie(pieData, pieOptions);
```

## Drawing a bar chart

![barC](https://wpdatatables.com/wp-content/uploads/2019/12/Selection_9991912.png)

Finally, let’s add  a bar chart to our page. Happily the syntax for the bar chart is very similar to the line chart we’ve already added. First, we add the canvas element:

```html
<canvas id="income" width="600" height="400"></canvas>

<!-- Next, we retrieve the element and create the graph: -->
<script>
var income = document.getElementById("income").getContext("2d");
new Chart(income).Bar(barData);
</script>

<!-- And finally, we add in the bar chart’s data: -->

<script>
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
</script>

```

## Usage of canvas

![canvas](https://i2.wp.com/www.csscodelab.com/wp-content/uploads/2020/03/javascript-html5-canvas-animated-background.png?fit=1147%2C727&ssl=1)

At first sight a `<canvas>` looks like the `<img>` element, with the only clear difference being that it doesn’t have the src and alt attributes. Indeed, the `<canvas>` element has only two attributes, width and height. These are both optional and can also be set using DOM properties. When no width and height attributes are specified, the canvas will initially be 300 pixels wide and 150 pixels high. The element can be sized arbitrarily by CSS, but during rendering the image is scaled to fit its layout size.

```html

<canvas id="stockGraph" width="150" height="150">
  current stock price: $3.15 + 0.15
</canvas>

<canvas id="clock" width="150" height="150">
  <img src="images/clock.png" width="150" height="150" alt="" />
</canvas>

```

## canvas shape

![shape](https://lh3.googleusercontent.com/proxy/VJ0gNXCBrBj3zfGTum6Y1DsQQfWnHcfcjELbaoshaLxiR2j_hmFRObK-WVKVRiyquUpqFmlANTuL32Qmp5Y75fw)

Before we can start drawing, we need to talk about the canvas grid or coordinate space. Our HTML skeleton from the previous page had a canvas element 150 pixels wide and 150 pixels high. To the right, you see this canvas with the default grid overlayed. Normally 1 unit in the grid corresponds to 1 pixel on the canvas. The origin of this grid is positioned in the top left corner at coordinate (0,0). All elements are placed relative to this origin. So the position of the top left corner of the blue square becomes x pixels from the left and y pixels from the top, at coordinate (x,y). Later in this tutorial we’ll see how we can translate the origin to a different position, rotate the grid and even scale it, but for now we’ll stick to the default.

## canvas text

![text](https://www.webfx.com/blog/images/assets/images.sixrevisions.com/2010/10/03-01_html5_canvas_element_ld_img.png)

The canves rendering context provides two methods to render text.

`fillText(text,x,y[, ,axWidth]` Fills a given text at the given (x,y) position, Optionally with a maximum width to draw, it will Appeare as a filled Text

`strokeText (text,x,y [,maxWidth]` Strokes a given text at the given (x,y) position, Optionally with a maximum width to draw, it will appear as a non-filled text.

