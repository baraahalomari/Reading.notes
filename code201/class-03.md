# HTML Lists
HTML lists allow web developers to group a set of related items in lists.
## Unordered HTML List
An unordered list starts with the &lt;ul> tag. Each list item starts with the &lt;li> tag.


The list items will be marked with **bullets**

## Ordered HTML List
An ordered list starts with the &lt;ol> tag. Each list item starts with the &lt;li> tag.


The list items will be marked with numbers
## Definition Lists
The defnition list starts with the &lt;dl> tag. Each list item starts with &lt;dt> and &lt;dd> tag.


and we can put a second list inside &lt;li> tag to create a nested list.


# BOXES
All HTML elements can be considered as boxes.To set dimensions for a box we can use the height and width properties.

There are several wayes to specify the size of a box :

* use pixels 
* percentages 
* ems
" you can use the max-width property to ensure that lines of text do not
appear too wide within a big browser window and you can
use the min-width property to make sure that they do not
appear too narrow"

## overflowing content

**overflow :** that property tells the browser what to do if the content is larger than the box, it have two value :

>hidden: to hides any extra content that doesn't fit in the box.

>scroll: allows the user scroll to see the missing content.

**Border :** The border separates the edge of one box from another
the *border-width* property is used to control the width of a border. The value of this
property can be given in pixels or using one of the following values:

> thin   
> medium    
> thick   


and You can control the style of a border using the border-style property. by this values:

> solid, dotted, dashed, double, groove, ridge, inset, outset.

if we put *hidden* or *none* there are no border is shown
to control of the border put **border-color: color;**


**Margin :** To create a gap between the borders of two boxes.

**Padding :** is the space between the border of a box and any content contained with it.The value of this property is most often specifed in pixels.


we can put the box in the center by  set a width for the box,  setting the left and right margins to auto will make the browser put an equal gap on each side of the box .


## Border images

The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces.

the possible values are:

* stretch: stretches the image
* repeat: repeats the image
* round: like repeat but if the tiles do not ft exactly, scales
the tile image so they will.


**box-shadow :** The box-shadow property allows to add a drop shadow around a box. 

**rounded corners :** create rounded corners on any box, using a property called *border-radius.* The value indicates the size of the radius in pixels.

**Elliptical shaps :** to specify different distances for the horizontal and the vertical parts of the rounded corners.


# Javascript 

creating an array :

> **Array literal:** declerate a variable and give it a name , this value  are assigned to the array inside a pair of square
brackets, and each value is separated by a comma.

coffeebreack= ['tea',

'coffee',

'nescafea'];

> **Array constructor :** This uses the new keyword followed by *Array();* The values are then specified in parentheses, and each value is separated by a comma.

Values in an array are accessed as if they are in a numbered list.

Each item in an array is automatically given a number called an index,
 the numbering of this list starts at zero (not one).

Each array has a property called length, which holds the number of items in the array



## IF...ELSE STATEMENTS


To checks a condition if it true the first code is executed if false the second code is run insted.

the statements inside an if statement should be followed by a semicolon, but
there is no need to place one after the closing curly brace of
the code blocks.

## Switch statement

A switch statement allows a variable to be tested for equality against a list of values. Each value is called a **case**.

"how it works:


* The switch expression is evaluated once.
* The value of the expression is compared with the values of each case.
* If there is a match, the associated block of code is executed.
* If there is no match, the default code block is executed. "

## Data type

string : text

number: numbers

Boolean: true or false

null: empty value

undefined : Variable has been declared but not yet assigned a value.


> Falsy values can also be treated as the number 0.

>Truthy values can also be treated as the number 1.

 > null and undefined are both falsy, they are not equal to anything other than themselves.

> NaN is considered falsy



## LOOPS

loops check a condition, if it true the code will run, the condition keep checking until  it returns false.

### Types of loops:

**for :** to run the code a specific number of times.
**while :** if we don't know how many times the code should run.
 


