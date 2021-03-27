
# css :

presentation our web page and make it more attractive .

Block level elements that start a new line like "h1, p"
Inline elements flow within the text and don't start a new line, like "img, em" .

A CSS rule contains two parts: a selector and a declaration.

p { color : red; }

Selectors indicate which element the rule applies to, Declarations indicate how the elements referred to in.
the selector should be styled, is made up of two parts: a property and a value, and are separated by a colon.


we can include CSS rules within an HTML page by placing them inside a  " style element ",
which usually sits inside the head element of the page. and The style element should use
the type attribute to indicate that the styles are specifed in CSS. 
If there are two or more rules that apply to the same element, it is important to understand which will take precedence.


by using the link element on each HTML page of our site to link to the same CSS document. This means that the same code does not need to be repeated in every page (which results in less code and smaller HTML pages) and If you are just creating a single page, put the rules in the same file to keep everything in one place.

# color
The color property allows you to specify the color of text inside an element.
When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible You can reduce contrast by using dark gray text on a white
background or an off-white text on a dark background.

## There are three ways to specify colors in CSS:

RGB values : Values for red, green, and blue are expressed as numbers between 0 and 255 .
hex codes : represent values for red, green, and blue in hexadecimal code .
color names : Colors are represented by predefned names.

## way to specify colors using :
hue : is often represented as a color circle where the angle represents the color, although it may also be shown as a slider with values from 0 to 360.
saturation :  is the amount of gray in a color. Saturation is represented as a percentage. 100% is full saturation and 0% is a shade of gray.
lightness values :  is the amount of white (lightness) or (black darkness) in a color. Lightness is represented as a percentage. 0% lightness is black, 100% lightness is white, and 50% lightness is normal .
alpha :This is expressed as a number between 0 and 1.0.
For example, 0.5 represents 50% transparency, and 0.75 represents 75% transparency