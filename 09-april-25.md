# Deep Dive into JavaScript: Decorators, Function Forwarding, Binding, and More
Today, I explored some powerful concepts in JavaScript that elevate the way we write and manage our code — from decorators to function forwarding, binding techniques, arrow functions revisited, and the core of object property configurations. Here's a breakdown of everything I learned:

##  Decorators

Decorators are a special kind of declaration that can be attached to classes and methods to modify their behavior. Although not natively available in JavaScript yet (they are in stage 3 of the TC39 proposal), decorators are widely used with TypeScript or transpilers like Babel.

##  Forwarding with call, apply, and bind
🔹 call() and apply()

call passes arguments individually

apply takes arguments as an array

🔸 bind()

bind() returns a new function with a bound this context.

## Arrow Functions Revisited
Arrow functions:

Do not have their own this

Are lexically bound to the scope where they are defined

Cannot be used as constructors.

## Object Property Configuration: Flags and Descriptors
Every object property has three internal flags:

writable – if true, the value can be changed

enumerable – if true, it shows up in loops

configurable – if true, the property can be deleted or modified

##  Getters and Setters
They are functions that behave like properties. Useful for defining computed properties.
