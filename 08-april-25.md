# Advanced workong with functions

As I continue my journey in learning JavaScript, today I explored some really interesting concepts that go beyond the basics—Global Object, Function Object, Named Function Expressions (NFE), the new Function() constructor, and task scheduling using setTimeout and setInterval. Here’s what I’ve learned and how these concepts work.
## The Global Object
In JavaScript, the global object provides variables and functions that are accessible from anywhere in your code.

In browsers, the global object is window.

In Node.js, it's global.

--> var myName = "Alex";

--> console.log(window.myName);

## Function as an Object
In JavaScript, functions are first-class objects, meaning they can:

Have properties

Be passed as arguments

Be returned from other functions

Functions even have built-in properties like:

name: the function's name

length: number of declared parameters

## Named Function Expression (NFE)
A Named Function Expression (NFE) is when a function expression has its own internal name. This is useful for recursion and debugging.

let sayHi = function greet() {

  console.log("Hi!");

};

sayHi();
## New Function Syntax (new Function)
You can create a function dynamically using the Function constructor:

let sum = new Function('a', 'b', 'return a + b');

console.log(sum(2, 3));

##  Scheduling: setTimeout & setInterval
JavaScript allows you to schedule tasks using:

### setTimeout(fn, delay)
Executes the function once after the delay.

### setInterval(fn, interval)
Executes the function repeatedly every interval.
