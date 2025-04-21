# Learn Browser Events in JavaScript
Today, I dived deep into one of the most essential parts of front-end development — Browser Events. Events allow web pages to be dynamic and interactive by responding to user actions. From clicking buttons to dragging elements across the screen, here’s a breakdown of what I explored:
## Introduction to Browser Events
Events are signals that something has happened. A few common examples include:

A user clicks a button

A key is pressed

The mouse moves

## Event Bubbling and Capturing
JavaScript events have a propagation phase:

Capturing Phase – the event goes down the DOM tree.

Target Phase – the event reaches the target.

Bubbling Phase – the event bubbles back up.

By default, most events bubble. But you can handle them during the capturing phase using the third argument in addEventListener.

## Event Delegation
Instead of adding listeners to many child elements, we can attach one listener to a parent and handle events as they bubble up. This is efficient and dynamic!

## Mouse Events
Some common mouse events include:

click

dblclick

mousedown / mouseup

mouseover / mouseout

mousemove

## Moving the Mouse
Tracking mouse position can be done with mousemove:

document.addEventListener('mousemove', (e) => {
  
  console.log(`Mouse at (${e.clientX}, ${e.clientY})`);

});

## Drag and Drop with Mouse
Creating drag-and-drop interfaces involves:

mousedown to start dragging

mousemove to move the item

mouseup to drop it

## Pointer Events
Pointer events unify mouse, touch, and stylus input:

pointerdown

pointermove

pointerup

pointercancel

## Keyboard Events
Handling keyboard input:

keydown: when a key is pressed

keyup: when a key is released

keypress: deprecated but was used for character input
