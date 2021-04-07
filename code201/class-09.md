# Form
A printed document that contains spaces for you to fill in information Whenever you want to collect information from
visitors, which lives inside a <form> element.

**There are several types of form controls :**
* adding text
* making choices
* uploading files

&lt;form>: This element should always carry the action attribute and will usually have a
method and id attribute too, Forms can be sent using one of two methods: **get** or **post**.
&lt;input> : is used to create several different form controls. The value of the type
attribute determines what kind of input they will be creating.

**type="oassword"**

When the type attribute has a value of password it creates a text box that acts just like a
single-line text input, except the characters are blocked out.

They are hidden in this way so that if someone is looking over the user's shoulder, they cannot
see sensitive data such as passwords.

**type="radio"**

Radio buttons allow users to pick just one of a number of options.

**type="checkbox"**

Checkboxes allow users to select  one or more options in answer to a question.

**type="file"**

This type of input creates a box that looks like a text input followed by a browse button.

When the user clicks on the browse button, a window opens up that allows them to select a
file from their computer to be uploaded to the website.



The &lt;select> : is used to create a drop down list box. It contains two or more &lt;option>
elements.


The &lt;button> : to allow users more control over how their buttons appear, and to allow other
elements to appear inside the button.



# Lists, Tables and forms


The list-style-type property allows you to control the shape or style of a bullet point .
It can be used on rules that apply to the &lt;ol>, &lt;ul>, and &lt;li> elements.

**Unordered Lists:** 

(none, disc, circle, square)
**Ordered Lists:**

(decimal, decimal-leading-zero, lower-alpha, upper-alpha, lower-roman, upper-roman)

**list-style-image:**

You can specify an image to act as a bullet point using the list-style-image property.

**list-style-position:**

This property can take one of two values:

> outside

The marker sits to the left of the block of text.

> inside

The marker sits inside the box of text.

**list-style:**

it allows you to express the markers' style, image and position properties in any order.


# Table

properties that used with tables:

* width :to set the width of the table.

* padding: to set the space between the border of each table cell and its content.

* text-transform :to convert the content of the table headers to uppercase.

* letter-spacing, font-size : to add additional styling to the content of the table headers.

* border-top, border-bottom: to set borders above and below the table headers.

* text-align : to align the writing to the left of some table cells and to the right of the others.

* background-color:  to change the background color of the alternating table rows.

* :hover : to highlight a table row when a user's mouse goes over it.


The border-spacing property allows you to control the distance between adjacent cells.
By default, browsers often leave a small gap between each table cell, so if you want to increase
or decrease this space then the border-spacing property allows you to control the gap.


# Forms

If you can make yours look more attractive and easier to use, more people are likely to fill it in. Also, when you
come to look at a form in a few different browsers , you will see that each browser displays them differently.

* font-size : sets the size of the text entered by the user.

* color :sets the text color.

* background-color :sets the background color of the input.
* border: adds a border around the edge of the input box.
* border-radius : can be used to create rounded corners.


# Events

Types of events that occur in the browser :

>load : Web page has finished loading

>unload: Web page is unloading 

>error: Browser encounters a JavaScript error or an asset doesn't exist

>resize: Browser window has been resized

>scroll: User has scrolled up or down the page


When an event has occurred, it is often described as having fired or been raised. if the user is tapping on a link, a
click event would fire in the browser.

* **focus / focus** in  Element gains focus


* **blur / focusout**  Element loses focus



**Event handling**

there are three steps involved in getting it to trigger some JavaScript code.

**Together these steps:**

1 Select t he element node(s) you want the script to respond to.

2 Indicate which event on the selected node(s) will trigger the response.

3 State the code you want to run when the event occurs.

**Binding:** is the process of stating which event you are waiting to happen, and which element you are waiting
for that event to happen upon.

When an event occurs on an element, it can trigger a JavaScript function. When this function then changes
the web page in some way, it feels interactive because it has responded to the user.

The most commonly used events are W3C DOM events, although there are others in the HTMLS
specification as well as browser-specific events.

