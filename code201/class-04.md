# Links

 allow you to move from one web page to another ,by using the &lt;a> element.
 Users can click on anything between the opening &lt;a> tag and the closing &lt;/a> tag. You specify which page you want to link to using the href attribute.

like &lt;a href="https://www.google.com"> google &lt;/a>

Clear link text can help visitors find what they want.

**absolute URL:** the full web address for the site
and If all the pages of the site are in the same folder, then the value
of the href attribute is just the name of the file.


we should organize the code by placing the pages for each different section of the site into a new folder.

**The root folder contains:**
* A fle called index.html which is the homepage for the entire site
* Individual folders for the sections of the site


**Mailto:** To create a link that starts up the user's email program and
addresses an email to a specifed email address, you use the &lt;a> element.


**Target:** to open the link in a new window, you can use the target attribute on the opening &lt;a> tag. 


**Linking to a specific part of the page:**

 to add a link from part way down the page back to the top we nead to identify the point in the page that the link will go.To link to an element that uses an id attribute we use the &lt;a> element again, but the value of
the *href* attribute starts with the # symbol, followed by the value of the id attribute of the element we want to link to. 

if we want to link to another page As long as the page we arelinking to has id attributes that identify specifc parts of the page, we can simply add the same syntax to the end of the link for that page.

Therefore, the **href** attribute will contain the address for the page (either an absolute URL or a relative URL), followed by the # symbol, followed by the value of the id attribute that is used on the element we are linking to.


# Layout

We talked before about control how much space each box takes up by setting the width of the boxes.to separate boxes  we can use borders, margins, padding, and background colors.

also, we can but boxes together by group elements inside a block-element.


> **positioning schemes:** to control the layout of a page: normal ﬂow, relative positioning, and absolute positioning.


**box offset:** To indicate where a box should be positioned.to tell the browser how far from the top or bottom and left or right it should be placed.


# Functions & Methods & Objects


**functions:** fonctions consist of a series of statements that have been grouped together because they perform a specific task.

first, we need to give our function a name,this name should describe the task it is performing.then we ask it to perform its task dy Calling the function.

when we write a function and expect it to provide us with an answer that return value

function sayHello(){

document.write("hello");

}

>function keyword=> function

>function name => sayHello

>in curly braces=> code block

some functions needs specific information we give it parameters act like variables.

**Method :** are created inside the object.

**Objects :**are made up of properties and methods.



# 6-reasons-for-pair-programming

pair programming commonly involves two roles: the Driver and the Navigator. 

The Driver is the programmer who is typing and the only one whose hands are on the keyboard. The Navigator uses their words to guide the Driver but does not provide any direct input to the computer. 

 there are four fundamental skills that help anyone learn a new language:
 * Listening: hearing and interpreting the vocabulary Speaking: using the correct words to communicate an idea 

* Reading: understanding what written language intends to convey 
* Writing: producing from scratch a meaningful

1. **Greater efficiency**

 Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging.

2. **Engaged collaboration**

knowing when to ask for help. We advise our students to spend no more than fifteen minutes stuck on a problem before asking a teaching assistant or instructor for help.

3. **Learning from fellow students**

Everyone has a different approach to problem solving; working with a teammate can expose developers to  techniques they otherwise would not have thought of.
When working with someone who has a different coding style, communication is key. This can become more difficult when two programmers have different personalities.

 Pair programming not only improves programming skills, but can also help programmers develop their interpersonal skills.

5. **Job interview readiness**

For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than
 specific technical skills. Pair programming strengthens all of those skills.

6. **Work environment readiness**

Code Fellows graduates who are already familiar with how pairing works can hit the 
ground running at a new job, with one less hurdle to overcome.


