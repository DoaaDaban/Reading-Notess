# From the Duckett HTML book:

## *Introduction (pp.2-11)

+ About this book 
+ How the web works
+ Learning from other pages

** how PeopLe access the weB? **

* 1- Browsers
* 2- weB s  ervers
* 3- screen readers

** how the weB works? **

1- When you connect to the web, you do so via an Internet Service Provider (ISP). You type a domain name or web address into your browser to visit a site;  for example: google.com, bbc.co.uk, microsoft.com

2-Your computer contacts a network of servers called Domain Name System (DNS) servers. These act like phone books; they tell your computer the IP address associated with the requested domain name. An IP address is a number of up to 12 digits separated by periods / full stops. Every device connected to the web has a unique IP address; it is like the phone number for that computer.

3-the unique number that the DNS server returns to your computer allows your browser to contact the web server that hosts the website you requested. A web server is a computer that is constantly connected to the web, and is set up especially to send web pages to users.

4-The web server then sends the page you requested back to your web browser.


## * HTML Chapter 1: “Structure” (pp.12-39)

HtmL uses 
+ eLementS to deScribe tHe Structure of Pages
+ tags
+ body, Head & tit Le


## *  HTML Chapter 8: “Extra Markup” (p.176-199)

* Specifying different versions of HTML
* Identifying and grouping elements
* Comments, meta information and iframes


 * DOCTYPES tell browsers which version of HTML you are using.
 * You can add comments to your code between the  X<!-- and --> markers.
 + The id and class attributes allow you to identify particular elements.
 + The <div> and <span> elements allow you to group block-level and inline elements together.
 + <iframes>cut windows into your web pages through which other pages can be displayed.
 * The <meta> tag allows you to supply all kinds of information about your web page.
 +Escape characters are used to include special characters in your pages such as <, >, and ©.


## * HTML Chapter 17: “HTML5 Layout” (pp.428-451)

+ The new HTML5 elements indicate the purpose of different parts of a web page and help to describe its structure.
+ The new elements provide clearer code (compared with using multiple <div> elements).
+ Older browsers that do not understand HTML5 elements need to be told which elements are block-level elements.
+ To make HTML5 elements work in Internet Explorer 8 (and older versions of IE), extra JavaScript is needed, which is available free from Google.

## * HTML Chapter 18: “Process & Design” (pp.452-475)

+ It's important to understand who your target audience is, why they would come to your site, what information they want to find and when they are likely to return.
+ Site maps allow you to plan the structure of a site.
+ Wireframes allow you to organize the information that will need to go on each page.
+ Design is about communication. Visual hierarchy helps visitors understand what you are trying to tell them.
+ You can differentiate between pieces of information using size, color, and style. 
+ You can use grouping and similarity to help simplify Xthe information you present.



# From the Duckett JS book:

## * Introduction

This book explains how JavaScript can be used in  browsers to make websites more interactive, interesting, and user-friendly. You will also learn about jQuery because it  makes writing JavaScript a lot easier. 

** How JS make webpages more interactive? **

1-ACCESS CONTENT 

2-MODIFY CONTENT 

3-PROGRAM RULES 

4-REACT TO EVENTS 



## * JS Chapter 1: “The ABC of Programming” (pp.11-52)

*** What is A SCRIPT? ***
 
+ A  script is a series of instructions that the computer can follow in  order to achieve a goal.
 + Each time the script runs, it might only use a subset of all the instructions. 
 + Computers approach tasks in a different way than humans, so your instructions must let the computer solve the task prggrammatically. 
 + To approach writing a script, break down your goal into a series of tasks and then work out each step needed to complete that task (a flowchart can help). 


*** How do computers fit in with the world around them? ***
+ Creats models using data
+ The models use objects
+ programmers write code to say when this event occurs
+ web browsers use HTML markup to create a model
+ write code to make web page interactive

*** How do i write script for a web page? ***

 + It is best to keep JavaScript code in its own JavaScript file. JavaScript files are text files (like HTML pages and CSS style sheets), but they have the . j s extension. 
 + The HTML <script> element is used in HTML pages to tell the browser to load the JavaScript file (rather like the <link> element can be used to load a CSS file).
 + If you view the source code of the page in  the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web page that the browser has created. 