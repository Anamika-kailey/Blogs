# Exlored Error Handling and Async/Await in JavaScript
Today, I explored two essential topics in JavaScript: Error Handling and Async/Await. These are foundational for building reliable, clean, and efficient asynchronous JavaScript applications.

##  Error Handling in JavaScript
### Try...Catch
JavaScript provides a powerful try...catch block to handle runtime errors and prevent them from crashing your application.

### Syntax:
try {
  
} catch (error) {
 
}

### Finally Block
The finally block is executed always, whether there’s an error or not.

try {

  console.log("Trying...");

} catch (e) {

  console.log("Caught an error");

} finally {

  console.log("This will always run");

}

## Async/Await in JavaScript
async makes a function always return a Promise.

await makes JavaScript wait for a Promise to resolve before continuing.

It helps write asynchronous code in a synchronous style — clean and readable!

### async function example
async function greet() {

  return "Hello!";

}

### await Example
async function greet() {

  const message = await Promise.resolve("Hi there!");
  
  console.log(message); // "Hi there!"

}
