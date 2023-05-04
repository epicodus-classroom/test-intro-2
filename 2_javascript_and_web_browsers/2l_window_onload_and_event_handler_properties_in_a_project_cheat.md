## Adding Event Handler Properties to a Project
---

### `window.onload`

* Any event handlers that we want to create when a webpage loads needs to be inside of the `window.onload` event handler property.
* The `window.onload` event handler property is triggered to run when a webpage has completed loading all of its resources: the CSS, images, scripts, HTML, and anything else.
* Putting our code to create event handlers inside of the `window.onload` event handler resolves the common error of our JS not being able to find the DOM elements it is supposed to target with an event handler. What's actually happening with this error is our JS is being run before the DOM has been constructed, which means the DOM elements actually don't exist when our JS is being run. 

<div class="filename">js/scripts.js</div>

```js
// User Interface Logic
window.onload = function() {
  let h1 = document.querySelector("h1");
  h1.onmouseover = function() {
    window.alert("I am a heading element.");
  };

  let p = document.querySelector("p");
  p.onmouseover = function() {
    document.querySelector("p>em").innerText = "Don't be surprised";
  };

  let img = document.querySelector("img");
  img.onmouseover = function() {
    img.style.height = "700px";
  };
};
```