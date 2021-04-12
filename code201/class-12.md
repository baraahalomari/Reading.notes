# Charts

We use charts for displaying data,they’re easier to look at. we create charts using Chart.js JavaScript  it’s simple to 
use and really very flexible, it’s a well documented plugin that makes using all kinds of bar charts, line charts, pie 
charts and more, incredibly easy.


To start using Chart.js :

* download Chart.js
* create a canvas element in our HTML in which Chart.js can draw our chart.
* write a script that will retrieve the context of the canvas
* create our data



# The &lt;canvas> element

It's look like img element but with out src and alt attributes. it has **width** and **height** attributes, 
 to supply an id , this makes it much easier to identify it in a script. The &lt;canvas> element can be styled normally.



## Rendering contexts

 "To display something, a script first needs to access the rendering context and draw on it. The &lt;canvas> element has a method called **getContext()**, used to obtain the rendering context and its drawing functions. **getContext()** takes one parameter, the type of context. "




# Drawing shapes with canvas

 &lt;canvas> only supports two primitive shapes: rectangles and paths,  All other shapes must be created by combining one or more paths. 

 > To create a rectangle we use function **fillRect(x, y, width, height)**



 A path is a list of points, connected by segments of lines that can be of different shapes, curved or not.

To create a path we use function **beginPath()** 




To moves the pen to the coordinates specified by x and y we use **moveTo(x, y)**


For drawing straight lines, use the **lineTo()** method.

To draw arcs or circles, we use the **arc() or arcTo()** methods.




# Applying styles and colors


If we want to apply colors to a shape, there are two important properties we can use: 
> fillStyle and strokeStyle
  
The new value becomes the default for all shapes being drawn from then on.


The miterLimit property determines how far the outside connection point can be placed from the inside connection 
point. If two lines exceed this value, a bevel join gets drawn instead. Note that the maximum miter length is the
 product of the line width measured in the current coordinate system, by the value of this miterLimit property.



## Drawing text


The canvas rendering context provides two methods to render text:


> fillText(text, x, y [, maxWidth])

> strokeText(text, x, y [, maxWidth])


There are some more properties which let you adjust the way the text gets displayed on the canvas:

> font = value

> textAlign = value

>textBaseline = value

>direction = value

