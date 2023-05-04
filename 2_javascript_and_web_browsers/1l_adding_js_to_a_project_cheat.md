## Terminology
<hr />

* When we execute a function, we're **calling** a function.

* Once called, many functions will provide a result of some kind. This is known as **returning**, and the result is often referred to as a **return value**.

* **Refactor** means to rewrite code.

## Adding JS to a Project

* Create a file named `scripts.js` in a folder named `js`. We organize our scripts into one folder in case we have multiple script files (which we'll learn about in future sections).
* Add a script tag to your HTML `<head>` tags that points to the location of the file, like this: `<script src="js/scripts.js"></script>`

## Examples
<hr />

```javascript
function saySomething(whatToSay) {
  window.alert(whatToSay);
}
```

In the code above, a function named `saySomething()` is defined. When **called** this function will trigger an alert.

```javascript
function add(number1, number2) {
  return number1 + number2;
}
```

Here, a function named `add()` is being defined. It **returns** the sum of the two numbers it is provided.

```javascript
saySomething("The sum is " + add(3,5) + ".");
```

Here, we **call** our `saySomething()` function. The argument to `saySomething()` also contains our `add()` function, and has a string concatenated on either end.
