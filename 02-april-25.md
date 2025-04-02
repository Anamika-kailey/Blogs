# Understanding JavaScript Data Types: Number, String, Array, Iterables, Map, and Set

Data types define the nature of the data stored in a variable and how it can be manipulated. In this blog, i will explore important JavaScript data types such as Number, String, Array, Iterables, Map, and Set.

## Number
The Number type represents both integer and floating-point values. JavaScript uses the IEEE 754 standard for representing numbers, meaning it supports both whole numbers and decimals, as well as special values like Infinity and NaN (Not-a-Number). Unlike some other programming languages, JavaScript does not have separate data types for integers and floating-point numbers.

--> let num1 = 42; // Integer

--> let num2 = 3.14; // Floating-point number

##  String

Strings represent sequences of characters and can be enclosed in single, double, or backticks ( ). JavaScript strings are immutable, meaning once created, they cannot be changed directly. Strings can contain alphanumeric characters, symbols, and even emojis. JavaScript provides various methods for handling and manipulating strings.

--> let str = "Hello, JavaScript!";

--> let str2 = 'Welcome to JS';

## String Methods

Some common methods used to manipulate strings:

--> console.log(str.length); // 18

--> console.log(str.toUpperCase()); // "HELLO, JAVASCRIPT!"

--> console.log(str.includes("JavaScript")); // true

--> console.log(str.replace("JavaScript", "JS")); // "Hello, JS!"

## Array

Arrays are ordered lists of values and can hold different data types. Arrays in JavaScript are zero-indexed, meaning the first element is at index 0. They are dynamic, allowing elements to be added or removed at runtime. Arrays are widely used for storing and manipulating collections of data.

--> let fruits = ["Apple", "Banana", "Mango"];

--> let mixedArray = [1, "Hello", true, { key: "value" }];

## Iterables

Iterables are objects that can be looped over using for...of. Examples include arrays, strings, maps, and sets. To be iterable, an object must implement the [Symbol.iterator] method. Iterables allow easy access and traversal of elements without needing to manually handle indexes or keys.

## Map

A Map is a collection of key-value pairs where keys can be of any type. Unlike objects, Maps maintain key order and allow any data type as a key. Maps are particularly useful when working with large datasets where key-value lookups need to be efficient.

--> let myMap = new Map();

--> myMap.set("name", "John");

--> myMap.set(42, "The answer");

## Set

A Set is a collection of unique values, meaning it automatically removes duplicates. It is useful when you need to store distinct elements and avoid redundancy in datasets. Sets are commonly used for operations like filtering unique values from an array.

--> let mySet = new Set([1, 2, 3, 3, 4]);

--> console.log(mySet); // Set { 1, 2, 3, 4 }
