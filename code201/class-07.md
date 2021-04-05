# Domain Modeling

creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors.
object-oriented:stores data in properties and encapsulates behaviors in methods.

### Model epic fails videos

 build self-contained objects with the same attributes and behaviors. That way, when I need to change the algorithm for determining popularity, the changes will be small and targeted.

the constructor function is defined using a function expression, and When the function is called, the data inside these parameters are stored inside the properties respectively.

### Generate random numbers

To model the random nature of user behavior, you'll need the help of a random number generator. Fortunately, the JavaScript standard library includes a Math.random() function for just this sort of occasion.

 method which is assigned a function with two parameters called **min** and **max**. The function uses both **Math.floor** and **Math.random** to calculate and return a random integer between min and max.

### Calculate daily Likes

the formula for calculating Likes is the number of viewers times the percentage of viewers who'll Like a video. In other words, viewers times percentage.


# Tables

A table represents information in a grid format, Grids allow us to understand complex data by referencing
information on two axes.

## Basic table structure

&lt;table> element : is used to create a table. The contents of the table are written out row by row.

&lt;tr>: the start of each row using the opening &lt;tr> tag, At the end of the row you use a closing &lt;/tr> tag.

&lt;td> : Each cell of a table is represented using a &lt;td> element, At the end of each cell you use a
closing &lt;/td> tag.


### Table headings

The &lt;th> element is used just like the &lt;td> element but its purpose is to represent the
heading for either a column or a row.

### Spaning columns

when a cell extends across more than one column, the &lt;td> or &lt;th> cells that would have been in the
place of the wider cells are not included in the code.

### Spaning row

The rowspan attribute can be used on a &lt;th> or &lt;td> element to indicate how many rows a cell
should span down the table.

## Long tables

There are three elements that help distinguish between the main content of the table and the first and last rows 

* The headings of the table should sit inside the &lt;thead> element

* The body should sit inside the &lt;tbody> element.

* The footer belongs inside the &lt;tfoot> element


### Width & spacing

The width attribute was used on the opening &lt;table> tag to indicate how wide that table
should be and on some opening &lt;th> and &lt;td> tags to specify the width of individual cells.



# Creating an object:

> constructor notation

"using a combination of the new keyword and the object () constructor function.

To update the value of properties, we use dot notation or square brackets.

they work on objects created using literal or constructor notation."


when there are several objects represent similar things, we can use a function as a tamplate for creating object.

## Creating objects using constructor syntax

To access a property of this object, we can use dot notation, just as we can with any object.
and to use the method, we can use the object name followed by the method name.

To delete a property, we use the keyword delete, and then use dot notation to identify the
property or method we want to remove from the object.


> Ways to create objects

* Create the object, then add properties and methods.

* Literal notation

* object constructor notation

* Creating an object with  properties and methods.


## This.

"The keyword this is commonly used inside functions and objects.
Where the function is declared alters what this means. It always refers
to one object, usually the object in which the function operates."


### A method of an object 

When a function is defined inside an object, it becomes a method. In a method, this refers to the containing object.


### Recap: storing data

To organize our data, we can use an array or object to group a set of related values. In arrays and objects the name is also known as a key.


> Browser object model

The Browser Object Model contains objects that represent the current browser window or tab.

> Document object model

it  uses objects to create a representation of the current page. It creates a new object for each element 

> Global javascript objects

it represent things that the JavaScript language needs to create a model of. 

