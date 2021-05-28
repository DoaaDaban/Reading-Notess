
<hr>

# Reading
</hr>
[Understanding the problem domain is the hardest part of programming
From the Duckett JS book](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

## What is the hardest thing about writing code?

There are many common answers to this question:

* Learning a new technology
* Naming things
* Testing your code
* Debugging
* Fixing bugs
* Making software maintainable
* The list goes on and on.

## Why problem domains are hard

Have you ever tried to put together a jigsaw puzzle that didn’t have any picture on it?  How about one like this one, that has a very similar pattern repeated on it and is double-sided?

The reason why puzzles like this one are so hard, is because you can’t really see what you are trying to build very clearly.  Normally when you put together a jigsaw puzzle you follow steps that might look something like this:

1- Figure out what the major components of the picture are
2- Sort the pieces by color or component
3- Put together all the border pieces
4- Put together each component of the picture from the piles you created
5- This all breaks down when you don’t have a picture with clear components that you can identify.

The same thing happens when writing code.  Writing code is a lot like putting together a jigsaw puzzle.  We put together code with the purpose of building components that we have taken out of the “bigger picture” of the problem domain.

The big issue is that many problem domains are like a puzzle with a blurry picture or no picture at all

he real world is a messy place.  Many of the problem domains we face as programmers are difficult to understand and look completely different depending on your viewpoint.

As programmers, we also are often not given complete information about the problem domain, so we don’t even have the information we need to understand it.

## What can you do about it?

If understanding the problem domain is the hardest part of programming and you want to make programming easier, you can do one of two things:

1- Make the problem domain easier
2- Get better at understanding the problem domain

You can often make the problem domain easier by cutting out cases and narrowing your focus to a particular part of the problem.

What I mean by this is that it is often beneficial to take a part of the problem and fully understand that part before expanding the problem domain.

The other choice is to become better at understanding problem domains.  As developers, we tend to think that sitting down and talking to customers or business people who know about the problem domain is a waste of time. It is easy to fall into the trap of thinking you understand enough of the problem to get started coding it.  Best to resist the temptation to “not waste anymore time talking” and make sure you understand a problem inside and out before you try and solve it with code.  It is much more expensive and time consuming to do things over than it is to do them right the first time.  I learn this lesson the hard way time and time again.



<hr>

# Chapter 3: “Object Literals” (pp.100-105)
</hr>

## WHAT IS AN OBJECT?

Objects group together a set of variables and functions to create a model
of a something you would recognize from the real world. In an object,
variables and functions take on new names.

* IN AN OBJECT: VARIABLES BECOME
KNOWN AS PROPERTIES 

If a variable is part of an object, it is called a
property. Properties te ll us about the object, such as
the name of a hotel or the number of rooms it has.
Each individual hotel might have a different name
and a different number of rooms.

* IN AN OBJECT: FUNCTIONS BECOME
KNOWN AS METHODS

If a function is part of an object, it is called a method.
Methods represent tasks that are associated with
the object. For example, you can check how many
rooms are available by subtracting the number of
booked rooms from the total number of rooms.

## [Creating a JavaScript Object](https://www.w3schools.com/js/js_object_definition.asp):

There are different ways to create new objects:

1- Define and create a single object, using an object literal.

Example

```js script
<script >
var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"};
document.getElementById("demo").innerHTML =
person.firstName + " is " + person.age + " years old.";
 </script>;  
```

2- Define and create a single object, with the keyword new.

```js script
<script>
var person = new Object();
person.firstName = "John";
person.lastName = "Doe";
person.age = 50;
person.eyeColor = "blue"; 

document.getElementById("demo").innerHTML =
person.firstName + " is " + person.age + " years old.";
</script>
```

3- Define an object constructor, and then create objects of the constructed type.

var varName = new Object();


## JavaScript Objects are Mutable

Objects are mutable: They are addressed by reference, not by value.

```js 
<script>
var person = {firstName:"John", lastName:"Doe", age:50, eyeColor:"blue"}

var x = person;
x.age = 10;           // This will change both x.age and person.age
</script>
```

<hr>

# Chapter 5: “Document Object Model” (pp.183-242)
</hr>

The Document Object Model (DOM) is a cross-platform and language-independent interface that treats an XML or HTML document as a tree structure wherein each node is an object representing a part of the document. The DOM represents a document with a logical tree. 

![DOM MODEL](https://upload.wikimedia.org/wikipedia/commons/5/5a/DOM-model.svg)

* MAKING A MODEL OF THE
HTML PAGE
When the browser loads a web page, it
creates a model of the page in memory.
The DOM specifies the way in which the
browser should structure this model using
a DOM tree.
The DOM is called an object model
because the model (the DOM tree) is
made of objects.
Each object represents a different part of
the page loaded in the browser window

* ACCESSING AND CHANGING
THE HTML PAGE
The DOM also defines methods and
properties to access and update each
object in this model, which in turn updates
what the user sees in the browser.
You will hear people call the DOM an
Application Programming Interface (API).
User interfaces let humans interact with
programs; APls let programs (and scripts)
talk to each other. The DOM states what
your script can "ask the browser about the
current page, and how to tell the browser
to update what is being shown to the user.


***THE DOCUMENT NODE***

**ELEMENT NODES**

**ATTRIBUTE NODES**

**TEXT NODES**



## WORKING WITH THE DOM TREE
Accessing and updating the DOM tree involves two steps:

1- Locate the node that represents the element you want to work with.
2- Use its text content, child elements, and attributes.

STEP 1: ACCESS THE ELEMENTS

* SELECT AN INDIVIDUAL ELEMENT NODE

* SELECT MULTIPLE
ELEMENTS (NODELISTS) 

* TRAVERSING BETWEEN ELEMENT NODES

STEP 2: WORK WITH THOSE ELEMENTS

* ACCESS/ UPDATE
TEXT NODES

* WORK WITH HTML
CONTENT

* ACCESS OR UPDATE
ATTRIBUTE VALUES

















































