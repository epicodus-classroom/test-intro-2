## Terminology
<hr />

* **Destructive** methods modify the receiver (the thing they are called on). 
* **Non-destructive** methods don't modify the receiver, they create a brand new array. For non-destructive methods, you'll need to store the return value of the method in a variable.

## Methods
<hr />

* `Array.prototype.push()`: Push elements to the end of an array.
* `Array.prototype.concat()`: Concatenate elements to the end of an array. Similar to `Array.prototype.push()` except it doesn't modify the original array.
* `Array.prototype.unshift()`: Add an element to the beginning of an array.
* `Array.prototype.shift()`: Remove an element from the beginning of an array.
* `Array.prototype.pop()`: Remove an element from the end of an array.
* `Array.prototype.join()`: Turn an array into a string. You can pass an optional separator in as an argument. `""` is a common separator.
* `Array.prototype.slice()`: Slice elements from the beginning and (optionally) the end of an array.

## Modify Elements in an Array with Bracket Notation
<hr />

```js
> let array = [1,2,3];
> array[0] = "We just modified the array at position zero.";
> array;
["We just modified the array at position zero.",2,3]
```

## Documentation on MDN
---

See the list of array methods in the left-hand pane of the [Mozilla array documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array).