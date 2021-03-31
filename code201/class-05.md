# Images

To organized our website we should keeping images in a separate folder,and we can called it **images** also we can add subfolders inside the images folder.


Images should...

>Be relevant

>Convey information

>Convey the right mood

>Be instantly recognisable

>Fit the color palette



## Adding images 

we  need to use an &lt;img> element. **src**  tells the browser where it can find the image file. This will usually be a relative URL pointing to an image in our site. **alt**  This provides a text description of the image which describes the image if we cannot see it.


## specific height & width of images

**There are other attributes that specify images size :**

*height :*This specifes the height of the image in pixels.

*width :*This specifes the width of the image in pixels.


### Where to place images in code ?

1: before a paragraph

2: InsIde the start of a paragraph

3: In the mIddle of a paragraph


### whate the importante of that?

because browsers show HTML elements in one of two ways:

* Block elements always appear on a new line. 

* Inline elements sit within a block level element and do not
start on a new line. 

## align:
 indicate how the other parts of a page should ﬂow around an image.

The align attribute can take these horizontal value:
> left or right


There are three values that the align attribute can take that
control how the image should align vertically with the text that
surrounds it:

> top, middle and bottom.


## Rules of images :

there are three rules for cretind images:

* save images in the right formate
* save images at the right size
* use the correct resolution

to edit and save images, The most popular tool amongst
web professionals is **Adobe Photoshop**.

### Images resolution

Images created for the web should be saved at a resolution of 72 ppi. The higher the resolution of the image, the larger the size of the file.


**Vector images**

Vector images differ from bitmap images and are resolution-independent. Vector images are commonly created in programs such as Adobe Illustrator.


**Animated GIFS**

Animated GIFs show several frames of an image in sequence and therefore can be used to create simple animations.


**Transparency**

Creating an image that is partially transparent  for the web involves
selecting one of two formats: Transparent GIF & PNG.


# color 

The color property allows you to specify the color of text inside
an element. You can specify any color in CSS in one of three ways:

* **rgb values**

These express colors in terms of how much red, green and
blue are used to make it up. For example: rgb(100,100,90).

* **hex Codes**

These are six-digit codes that represent the amount of red, green and blue in a color, preceded by a pound or hash # sign.

* **Color names**

There are 147 predefned color names that are recognized by browsers.


### Background-color 

background-color property sets the color of the background
for that box it is appear in . 
**Contrast**

When picking foreground and background colors, it is important to ensure that there is enough contrast for the text to be legible.

we can reduce contrast by using dark gray text on a white
background or an off-white text on a dark background.


**Opacity :**

allows you to specify the opacity of an element and any of its child elements.
The value is a number between 0.0 and 1.0 (so a value of 0.5 is 50% opacity and 0.15 is 15% opacity).


### hsl, hsla

The value of the property starts with the letters hsl, followed by individual values inside parentheses for:

**hue** 

This is expressed as an angle (between 0 and 360 degrees).

**saturation**

This is expressed as a percentage.

**lightness**

This is expressed as a percentage with 0% being white, 50% being normal, and 100%
being black

**alpha**

This is expressed as a number between 0 and 1.0. For example, 0.5 represents
50% transparency, and 0.75 represents 75% transparency.


# Text

"The properties that allow you to control
the appearance of text can be split into
two groups:

● Those that directly affect the font and its appearance
(including the typeface, whether it is regular, bold or italic,
and the size of the text)

● Those that would have the same effect on text no matter
what font you were using (including the color of text and
the spacing between words and letters)"


## Typeface Terminology

When choosing a typeface, it is important to understand that a browser will usually only display it if it's installed on that user's computer.

* serif 
* sans-serif
* Monospace 
* cursive 
* fantasy

### Techniques That offer a Wider choice of TypefaceS:

* **font-family :** to specify the typeface that should be used for
any text inside the element(s) to which a CSS rule applies.

* **font-size :** to specify a size for the font. (pixels, percentage, ems).

* **font-face :** allows you to use a font, even if it is not installed
on the computer of the person browsing, by allowing you to specify a path to a copy of the font, which will be downloaded if it is not on the user's machine.

* **font-weight :**  to create bold text.

There are two values that this
property commonly takes:(normar or bold)

* **font-style :** There are three values this property can take:(normal, italic, oblique)

* **text-transform :** used to change the case of text giving it one of the following values (uppercase, lowercase, capitalize)

* **text-decoration :** under line and strike ( none, underline, overline, line-through, blink)

* **text-align :** to control the alignment of text. The property can take one
of four values:(left, right, center, justify)

* **text-indent :**  to indent the first line of text within an element.

The amount you want the line indented by can be specifed in
a number of ways but is usually given in pixels or ems.

* **text-shadow :**  to create a drop shadow, which is a dark version
of the word just behind it and slightly offset. It can also be used
to create an embossed effect by adding a shadow that is slightly
lighter than the text.



