## Event Handler Properties
---

* These properties are also called "onevent" properties because they follow the naming convention on + event name.
* We set the value of an event handler property to a function. Any time the event is triggered, the function will be called. We can put whatever code we want to have run into the function. 
* Event handler properties belong to Web API objects (also called "interfaces"), like `Element`, `HTMLElement`, `document`, and `window`. This lesson covered events that targeted the HTML body, paragraph, H1, and image elements.
* Event handler properties are grouped by type, and often an event type is made up of many events. For example:
  * Keyboard events is an event type
  * Keyboard events are made up of three events: `onkeypress`, `onkeyup`, `onkeydown`.
* **Never use inline HTML event handler attributes.**

## Examples
---

The examples in this lesson used the Cookie Recipe project.

### Keyboard Events: `onkeydown` and `onkeyup`

```js
> let body = document.body;
> body.onkeydown = function() {
  body.style.backgroundColor = "black";
  body.style.color = "white";
};
> body.onkeyup = function() {
  body.style.backgroundColor = "white";
  body.style.color = "black";
};
```

### Mouse Events: `onclick` and `onmouseover`

```js
> let h1 = document.querySelector("h1");
> h1.onclick = function() {
  window.alert("I am a heading element.");
};
```

```js
> let h1 = document.querySelector("h1");
> h1.onmouseover = function() {
  window.alert("I am a heading element.");
};
> let p = document.querySelector("p");
> p.onmouseover = function() {
  document.querySelector("p>em").innerText = "Don't be surprised";
};
> let img = document.querySelector("img");
> img.onmouseover = function() {
  img.style.height = "700px";
};
```

### Clipboard Events: `oncopy`

```js
> let h1 = document.querySelector("h1");
> h1.oncopy = function() {
  window.alert("The heading element has been copied.");
};
```