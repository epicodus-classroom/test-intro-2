## Terminology
<hr />

* **Pointer**:  A reference to an object in memory but not the object itself; for example, a variable that is set to an array does not contain the array itself but rather a pointer to the saved array.  
* **Edge case**: An edge case in computer programming is a possible outcome of an operation that leads to unexpected or inconsistent results.

## Tips
<hr />

* No two arrays are the same even if they have the exact same contents inside!

* Arrays cannot be compared with the `===` operator. However, they may be transformed into strings with `.toString()`, and those strings may be compared with `===`.

* Arrays cannot be cloned by setting a new variable name to the original array (i.e.: `let cloneArray = originalArray;`). This will only create a pointer to the original array.

## Examples
<hr />

To properly clone array (i.e.: not simply create a pointer to existing array):

```javascript
const cloneArray = originalArray.slice();
```

To compare arrays by transforming them into strings:

```javascript
const a = [1,2,3];
const b = [1,2,3];

a.toString() === b.toString();
```

## Additional Resources
<hr />

For more details on how the `Array.prototype.slice()` method works, check out [MDN's JavaScript documentation](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array/slice).
