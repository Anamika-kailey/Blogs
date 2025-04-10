# Understanding JavaScript Prototypes and Classes

 Today, i explore some of core concepts: prototype inheritance, F.prototype, native prototypes, prototype methods, objects without __proto__, and the basics of classes and class inheritance.

## What is Prototype Inheritance?
In JavaScript, every object has a hidden property called [[Prototype]], which can be accessed using __proto__ (although it's better to use Object.getPrototypeOf() for modern code). This prototype is itself an object, and it can have its own prototype, forming a prototype chain.

When you try to access a property or method on an object and it's not found, JavaScript will look up the chain to the prototype to find it.

## The F.prototype Property
When you create a function in JavaScript, it automatically gets a prototype property. This is not the prototype of the function itself, but of objects created using that function with new.

##  Native Prototypes
Built-in objects like Array, Object, and Function also have prototypes. You can extend them, but you should be cautious when doing so.

## Prototype Methods
Prototype methods are functions defined on the constructor’s prototype. This makes them shared across all instances of that constructor, saving memory and improving performance.

##  Class Basic Syntax
JavaScript classes are a cleaner way to create constructor functions and handle inheritance.

class User {

  constructor(name) {
  
    this.name = name ;
  
  }

  greet() {
  
    console.log(`Hello, ${this.name}`) ;
  
  }

}

let user1 = new User("John") ;

user1.greet() ; 
