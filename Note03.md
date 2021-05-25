
# From the Duckett HTML [book](https://lqudscollege-my.sharepoint.com/personal/advtech_ltuc_com/_layouts/15/onedrive.aspx?id=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks%2FHTML%20CSS%2Epdf&parent=%2Fpersonal%2Fadvtech%5Fltuc%5Fcom%2FDocuments%2FAcademia%2FCourses%2FCode%20Fellows%20Courses%2FE%2Dbooks&originalPath=aHR0cHM6Ly9hbHF1ZHNjb2xsZWdlLW15LnNoYXJlcG9pbnQuY29tLzpiOi9nL3BlcnNvbmFsL2FkdnRlY2hfbHR1Y19jb20vRVRES1VTSXQ5QnhLbWw5Mm5lUXFzTG9CN1dUTEZPNzB2Y3NtUThJLUhsUlRFUT9ydGltZT03ZGVwV3hVZTJVZwa):


## Chapter 3: “Lists” (pp.62-73)



There are lots of occasions when we need to use lists. HTML provides us with three different types:

* Ordered lists "ol" , "li" are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.
* Unordered lists "ul" , "li"  are lists that begin with a bullet point (rather than characters that indicate order).
* Definition lists "dl" , "dt" , "dd" , are made up of a set of terms along with the definitions for each of those terms.

## nested Lists

<ul>  <li>Mousses</li>  <li>Pastries<ul><li>Croissant</li><li>Mille-feuille</li><li>Palmier</li><li>Profiterole</li>      </ul>  </li>  <li>Tarts</li></ul>


<hr></hr>



## Chapter 13: “Boxes” (pp.300-329)

* Box Dimensionsw width, height
* limiting WiDth min-width, max-width 
* limiting height min-height, max-height

 ### overfloWing content

 * overflow
 * hidden
 * scroll

 p.one { 
     
      overflow: hidden;}
      
      p.two { 
          
           overflow: scroll;}



     ## Every box has three available properties that can be adjusted to control its appearance:

     1-  Border : Every box has a border (even if it is not visible or is specified to be 0 pixels wide). The border separates the edge of one box from another.

     2- Margin : Margins sit outside the edge of the border. You can set the width of a margin to create a gap between the borders of two adjacent boxes.

     3- Padding : Padding is the space between the border of a box and any content contained within it. Adding padding can increase the readability of its contents.



### White sPAce &verticAl mArgin

### border-width

### border-style

### border-color

### chAnge inline/Block: display

* inline
* block
* inline-block
* block


### visibility

* hidden
* visible

### border-image

### box-shadow

* horizontAl offset 
* verticAl offset 
* Blur Dist Ance
* sPreAD of shADoW


### border-radius

* border-top-right-radius
* border-bottom-right-radius
* border-bottom-left-radius
* border-top-left-radius





<hr> </hr>




# From the Duckett JS book:


## Review from Reading 02 - Chapter 2: “Basic JavaScript Instructions” (pp.70-73)

### VALUES IN ARRAYS

* NUMBERING ITEMS IN AN ARRAY 
* ACCESSING ITEMS IN AN ARRAY 
* NUMBER OF ITEMS IN AN ARRAY 


### EXPRESSIONS 
An expression evaluates into (results in) a single value. Broadly speaking there are two types of expressions. 

1- EXPRESSIO NS THAT JUST ASSIGN A VALUE TO A VARIABLE 
2- EXPRESSIONS THAT USE TWO OR MORE VALUES TO RETURN A SINGLE VALUE 


### OPERATORS 

Expressions rely on things called operators; they allow programmers to create a single value from one or more values. 


* A  script is made up of a series of statements. Each statement is like a step in a recipe. 
* Scripts contain very precise instructions. For example, you might specify that a value must be remembered before creating a calculation using that value. 
* Variables are used to temporarily store pieces of information used in  the script.
* Arrays are special types of variables that store more than one piece of related information.
* JavaScript distinguishes between numbers (0-9), strings (text), and Boolean values (true or false).
*  Expressions evaluate into a single value. Expressions rely on operators to calculate a value. 



## Chapter 4: “Decisions and Loops” from switch statements on (pp.162-182)