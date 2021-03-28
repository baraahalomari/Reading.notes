TEXT
the matter of the text is to show users the appropriate structure for the page

<h1> to <h6> html provide six level of heading
<p> </p> to create a new paragraphs
<b> </b> to  make characters appear bold
<i> </i> to make characters appear italic
<sup> </sup> is used to contain characters that should be superscript
<sub> </sub>  is used to contain characters that should be subscript
<br  /> to add a line break inside the middle of a paragraph
<hr /> To create a break between themes

Content management systems and HTML editors usually have two views of the page :
visual editor :  resemble word processors and allow you to control the presentation of text
code view : you can manually edit it, or so you can just enter new code by yourself. 

semantic markup: to o add extra information to the pages
<strong> : to  indicates that its content has strong importance.
<em> :to show the contents in italic
<blockquote> :used for longer quotes that take up an entire paragraph
<q> :used for shorter quotes that sit within a paragraph
<abbr> : for abbreviation or an acronym
<cite> : to indicate where the citation is from.
<dfn> : indicate the defning instance of a new term
<address> :to contain contact details for the author of the page, it may also contain a
phone number or email address
<ins> :to show content that has been inserted into a document
<del> :to show text that has been deleted from a document
<s> :indicates something that is no longer accurate or relevant (but that should not be deleted).


css

Block Elements
Block elements are used for large sections of text, such as paragraphs, headlines, or lists
A block element creates a (usually invisible) box in the browser display. By default, this box takes
up the full width of the display. The beginning of a block always starts on a new line in the display.
Inline Elements
Inline elements do not create a full-width box on the display. They modify the display of text, or
insert other things into the text — such as line breaks, images, or hyperlinks.
The basic syntax of a CSS ruleset has two parts: a ​selector​, and a group of ​rules​, each of which
consists of a ​property​ name and the ​value​ of that property.
selector​ {
​property​: value;
}
The selector indicates which HTML elements the rule will apply to. 
A ruleset can be composed of several rules, each of which applies a particular ​value​ to a ​property​ of
the selected elements. Properties are things such as the color, position, size, and shape of the element
A ​type selector​ applies to every HTML element of a particular type, such as ​p​ ​or​ ​em​. This selector
will apply to every ​p​ ​element:
p​ {
​color​: blue;
}

A ​class selector​ applies to all elements that share a ​class​ attribute. The class selector is written
starting with a ​.​ (dot):
.narrow {
​width​: ​20%​;
}

​id selector​ applies to an element with a particular ​id​ attribute. The id selector is written
starting with a ​#​ sign:
#sidebar​ {
​float​: left;
}

Using external css:
this means that the same code does not need to be repeated in every page
you should tell the browser where to find the CSS file used to style the page by <link> element
Using internal css
by placing CSS rules inside a <style> element, which usually sits inside the <head> element of the page

Javascript

A script: is a series of instructions that a computer can follow one-by-one.
Each individual instruction or step is known as a statement.
A statement is an individual instruction that the computer should follow. Each one should start on a
new line and end with a semicolon.
code blocks: when statements are surrounded by curly braces, The closing curly brace is not followed by a semicolon

comments
to explain what your code does, That help make your code easier to read and understand.
multi-line comment: starting with the /* characters and ending with the * / characters.
single-line comment: anything that follows the two forward slash characters // on that line will not
be processed by the JavaScript interpreter

variables: we can store the data in it.







