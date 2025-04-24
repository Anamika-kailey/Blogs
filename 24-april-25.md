# Advanced Web Development Essentials – Day's Learning Recap
Today, I explored a variety of modern web technologies that play a crucial role in enhancing interactivity, real-time communication, storage, and animations on the web. Here's a detailed overview of what I learned:

## URL Objects in JavaScript
URL objects provide a convenient way to parse, manipulate, and construct URLs. This is useful for query string manipulation, extracting parts of a URL, or dynamically building URLs.

let url = new URL('https://example.com?name=John&age=30');

console.log(url.searchParams.get('name')); // John
## Resumable File Uploads
Resumable uploads allow large files to be uploaded in chunks, and in case of interruptions, only the missing chunks are retried. Libraries like tus.io or Resumable.js are commonly used for this.

## Long Polling
A technique where the client repeatedly requests data from the server, with each request waiting until new data is available before responding.

## WebSocket
WebSocket provides full-duplex communication channels over a single TCP connection, ideal for real-time apps like chat systems.

## Server-Sent Events (SSE)
SSE is a server push technology that sends updates from the server to the browser via HTTP.

## Browser Storage
Cookies: Small data stored with every HTTP request. Limited in size (~4KB).

localStorage: Stores data with no expiration date.

sessionStorage: Similar to localStorage, but data is cleared when the session ends.

## Animations
### Bezier Curve
Defines smooth transitions using cubic-bezier functions in CSS.

transition: all 0.3s cubic-bezier(0.25, 1, 0.5, 1);
### CSS Animations

@keyframes slideIn {
 
  from { transform: translateX(-100%); }
  
  to { transform: translateX(0); }

}
### JavaScript Animations

let start = performance.now();

requestAnimationFrame(function animate(time) {

  let timePassed = time - start;
  
  draw(timePassed);
  
  if (timePassed < 2000) requestAnimationFrame(animate);

});

## Web Components
### Custom Elements
Define your own HTML elements using JavaScript.

### Shadow DOM
Encapsulates styles and markup to avoid conflicts with the main DOM.

### Template Elements
Reusable chunks of markup, ideal with Shadow DOM.
