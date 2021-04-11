# IMAGES

we can control the size of an image using the width and height properties in CSS.Specifying image sizes helps
pages to load more smoothly, we can use CSS to control the dimensions of the images, instead of putting the
dimensions in the HTML.

**There are two ways that this is commonly achieved:**

* The float property is added to the class that was created to represent the size of the image.
* New classes are created with names such as align-left or align-right to align the images to the left or right of the page.

**There are two common ways in which we can horizontally center an image:**

* On the containing element, we can use the text-align property with a value of center.
* On the image itself, we can use the use the margin property and set the values of the left and
right margins to auto.

The background-image property allows us to place an image behind any HTML element. 

p {

background-image: url("path of img or url");
}

**The background-repeat property can have four values:**

> repeat

>repeat-x

>repeat-y

>no-repeat


When an image is not being repeated, we can use the background-position property to specify where in the
browser window the background image should be placed.


Using CSS, it is possible to create a link or button that changes to a second style when a user moves
their mouse over it  and a third style when they click on it.


The gradient is created using the background-image property and, at the time of writing, different browsers required a
different syntax.

If we want to overlay text on a background image, the image must be low
contrast in order for the text to be legible.


# Search engine optimization (SEO)

Practical Information Search engine optimization SEO is the practice of trying to help our site appear nearer
the top of search engine results when people look for the topics that our website covers,The main component of this is
looking at keywords that people are likely to enter into a search engine if they wanted to find our site, and then including these in the text and HTML code for our site in order to help the search engines know that our site covers these topics.


**There are seven key places where keywords can appear in order to improve its fndability:**

* Page title
*  url / WeB address
* headings
* text
* link text
*  image alt text
* Page descriPtions


When people start coming to our site, we can start analyzing how they found it, what they were looking at and at what point they are leaving.

The traffc sources link on the left hand side allows us to learn where our visitors are
coming from.

In order to put our site on the web we will need a **domain name** and **web hosting**.
Many companies provide platforms for blogging, email newsletters, e-commerce and other popular website
tools .



# Audio and Video Elements

The &lt;video> and &lt;audio> elements allow us to embed video and audio into web pages, the HTMLMediaElement API
 provides features to allow you to control video and audio players programmatically.

Because &lt;audio> elements have the same HTMLMediaElement functionality available to them, you could easily get this player to work for an &lt;audio> element too.

Can you work out a way to turn the timer inner &lt;div> element into a true seek bar/scrobbler — i.e., when you click somewhere on the bar, it jumps to that relative position in the video playback? As a hint, you can find out the X and Y values of the element's left/right and top/bottom sides via the getBoundingClientRect() method,
 and you can find the coordinates of a mouse click via the event object of the click event, called on the Document object.