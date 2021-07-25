# Readings : Object-Oriented Programming, HTML Tables

## [READ](https://github.com/codefellows/domain_modeling#domain-modeling)

Domain Modeling
Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model.

A domain model that's articulated well can verify and validate the understanding of a specific problem among various stakeholders. As a communication tool, it defines a vocabulary that can be used within and between both technical and business teams

Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.

Here's some tips to follow when building your own domain models.

* When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and    behaviors.
* Model its attributes with a constructor function that defines and initializes properties.
* Model its behaviors with small methods that focus on doing one job well.
* Create instances using the new keyword followed by a call to a constructor function.
* Store the newly created object in a variable so you can access its properties and methods from outside.
* Use the this variable within methods so you can access the object's properties and methods from inside.

![object modeling](http://sanderhoogendoorn.com/wp-content/image92.png)

Define a constructor and initialize properties
To define the same properties between many objects, you'll want to use a constructor function. Below is a table that summarizes a JavaScript representation of an EpicFailVideo object.

Property	Data	Type
epicRating	1 to 10	Number
hasAnimals	true or false	Boolean
Here's an implementation of the EpicFailVideo constructor function.

var EpicFailVideo = function(epicRating, hasAnimals) {
  this.epicRating = epicRating;
  this.hasAnimals = hasAnimals;
}

var parkourFail = new EpicFailVideo(7, false);
var corgiFail = new EpicFailVideo(4, true);

console.log(parkourFail);
console.log(corgiFail);
As you can see, the constructor function is defined using a function expression. In other words, the variable EpicFailVideo is declared and then assigned a function with two parameters called epicRating and hasAnimals.

When the function is called, the data inside these parameters are stored inside the this.epicRating and this.hasAnimals properties respectively. Storing data within properties ensures any newly created object can access that data later.

After the constructor function definition, two objects are instantiated with the new keyword and their properties are initialized by calling the EpicFailVideo constructor function. After being instantiated and initialized, these objects are stored inside the parkourFail and corgiFail variables.


## From the Duckett HTML book:

### Chapter 6: “Tables” (pp.126-145)

Define an HTML Table
The ```html <table> ```tag defines an HTML table.

Each table row is defined with a ```html <tr>``` tag. Each table header is defined with a ```html <th>``` tag. Each table data/cell is defined with a ```html <td>``` tag.

By default, the text in ```html <th> ``` elements are bold and centered.

By default, the text in ```html <td> ``` elements are regular and left-aligned.





### Chapter 3: “Functions, Methods, and Objects” (pp.106-144)

A method is a function associated with an object, or, put differently, a method is a property of an object that is a function. Methods are defined the way normal functions are defined, except that they have to be assigned as the property of an object.
