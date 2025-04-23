# Understanding JavaScript: Frames, Binary Data, and Network Requests

Today was a productive one! I explored some essential concepts in JavaScript that every web developer should be comfortable with: frames and windows, working with binary data files, and handling network requests using fetch, FormData, and URL objects. Here's what I learned:

## Frames and Windows in JavaScript
JavaScript provides control over different windows or frames opened by a browser. These are useful when dealing with popups, embedded pages, or multiple browsing contexts.

Key Concepts:
window.open(url, name, specs) – Opens a new window or tab.

window.close() – Closes the current window (if opened by a script).

window.opener – A reference to the parent window.

iframe.contentWindow – Lets us access the window inside an <iframe>.

## Binary Data Files
Binary data is essential for handling files like images, PDFs, or custom formats in JavaScript. I explored how to manage this using Blob, ArrayBuffer, and TypedArray.

Useful APIs:
Blob – Represents immutable raw binary data.

ArrayBuffer – A fixed-length binary data buffer.

Uint8Array, Float32Array, etc. – Typed arrays that represent binary data in various numeric formats.

FileReader – Reads contents of files (e.g., using .readAsArrayBuffer()).

## Network Requests with fetch()
The fetch() API is modern and promise-based, making HTTP requests easy and readable.

const formData = new FormData();

formData.append('username', 'johndoe');

formData.append('profilePic', fileInput.files[0]);

fetch('/upload', {

  method: 'POST',
  
  body: formData

});

## Constructing URLs with URL and URLSearchParams
The URL object makes handling query parameters and relative paths clean and robust.

const url = new URL('https://example.com/api');

url.searchParams.append('user', 'john');

url.searchParams.set('active', 'true');

console.log(url.toString()); 
