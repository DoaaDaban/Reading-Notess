# Maps, Primitives, and File I/O

## Primitives vs Objects
Java's type system contains two main types: primitives and reference. All primitives have a reference object counterpart denoted as the same keyword with the first letter capitalized and written out as a full word if it wasn't already. The reference objects act as a form of wrappers and are required because of the way certain generic collections are written so that they can use anything that inherits from Object. Java usually can autobox from primitives to reference and unbox when not needed.<br>
In scalable systems, the usage from primitive to reference type will have an effect. Primitives almost always take up less memory and are accessed more quickly because they live in the stack while the reference types live in the heap. The default values for reference types are always null while numerics are always 0, booleans are false, and char is \u0000.

## Exceptions
An exception occurs when the normal execution of code is disrupted by something. These can happen naturally or be thrown manually using `throw`. To make sure the code doesn't completely end if this happens, you can wrap code in `try-catch` statements. In a `try` block, if an exception is thrown, then the code will jump to a `catch` statement. In a `catch` statement, all exceptions can be caught, or only specific types of exceptions. A `finally` statement is an additional section that will always run last, regardless if an exception was thrown or not.<br>
Try statements can also be used with resources. They do not necessarily need a catch statement connected. This usage allows for the resource to be closed automatically when it is finished using it, cleanly containing its usage to a single code block.<br>
Sometimes it is better for a method further up the call stack to catch an exception and you may even know what exception to expect. When this is the case, the keyword `throws` followed by a comma separated list of all expected exception types can be listed after the argument list in the method signature but before the first curly brace to start the code block. 

## Scanning
Java's scanner class looks at formatted input and breaks the data into tokens that can be properly translated to the correct data type. By default, the scanner uses white spaces as separators to determine a token, but there is a full list that can be adjusted invoking `useDelimiter()`. The scanner is able to convert these string tokens to the correct datatype using its built in collection of methods, but some of them are locale dependent, such as how commas or periods are read in things like long numbers. To account for this there is a method called `useLocale()` that takes in a Locale Object to set for the settings. Once done with a scanner, it needs to be closed using `close()`.



[Table of Contents](../README.md)



### External Links
- [Primitives vs Objects](https://www.baeldung.com/java-primitives-vs-objects)
- [Exceptions in Java](https://docs.oracle.com/javase/tutorial/essential/exceptions/index.html)
- [Java Scanner](https://docs.oracle.com/javase/tutorial/essential/io/scanning.html)