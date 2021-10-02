# Online Reading: 02 - Arrays, Loops, Imports

# Packages and Import
Package = directory. Java classes can be grouped together in packages. A package name is the same as the directory (folder) name which contains the .java files. You declare packages when you define your Java program, and you name the packages you want to use from other libraries in an import statement.

Package declaration
The first statement, other than comments, in a Java source file, must be the package declaration.

Following the optional package declaration, you can have import statements, which allow you to specify classes from other packages that can be referenced without qualifying them with their package.

Default package. Altho all Java classes are in a directory, it's possible to omit the package declaration. For small programs it's common to omit it, in which case Java creates what it calls a default package. Sun recommends that you do not use default packages.

## [Java Imports (ignore the parts about NetBeans)](https://perso.ensta-paris.fr/~diam/java/online/notes-java/language/10basics/import.html)

**Packages and Import**
* Packages - Java classes can be grouped together in packages. Package name same as directory name containing the .java files.
* Package declaration - you can have import statements following the declaration, which will allow you to specify classes from other packages.
* Default package - a package that has omitted the package declaration.
* Package declaration syntax - statement order
  - Package statment
  - Imports
  - Class or interface definitions
* Imports: three options
  - JOptionPane class - is in the swing package, which is located in the javax package.
  - Wildcard character (*) - specifies that all classes with that package are available to your program.
  - Classes can be specified explicitly on import instead of using the wildcard character.
  - Can use class name without an import
* Common imports
  - import java.awt.*; -	Common GUI elements
  - import java.awt.event.*; -	The most common GUI event listeners
  - import javax.swing.*; - More common GUI elements. Note "javax"
  - import java.util.*; -	Data structures (Collections), time, Scanner, etc classes
  - import java.io.*; -	Input-output classes
  - import java.text.*; -	Some formatting classes.
import java.util.regex.*;	- Regular expression classes

## [Different types of loops in Java](https://www.baeldung.com/java-loops)

**A Guide to Java Loops**
* Looping in programming langauges is a feature that facilitates the execution of a set of instructions until the controlling Boolean-expression evaluates to false.
* Types of loops
  - For loop - allows you to repeat certain operations by incrementing and evaluating a loop counter
  - While loop - repeats a statement or a block of statements while its controlling Boolean-expression is true
  - Do-While loop - like a while loop, but the first condition evaluation happens after the first iteration of the loop