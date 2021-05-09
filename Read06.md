
# JavaScript Functions

A JavaScript function is a block of code designed to perform a particular task.

A JavaScript function is executed when "something" invokes it (calls it).

Example
function myFunction(p1, p2) {
  return p1 * p2;   // The function returns the product of p1 and p2
}

 ** Why Functions? **

You can reuse code: Define the code once, and use it many times.

You can use the same code many times with different arguments, to produce different results.


** Function Invocation: **

The code inside the function will execute when "something" invokes (calls) the function:

* When an event occurs (when a user clicks a button)
* When it is invoked (called) from JavaScript code
* Automatically (self invoked)


* ** Function Return **

 When JavaScript reaches a return statement, the function will stop executing.

If the function was invoked from a statement, JavaScript will "return" to execute the code after the invoking statement.

Functions often compute a return value. The return value is "returned" back to the "caller".

* ** The () Operator Invokes the Function **

Using the example above, toCelsius refers to the function object, and toCelsius() refers to the function result.

Accessing a function without () will return the function object instead of the function result.

* ** Functions Used as Variable Values **

Functions can be used the same way as you use variables, in all types of formulas, assignments, and calculations.

* ** Local Variables **

Variables declared within a JavaScript function, become LOCAL to the function.

Local variables can only be accessed from within the function.


for more [link](https://www.w3schools.com/js/js_functions.asp)


** Defining functions **

A function definition (also called a function declaration, or function statement) consists of the function keyword, followed by:

The name of the function.
A list of parameters to the function, enclosed in parentheses and separated by commas.
The JavaScript statements that define the function, enclosed in curly brackets, {...}.

** Function expressions**

While the function declaration above is syntactically a statement, functions can also be created by a function expression.

Such a function can be anonymous; it does not have to have a name. For example, the function square could have been defined as:

const square = function(number) { return number * number }
var x = square(4) // x gets the value 16

** Calling functions**

Defining a function does not execute it. Defining it names the function and specifies what to do when the function is called.

Calling the function actually performs the specified actions with the indicated parameters. For example, if you define the function square, you could call it as follows:

square(5);


** Function scope **

Variables defined inside a function cannot be accessed from anywhere outside the function, because the variable is defined only in the scope of the function. However, a function can access all variables and functions defined inside the scope in which it is defined.

In other words, a function defined in the global scope can access all variables defined in the global scope. A function defined inside another function can also access all variables defined in its parent function, and any other variables to which the parent function has access.


** Scope and the function stack**

Recursion
A function can refer to and call itself. There are three ways for a function to refer to itself:

The function's name
arguments.callee
An in-scope variable that refers to the function


** Nested functions and closures **

You may nest a function within another function. The nested (inner) function is private to its containing (outer) function.

It also forms a closure. A closure is an expression (most commonly, a function) that can have free variables together with an environment that binds those variables (that "closes" the expression).

Since a nested function is a closure, this means that a nested function can "inherit" the arguments and variables of its containing function. In other words, the inner function contains the scope of the outer function.

To summarize:

The inner function can be accessed only from statements in the outer function.
The inner function forms a closure: the inner function can use the arguments and variables of the outer function, while the outer function cannot use the arguments and variables of the inner function.