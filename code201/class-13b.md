# What Google Learned From Its Quest to Build the Perfect Team


Our data-saturated age enables us to examine our work habits and office quirks with a scrutiny that our cubicle-bound
 forebears could only dream of.

Yet many of today’s most valuable firms have come to realize that analyzing and improving individual workers ­ isn’t enough. As commerce becomes increasingly global and complex, the bulk of modern work is more and more team-based. 
In Silicon Valley, software engineers are encouraged to work together, in part because studies show that groups tend to innovate .

faster, see mistakes more quickly and find better solutions to problems. 
Google — one of the most public proselytizers of how studying workers can transform productivity — became focused on building the  perfect team. In the last decade, the tech giant has spent untold millions of dollars measuring nearly every aspect of its employees’ lives. 

The company’s top executives long believed that building the best teams meant combining the best people.
In 2012, the company embarked on an initiative — code-named Project Aristotle — to study hundreds of Google’s teams and figure out why some stumbled while others soared. 

No matter how researchers arranged the data, though, it was almost impossible to find patterns — or any evidence that the composition of a team made any difference. 

Some groups that were ranked among Google’s most effective teams, for instance, were composed of friends who socialized outside work. Others were made up of people who were basically strangers away from the conference room.

In 2008, a group of psychologists from Carnegie Mellon, M.I.T. and Union College began to try to answer a question very much like this one.

Conversely, teams that failed at one thing seemed to fail at everything. The researchers eventually concluded that what distinguished the ‘‘good’’ teams from the dysfunctional groups was how teammates treated one another. 



# Transforms


The transform property comes in two different settings, two-dimensional and three-dimensional. Each of these come with their own individual properties and values.

The actual syntax for the transform property is quite simple, including the transform property followed by the value. The value specifies the transform type followed by a specific amount inside parentheses.


## 2D Transforms


Two-dimensional transforms work on the x and y axes, known as horizontal and vertical axes. Three-dimensional transforms work on both the x and y axes, as well as the z axis.

### 2D Rotate

The transform property accepts a handful of different values. The rotate value provides the ability to rotate an element from 0 to 360 degrees. Using a positive value will rotate an element clockwise, and using a negative value will rotate the element counterclockwise. 


### 2D Scale

Using the scale value within the transform property allows you to change the appeared size of an element. The default scale value is 1


### Transform Origin


As previously mentioned, the default transform origin is the dead center of an element, both 50% horizontally and 50% vertically. To change this default origin position the transform-origin property may be used.the transform-origin property does run into some issues .

When also using the translate transform value. Since both of them are attempting to position the element, their values can collide. 




# Transitions & Animations


The easiest way for determining styles for different states is by using the **:hover**, **:focus**, **:active**, and **:target** pseudo-classes.

The transition-property property determines exactly what properties will be altered in conjunction with the other transitional properties. By default, all of the properties within an element’s different states will be altered upon change. 


## Transition Duration


The duration in which a transition takes place is set using the transition-duration property. The value of this 
property can be set using general timing values, including seconds (s) and milliseconds (ms). These timing values
 may also come in fractional measurements, .2s for example.



## Transition Timing


The transition-timing-function property is used to set the speed in which a transition will move. Knowing the duration
 from the transition-duration property a transition can have multiple speeds within a single duration. 



# Animations


when more control is required, transitions need to have multiple states. In return, this is where animations pick up where transitions leave off.

To set multiple points at which an element should undergo a transition, use the @keyframes rule. The @keyframes rule includes the animation name, any animation breakpoints, and the properties intended to be animated.

It is important to note, as with transitions only individual properties may be animated. Consider how you might move an element from top to bottom .


## Animation Duration, Timing Function, & Delay


Once you have declared the animation-name property on an element, animations behave similarly to transitions. They include a duration, timing function, and delay if desired. 

A timing function and delay can be declared using the animation-timing-function and animation-delay properties respectively.

## Customizing Animations


Animations also provide the ability to further customize an element’s behavior, including the ability to declare the number of times an animation runs, as well as the direction in which an animation completes.