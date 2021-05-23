
# From the Duckett HTML book:

## * Chapter 2: “Text” (pp.40-61)

+ Headings and paragraphs
+ Bold, italic, emphasis
+ Structural and semantic markup


### + Headings : <h1<h2<h3<h4<h5<h6
### + ParagraPHs: <p
### + Bold & iTalic: <b & <i
### + suPerscriPT & suBscriPT: <sup & <sub
### + line Breaks & HorizonTal rules: <br/ & <hr/
### + strong & emphasis: <strong & <em
### + QuoTaTion: <blockquote & shorter quote <q
### + aBBreViaTions & acronyms: <abbr
### + ciTaTions & definiTions: <cite & <dfn
### + auTHor deTails: <address 
### + cHanges To content: <ins & <del & <s


<hr> </hr>

## * Chapter 10: Ch.10 “Introducing CSS” (pp.226-245)

+ What CSS does
+ How CSS works
+ Rules, properties, and values


- ExternaL css

link with html file > Head >>>   <link href="css/styles.css" type="text/css" rel="stylesheet" / ..

- Internal css
Html > head >>> <style ... { }

- Inine css
Inside the tag ..



CSS SeLectorS

* universal selector * {}

* Type selector h1,h2,h3 {}

* Class selector .note {}

* Id selector #intro {}

* child selector l1>a {}








<hr> </hr>


# From the Duckett JS book:


## * Chapter 2: “Basic JavaScript Instructions” (pp.53-84)

+ ARRAYS : An array is  a special type of variable. It doesn't just store one value; it stores a list of values. 

- CREATING AN ARRAY:

var colors; colors ['white', 'black', 'custom']; 

var el document.getElementByld('colors'); el. textContent = colors[0]; 


- ACCESSING & CHANGING VALUES IN AN ARRAY:

 // Create the array 

 var colors= ['white', 'black' , 'custom']; 
 
 // Update the third item in the array

  colors[2] =  'beige' ; 
 
 // Get the  element with an id of colors 

 var el = document. getElementByid('colors'); 

 //Replace with third item from the array

  el . textContent = colors[2]; 



+ EXPRESSIONS 

An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions:

1-EXPRESSIO NS THAT JUST ASSIGN A VALUE TO A VARIABLE.

2- EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE .



<hr></hr>
 
## * Chapter 4: “Decisions and Loops” only up to the section on switch statements (pp.145-162)

+ Conditional statements allow your code to make decisions about what to do next. 

+ Comparison operators (===, ! ==,  ==, ! =, <, >, <=, =>) are used to compare two operands.

+ Logical operators allow you to combine more than one set of comparison operators. 

+ if ... else statements allow you to run one set of code if a condition is true, and another if it is false.

+ switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match).

+ Data types can be coerced from one type to another.

+ All values evaluate to either truthy or falsy. 

+ There are three types of loop: for, while, and do ... while. Each repeats a set of statements. 



<hr> </hr>

# Additional Resources [link](https://chris.beams.io/posts/git-commit/)


## How to Write a Git Commit Message

Commit messages matter. Here's how to write them well.


### The seven rules of a great Git commit message

1- Separate subject from body with a blank line

2- Limit the subject line to 50 characters

3- Capitalize the subject line

4- Do not end the subject line with a period

5- Use the imperative mood in the subject line

6- Wrap the body at 72 characters

7- Use the body to explain what and why vs.how