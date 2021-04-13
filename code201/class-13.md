# The Past, Present, and Future of Local Storage for Web Applications

The operating system typically provides an abstraction layer for storing and retrieving application-specific
 data like preferences or runtime state. These values may be stored in the registry, INI files, XML files, or some other
 place according to platform convention. 

Cookies were invented early in the web’s history.




## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5


userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure. 

In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of “Flash cookies.”

In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers.

In the meantime, Brad Neuberg and others continued to hack away on dojox.storage to provide a unified interface to all 
these different plugins and APIs. By 2009, dojox.storage could auto-detect (and provide a unified interface on top of) 
Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.



## INTRODUCING HTML5 STORAGE


It’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data
 persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. 
 Certain browser vendors also refer to it as **“Local Storage”** or **“DOM Storage.”**


## HTML5 STORAGE SUPPORT


> IE  8.0+

> FIREFOX  3.5+

> SAFARI 4.0+

> CHROME 4.0+

> OPERA  10.5+

> IPHONE 2.0+

> ANDROID 2.0+

				
## USING HTML5 STORAGE


You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. 
The data can be any type supported by **JavaScript**.

There are also methods for removing the value for a given named key, and clearing the entire storage area.
If you want to keep track programmatically of when the storage area changes, you can trap the storage event. 
The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.

Data is stored as strings. If you are storing something other than a string, you’ll need to coerce it yourself when you retrieve it.	
