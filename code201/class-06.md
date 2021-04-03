# Objects 
Objects group together a set of variables and functions to create a model
of a something we would recognize from the real world, **Properties** tell us about the object.

**Methods** represent tasks that are associated with the object.

properties and methods have a *name* and a *value*. In an object, that name is called a key.

The value of a property can be a *string*, *number*, *Boolean*, *array*, or even another object.

* we can access the properties or methods of an object using dot notation.

examble: hotel .checkAvailability()

* and also by using square brackets.


## Document object model

**The Document Object Model (DOM)** specifies how browsers should create a model of an HTML
page and how JavaScript can access and update the contents of a web page while it is in the browser window.

It covers two primary areas:

* making a model of the HTML page.

The DOM specifies the way in which the browser should structure this model using
a DOM tree.

* accessing and changing the HTML page.

which in turn updates what the user sees in the browser.


**DOM tree:** it is stored in the browsers memory. It consists of four main types of nodes.

**The document node:** 
Every element, attribute, and piece of text in the HTML is represented by its own DOM node.

**Element nodes:**
HTML elements describe the structure of an HTML page. (The &lt;hl > - &lt;h6> elements describe what
parts are headings; the &lt;p> tags indicate where paragraphs of text start and finish.

Each node is an object with methods and properties.

Any changes made to the DOM tree are reflected in the browser.

**Attribute nodes:**
Attribute nodes are not children of the element that carries them; they are part of that element. 

**Text nodes:**
Text nodes cannot have children. If an element contains text and another child element, the child
element is not a child of the text node but rather a child of the containing element.


>Accessing and updating the DOM tree

1. Access the elements

2. Work with those elements


**DOM queries:** methods that find elements in the DOM tree, and it  return one element, or they may return a Nodelist,
which is a collection of nodes.


**Groups of element nodes:**

If a method can return more than one node, it will always return a Nodelist, which is a collection of
nodes.

**Fastest route :**

evaluating the minimum number of nodes on the way to the element you want to work with.


* Methods that return a single element node:

> getElementByld(&#x60;id`)

> querySel ector(&#x60;css selector`)

* Methods that return one or more element node:

> getEl ementsByClassName(&#x60;class`)

> getEl ementsByTagName(&#x60;tagName`)

> querySelectorAll (&#x60;css selector`)


**getElementByid() :** allows you to select a single element node
by specifying the value of its id attribute.


**Nodelist :** is a collection of element nodes. Each node is given an index number, they are a
type of object called a collection.


**live Nodelist :** The methods beginning getElementsBy_ return live Nodelists.
 They are also typically faster to generate than static Nodelists.

**static Nodelis :** They reflect the document when the query was made. If the script changes the content
of the page, the Nodelist is not updated to reflect those changes.

### There are two ways to select an element from a Nodelist:

>The item() method and array syntax.

>The getElementsByClassName() method : allows you to select elements whose c1ass attribute contains a specific value.

>The getElementsByTagName() method: allows you to select elements using their tag name.


>querySe1ector() returns the first element node that matches the CSS-style selector.

>querySe1ectorA11() returns a Nodelist of all of the matches.


**Looping through a nodelist:** It involves finding out how many items are in the Nodelist, and
then setting a counter to loop through them, one-by-one.

Each time the loop runs, the script checks that the counter is less than the total number of
items in the Nodelist.


**we can select another element in relation to it using these five properties:**

* parentNode
* previousSibling nextSibling
* firstChild lastChild


### Previous & next sibling

these properties can return inconsistent results in different browsers.using getElementByld ()


**First & last child**

These properties also return inconsistent results if there is whitespace between elements
When we select a text node, you can retrieve or amend the content of it using the nodeVa1ue property.



The textContent property allows us to collect or update just the text that is in the
containing element.

we can use the textContent property on the containing &lt;li > element.


### Adding and removing HTML content

> innerHTML oroperty

we can access and amend the contents of an element, including any child elements.

> DOM manipulation.

offers another technique to add new content to a page.

**createElement():** creates an element that can be added to the DOM tree, This new element is stored
inside a variable called newEl until it is attached to the DOM tree later on.


The **document object's write()** method is a simple way to add content that was not in the original
source code to the page, but its use is rarely advised.


The **innerHTML** property lets you get/update the entire content of any element as a string.


### XSS: Escaping & controlling markup.

we can control any markup added to the page. All data from untrusted sources should be escaped
on the server before it is shown on the page. Most server-side languages offer helper functions
that will strip-out or escape malicious code.


### Removing attributes:

to remove an attribute first select the element, then call removeAttribute().
It has one parameter the *name* of the attribute to remove it .