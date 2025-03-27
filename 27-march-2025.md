# Introduction to JavaScript: 
JavaScript is one of the most essential programming languages for web development. It allows developers to create dynamic and interactive websites. Today, I started my JavaScript learning journey, covering the basics, including code structure, variables, data types, interactions, type conversions, and operators.

## Understanding JavaScript Fundamentals

### Code Structure
JavaScript code is executed from top to bottom, following a structured flow. A script can consist of multiple statements, and each statement is generally terminated with a semicolon (;). However, JavaScript can still interpret code correctly without semicolons in many cases.

### Example -->
console.log("Hello, World!");
### Variables in JavaScript

Variables are used to store data values. In JavaScript, we use let, const, or var to declare variables:

let – allows reassignment

const – for constant values that cannot be changed

var – old way of defining variables (less recommended now)

### Example --> 
let name = "John";

const age = 25;

var city = "New York";

### Data Types in JavaScript

JavaScript has different types of data:

Primitive Data Types: string, number, boolean, null, undefined, symbol, bigint.

### Example --> 
let str = "Hello"; // string

typeof str; // "string"

let num = 10; // number

typeof num; // "number"

let isJavaScriptFun = true; // boolean

typeof isJavaScriptFun; // "boolean"

### Interaction with Users

JavaScript allows interaction with users through built-in functions like:

alert() – displays a message

prompt() – asks for user input

confirm() – asks for confirmation

### Example --> 
alert("Welcome to JavaScript!");

let userName = prompt("What is your name?");

let isConfirmed = confirm("Do you like JavaScript?");

### Type Conversions

JavaScript provides automatic and manual type conversions.

String conversion: String(value)

Number conversion: Number(value)

Boolean conversion: Boolean(value)

### Example --> 
let numString = String(123); // "123"

let stringToNum = Number("456"); // 456

let boolValue = Boolean(0); // false

### Basic Operators and Comparisons

JavaScript provides arithmetic, assignment, comparison, and logical operators.
