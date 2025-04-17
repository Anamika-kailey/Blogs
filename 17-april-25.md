# Understanding Promises, Async/Await, Generators, and Modules in JavaScript

 Today, I dove into some of the most powerful tools JavaScript offers: Promises, Async/Await, Generators, and Modules.

## Promises: Handling Asynchronous Code Gracefully
A Promise is an object that represents the eventual completion (or failure) of an asynchronous operation. It has three states:

pending: initial state.

fulfilled: operation completed successfully.

rejected: operation failed.

let promise = new Promise((resolve, reject) => {
 
  setTimeout(() => resolve("Success!"), 1000);

});

promise.then(result => console.log(result)).catch(error => console.log(error));

Using .then() and .catch(), we can handle successful and failed outcomes cleanly.

##  Async/Await: Writing Cleaner Asynchronous Code
Async/await is syntactic sugar over promises, allowing us to write asynchronous code in a synchronous-looking way.

##  Generators: Pausing and Resuming Execution
Generators are special functions that can pause and resume execution. They are defined using the function* syntax and yield values one at a time.
Example--> 
function* numberGenerator() {
 
  yield 1;
  
  yield 2;
  
  yield 3;

}

const gen = numberGenerator();

console.log(gen.next().value);

console.log(gen.next().value);

## Modules: Organizing Code for Reuse

JavaScript modules allow us to split our code into reusable pieces. Using export and import, we can organize and manage large codebases better.
