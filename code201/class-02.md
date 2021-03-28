# TEXT
the matter of the text is to show users the appropriate structure for the page


&lt;h1> to &lt;h6> html provide six level of heading

&lt;p> &lt;/p> to create a new paragraphs

&lt;b> &lt;/b> to  make characters appear bold

&lt;i> &lt;/i> to make characters appear italic

&lt;sup> &lt;/sup> is used to contain characters that should be superscript

&lt;sub> &lt;/sub>  is used to contain characters that should be subscript

&lt;br  /> to add a line break inside the middle of a paragraph

&lt;hr /> To create a break between themes


Content management systems and HTML editors usually have two views of the page :

* visual editor :  resemble word processors and allow you to control the presentation of text
* code view : you can manually edit it, or so you can just enter new code by yourself. 


> semantic markup: to o add extra information to the pages

&lt;strong> : to  indicates that its content has strong importance.

&lt;em> :to show the contents in italic

&lt;blockquote> :used for longer quotes that take up an entire paragraph.

&lt;q> :used for shorter quotes that sit within a paragraph.

&lt;abbr> : for abbreviation or an acronym.

&lt;cite> : to indicate where the citation is from.

&lt;dfn> : indicate the defning instance of a new term.

&lt;address> :to contain contact details for the author of the page, it may also contain a phone number or email address.

&lt;ins> :to show content that has been inserted into a document.

&lt;del> :to show text that has been deleted from a document.

&lt;s> :indicates something that is no longer accurate or relevant (but that should not be deleted).


# CSS

**Block Elements:**

Block elements are used for large sections of text, such as paragraphs, headlines, or lists.

A block element creates a (usually invisible) box in the browser display. By default, this box takes up the full width of the display. The beginning of a block always starts on a new line in the display.

**Inline Elements:**

Inline elements do not create a full-width box on the display. They modify the display of text, or insert other things into the text — such as line breaks, images, or hyperlinks.

The basic syntax of a CSS ruleset has two parts: *a ​selector*​, and a group of ​rules​, each of which consists of a ​property​ name and the ​value​ of that property.

selector​ {

    ​property​: value;

    }


The selector indicates which HTML elements the rule will apply to.

A ruleset can be composed of several rules, each of which applies a particular ​value​ to a ​property​ of
the selected elements. Properties are things such as the color, position, size, and shape of the element

A ​type selector​ applies to every HTML element of a particular type, such as ​p​ ​or​ ​em​. This selector will apply to every ​p​ ​element:

p​ {

​color​: blue;

}


A ​class selector​ applies to all elements that share a ​class​ attribute. The class selector is written starting with **a ​.​ (dot):**

.narrow {

​width​: ​20%​;

}


​id selector​ applies to an element with a particular ​id​ attribute. The id selector is written starting with **a ​#​ sign** :

#sidebar​ {

​float​: left;

}


### Using external css:

this means that the same code does not need to be repeated in every page
you should tell the browser where to find the CSS file used to style the page by &lt;link> element.

### Using internal css:
by placing CSS rules inside a &lt;style> element, which usually sits inside the &lt;head> element of the page.


# Javascript

* script: is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
* statement: is an individual instruction that the computer should follow. Each one should start on a new line and end with a semicolon.
* code blocks: when statements are surrounded by curly braces, The closing curly brace is not followed by a semicolon.


### comments:

to explain what your code does, That help make your code easier to read and understand.

> multi-line comment: starting with the /* characters and ending with the * / characters.

> single-line comment: anything that follows the two forward slash characters // on that line will not be processed by the JavaScript interpreter.


**variables:** we can store the data in it.
The result of any Calculation can be calculated or computed using the data stored in the variables.

> How to declare variables ?


**Numeric data type :** "var quantity = 3;"
**String data type :** "var quantity ="hello"
**Boolean data type:** true or false

we can then change what is stored in the variable later in the same script.

Here are rules we must always follow when giving a variable a name:

> The name must begin with a letter, dollar sign ($),or an underscore (_). It must not start with a number.

> All variables are case sensitive, so score and Score would be different variable names, but it is bad practice to create two variables that have the same name using different cases.

> The name can contain letters, numbers, dollar sign ($), or an underscore (_). Note that you must not use a dash(-) or a period (.) in a variable name.

> Use a name that describes the kind of information that the variable stores.

> You cannot use keywords or reserved words. Keywords are special words that tell the interpreter to do something. 

> If your variable name is made up of more than one word, use a capital letter for the first letter of every word after the first word(camel case). You can also use an underscore between each word (you cannot use a dash).


**Arrays :** is a special type of variable. It doesn't just store one value; it stores a list of values.

Each item in an array is automatically given a number called an index. This can be used to access specific items in the array.

**Expression :** evaluates into (results in) a single value 

var color = 'beige';

var area = 3 * 2;

buy = 3 > 5;  The value of buy is fa1se

buy= (5 > 3) && (2 < 4); The value of buy is now true


**concatenation :** Programmers call the process of joining together two or more strings to create one new string.


greeting= 'Hi 1 + 'Mol ly';  The value of greeting is now Hi Molly

var firstName = 'Ivy ' ;

var lastName = ' Stone' ;

var ful l Name = firstName + lastName;


## Decisions & loops

**Evaluations :** we can analyze values in our scripts to determine whether or note they match expected results.

**Decisions :** Using the results of evaluations, we can decide which path our script should go down.

**Loops :** There are also many occasions where we will want to perform the same set of steps repeatedly.


To make a decision, the code checks the current status of the script. this done by comparing two values using a comparison operator
which returns a value of true or false.

a conditional statement is based on a concept of if/else.
if the conditio returns true execute the statements between the first set of curly brackets, otherwise execute the statements between 
the secuned set of curly brackets.

if (i>5) {

document.write("true") ;

} else {

document.write("false");

}

> To comparing two expressions

((5<2) && (2>=8))

**logical operator** to compare the results of more than one comparison operator

&& logical and 

|| logical or 

! logical not 




