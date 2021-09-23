# Reading: 01 - Java Basics

## [Java Basics](https://docs.oracle.com/javase/tutorial/java/nutsandbolts/index.html)

**Lesson: Language Basics**
* Variables 
  - Object stores its state in fields
  - Instance Variables (Non-Static Fields) - Objects store their individual states in non-static fields. In other words fields declared without the static keyword. Also known as instance variables.
  - Class Variables (Static Fields) - Class variables are any field declared with the static modifier. This tells you that there is exactly one copy of this variable in existence, regardless of how many times the class has been instantiated. 
  - Local Variables - A method will often store its temporary state in local variables, and is determined from where it is declared, which is between the opening and closing braces of a method.
  - Parameters - Always classified as "variables" not "fields". Example: main method
* Naming
  - Variable names are case-sensitive. 
  - Subsequent characters may be letters, digits, dollar signs, or underscore characters. 
  - If the name you choose consists of only one word, spell that word in all lowercase letters. If it consists of more than one word, capitalize the first letter of each subsequent word. 
  
* Operators - are special symbols that perform specific operations on one, two, or three operands, and then return a result.
  - Operator: Precedence
    postfix: 	expr++ expr--
    unary: 	++expr --expr +expr -expr ~ !
    multiplicative:	* / % 
    additive:	+ -
    shift:	<< >> >>>
    relational:	< > <= >= instanceof
    equality:	== !=
    bitwise AND:	&
    bitwise exclusive OR:	^
    bitwise inclusive OR:	|
    logical AND:	&&
    logical OR:	||
    ternary:	? :
    assignment:	= += -= *= /= %= &= ^= |= <<= >>= >>>=

* Expressions, Statements, and Blocks
  - Expression - is a construct made up of variables, operators, and method invocations, which are constructed according to the syntax of the language, that evaluates to a single value. 
  - Statements - are roughly equivalent to sentences in natural languages, and forms a complete unit of execution. 
    * Expression statement - Expressions can be made into a statement by terminating the expression with a semicolon (;). Types: assignment expressions, any use of ++ or --,method invocations, and object creation expressions
  - Blocks are a group of zero or more statements between balanced braces and can be used anywhere a single statement is allowed. 

* Control Flow Statements - break up the flow of execution by employing decision making, looping, and branching, enabling your program to conditionally execute particular blocks of code. 

![Control Flow Statements](https://static.javatpoint.com/tutorial/dart/images/dart-control-flow-statement.png)