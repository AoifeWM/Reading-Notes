# Chart.js, Canvas

Chart.js is a javascript library that lets you easily generate charts using a series of paramaters. It uses the HTML canvas element, which must be first set be set up with an `id`, and a `width` and `height`. To create the chart you select the element by ID from javascript and add `.getContext('2d');` to the end of the `getElementById` tag. Then you call `Chart(your new dom element here).[chart type, Ie 'Line'](one or multiple objects)`. The object(s) need various properties like `labels` and `dataset`. Other properties are `fillColor`, `strokeColor`, `pointColor`, etc. It can make a wide arrary of chart types like pie charts, bar charts, line charts, point charts, etc.

## The canvas element in HTML

Canvas is a powerful HTML element which allows various things to be easily drawn onto it by javascript. It must be initialized with width and height and then selected in JS with DOM manipulation. Once selected, various properties can be edited to draw on it, for instance, `.fillStyle` which chooses the color to draw with and `.fillRect` which allows you to set starting points and dimensions of a rectangle to draw. It has many other useages, such as drawing other shapes and text as well. The possibilities of this tool are nearly endless.
