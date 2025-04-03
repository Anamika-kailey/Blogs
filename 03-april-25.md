# Exploring JavaScript Concepts: WeakSet, WeakMap, Object Methods, Destructuring, Date & Time, and JSON Methods

## WeakSet and WeakMap

### WeakSet

A WeakSet is a collection of objects where:

It only stores objects (no primitive values).

Objects in a WeakSet are weakly held, meaning they can be garbage-collected if there are no other references.

It does not have size properties or iteration methods like Set.

### WeakMap

A WeakMap is similar to Map but with the following differences:

Keys must be objects.

It does not prevent garbage collection of keys.

It lacks iteration methods and size properties.

### Object Methods: Object.keys(), Object.values(), Object.entries()

These methods allow easy extraction of object data.

Object.keys(obj): Returns an array of keys.

Object.values(obj): Returns an array of values.

Object.entries(obj): Returns an array of [key, value] pairs.

## Destructuring Assignment

Destructuring simplifies variable assignment from arrays and objects.

Array Destructuring:let [a, b, c] = [10, 20, 30];

console.log(a, b, c); // 10 20 30

Object Destructuring:let person = { firstName: "John", lastName: "Doe" };

let { firstName, lastName } = person;

console.log(firstName, lastName); // John Doe

## Date and Time in JavaScript

JavaScript provides the Date object for handling dates and times.

## JSON Methods and toJSON()

JSON.stringify() and JSON.parse()

These methods convert JavaScript objects to JSON and vice versa.

toJSON():

The toJSON() method allows customization of JSON stringification.

