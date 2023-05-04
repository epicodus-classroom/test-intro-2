## JavaScript `arguments` Object

---

* JavaScript provides an `arguments` object in all functions. It is an "array-like" object that stores _all_ of the arguments passed into a function. We can use bracket notation to access arguments individually.

Here's an example:

```js
function isEmpty() {
  for (let i=0; i < arguments.length; i++) {
    if (arguments[i].trim().length === 0) {
      return true;
    }
  }
  return false;
}
```

We use a `for` loop and bracket notation to access each argument in the `arguments` object because `arguments` is not an array, which means we can't use `Array.prototype.forEach()` to loop through its arguments.