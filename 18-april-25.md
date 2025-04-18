# JavaScript Miscellaneous Topics: Proxy, Reflect, Currying, BigInt, and More
Today, I dove into some of the more advanced and lesser-known parts of JavaScript. These concepts expand the way we write, optimize, and interact with code. Here's a breakdown of what I learned

## Proxy and Reflect
Proxy allows us to create a wrapper around an object or function and intercept operations like reading, writing, or function calls.

Reflect is a built-in object that provides methods for interceptable JavaScript operations. It complements Proxy by offering default behavior implementations.

##  eval
The eval() function executes a string as JavaScript code. While powerful, it should be used with caution due to security and performance risks.

let code = "console.log('Hello from eval!')";

eval(code);

## Currying
Currying is a functional programming technique where a function with multiple arguments is transformed into a sequence of functions each taking a single argument.

## Reference Type
Primitive types (like numbers and strings) are copied by value, while objects are copied by reference.

let a = { name: "Alice" };

let b = a;

b.name = "Bob";

console.log(a.name);

## BigInt
JavaScript's Number type cannot safely represent integers beyond 2^53 - 1. BigInt allows you to work with arbitrarily large integers.

let big = 1234567890123456789012345678901234567890n;

console.log(big * 2n);

## Unicode
JavaScript strings are sequences of UTF-16 code units. Unicode allows for a wide range of characters from different languages and symbols.

let smile = "😊";

console.log(smile.length); 

## String Intervals
Checking string intervals or ranges can help with sorting and pattern detection.

let a = "apple";

let b = "banana";

console.log(a < b); 

## WeakRef and FinalizationRegistry
WeakRef lets you hold a weak reference to an object, allowing it to be garbage-collected if no other strong references exist.

let obj = { name: "Test" };

let ref = new WeakRef(obj);

console.log(ref.deref()); 

FinalizationRegistry lets you register a callback to be called when an object is garbage-collected.





