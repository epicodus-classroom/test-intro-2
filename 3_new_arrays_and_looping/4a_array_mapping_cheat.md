## `Array.prototype.map()`
---

This is perhaps the most powerful looping method in JavaScript because it loops through a collection _and_ also transforms it.

Here's an example:

```js
const array = [0,1,2,3,4,5];
const doubledArray = array.map(function(element) {
  return element * 2;
});
doubledArray;
(6) [1, 2, 4, 6, 8, 10]
```

* Like `Array.prototype.forEach()`, `Array.prototype.map()` takes a function as an argument, which we call a callback function.

* With `Array.prototype.map()`, we _must_ use a `return` statement (unlike `Array.prototype.forEach()`).

* Each time we iterate with `Array.prototype.map()`, we are specifying how the element should be transformed. In the example above, we specify that we should `return element * 2`.

* `Array.prototype.map()` returns a transformed array. We can't use it to return another data type such as a number or string.

## Documentation on MDN
---

For more information, check out [the Mozilla documentation on `Array.prototype.map()`.](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/map)