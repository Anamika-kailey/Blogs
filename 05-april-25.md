# JavaScript Concepts Learned: Recursion & Stack, Global Object, Function Object, and new Function Syntax
In today's learning journey, I explored some deeper areas of JavaScript that are essential for mastering its inner workings. This blog covers four important concepts:

Recursion and the Call Stack

The Global Object

Function as an Object

The new Function Syntax

##  Recursion and the Call Stack

Recursion is a programming technique where a function calls itself in order to solve a problem. The idea behind recursion is to divide a complex problem into smaller, simpler sub-problems.

Recursion relies heavily on base cases, which define the condition under which the recursion should stop. Without a base case, recursion can lead to infinite loops and eventually result in a "stack overflow" error.

Key Points:
Recursive functions must have a termination condition (base case).

Deep recursive calls may lead to a stack overflow.

The call stack maintains execution context in a LIFO (Last In, First Out) manner.

##  Global Object

In JavaScript, the global object serves as the top-most object in the execution environment. It provides access to built-in functions, constructors, and variables that are globally available.

All global variables and functions are actually properties of this global object. This means that defining a variable globally implicitly attaches it to the global object.

Understanding the global object is crucial for managing scope, avoiding naming conflicts, and writing efficient global-level code.

Key Characteristics:

Acts as a container for all global identifiers.

Provides global methods like parseInt, setTimeout, alert, etc.

Avoid excessive use of global variables to prevent pollution of the global namespace.

##  Function as an Object

In JavaScript, functions are first-class objects. This means:

They can be assigned to variables.

Passed as arguments to other functions.

Returned from other functions.

Have properties and methods like any other object.

Each function in JavaScript is an instance of the built-in Function constructor. Because of this, functions themselves are objects, and we can even add properties to them.

This object-like behavior allows JavaScript to support advanced concepts like higher-order functions, closures, and callbacks.

## new Function Syntax

JavaScript allows us to dynamically create functions using the Function constructor. The syntax is:

new Function([arg1, arg2, ...argN], functionBody)

This approach is similar to using eval — it interprets the string as code and creates a new function at runtime.
