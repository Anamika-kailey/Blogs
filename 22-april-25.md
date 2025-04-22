# Explored concepts like Forms, Events, Resource Loading, and the Event Loop in JavaScript
Today’s deep dive into JavaScript unlocked some powerful browser concepts—from how forms work to how JavaScript manages execution and resource loading. Here’s a summary of what I explored:

## Form Properties and Methods
Forms are central to user input. JavaScript allows us to interact with form elements through properties like:

form.elements: Accesses all form controls.

form.name / form.method / form.action: Read or modify form details.

form.submit(): Submits the form programmatically.

form.reset(): Resets the form to its initial values.

## Focusing Elements
JavaScript can programmatically focus or blur input fields:

element.focus(): Sets focus to the element.

element.blur(): Removes focus.

##  Useful Input Events
Events on form inputs are essential for interactivity:

input: Triggers on every value change (real-time).

change: Triggers after losing focus when the value has changed.

cut, copy, paste: Triggered when the clipboard is used.

You can prevent default behavior using event.preventDefault() or customize responses to user actions.

## Document and Resource Loading
There are two main stages:

DOMContentLoaded: Fires when the HTML is fully parsed and DOM is built.

load: Fires when all resources (images, stylesheets, etc.) are loaded.

## Resource Loading
JavaScript can dynamically load scripts or resources. You can control this using attributes:

async: Script loads in parallel and executes when ready.

defer: Script loads in parallel but waits until DOM is ready.

## Selection and Range API
This is useful for custom text editors or handling selected content:

window.getSelection(): Gets the selected text.

document.createRange(): Creates a range to manipulate part of the DOM.

## JavaScript Event Loop
The event loop is the heart of JavaScript’s concurrency model. It processes:

Call Stack (sync code)

Task Queue (e.g., setTimeout)

Microtasks Queue (e.g., Promise.then)



