## Summary
---

* **To write code that we can reuse, it's generally considered a good choice to set up event handlers to use function declarations or function expressions that are stored in variables.** This code is considered scalable, because we can reuse those functions in multiple locations. The "scalability" of the code we write comes down to how quickly we can adapt our code to new requirements.
* You can choose to use either function declarations or function expressions in your event handlers, just remember the implication of hoisting. JS interpreters (programs that interpret JS code, like Google Chrome's V8 JS engine) perform **hoisting**, which is the process of moving the declaration of functions and variables to the top of their scope, prior to execution of the code.

## Code Examples
---

### Function Syntax: Defining, Calling, and Printing a Function

```js
// we are defining a function with a function declaration
> function alertHeading() {
  window.alert("This is a heading element.");
}
```

```js
// we are calling the alertHeading() function
> alertHeading();
```

```js
// this is printing the value of a function
> alertHeading;
ƒ alertHeading() {
  window.alert("This is a heading element.");
}
```

### Function Declarations with Event Handler Properties

```html
<h1>Heading 1</h1>
```

With a function expression:

```js
let h1 = document.querySelector("h1"); 
h1.onclick = function() {
  window.alert("This is a heading element.");
};
```

With a function declaration:

```js
let h1 = document.querySelector("h1");
function alertHeading() {
  window.alert("This is a heading element.");
}
h1.onclick = alertHeading;
```

### Function Declarations with Event Listeners

```html
<h1>Heading 1</h1>
```

With a function expression:

```js
let h1 = document.querySelector("h1"); 
h1.addEventListener("click", function() {
  window.alert("This is a heading element.");
});
```

With a function declaration:

```js
let h1 = document.querySelector("h1");
function alertHeading() {
  window.alert("This is a heading element.");
}
h1.addEventListener("click", alertHeading);
```


