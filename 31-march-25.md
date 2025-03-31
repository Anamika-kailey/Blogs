# Understanding Objects in JavaScript
Today, i explore JavaScript objects, object references, copying, garbage collection, object methods, the this keyword, constructors, and the new operator.

##  Objects in JavaScript

Objects are fundamental building blocks in JavaScript. They allow us to store multiple values in a single variable using key-value pairs. An object is created using curly braces {} and contains properties and methods.

## Object References and Copying

Objects in JavaScript are stored by reference. When you assign an object to another variable, they both reference the same object, meaning changes in one reflect in the other.

##  Garbage Collection

JavaScript has automatic garbage collection. When an object becomes unreachable (i.e., no references point to it), the garbage collector removes it from memory.

## Object Methods

Objects can have methods—functions stored as properties.

## The this Keyword

To access the object, a method can use the this keyword.
let user = {

  name: "John",
  
  age: 30,

  sayHi() {
  
    alert(this.name);
  
  }

};

user.sayHi();

## The new Operator

The new operator creates a new object and binds this to it inside a constructor function.

et user2 = new Person("Bob", 28);

console.log(user2.name); // Output: Bob
