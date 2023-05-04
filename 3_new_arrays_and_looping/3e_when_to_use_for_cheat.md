## When to Use `for` Loops
---

* **When we need to break out of the loop.** For instance, we might want to break out of a loop when we verify that an array contains a result. Instead of looping through the rest of the array, we can use the `break;` or `return` keyword to end the loop.

* **When we're not looping through an array.** `Array.prototype.forEach()` only works with arrays. When we are using other data types, `for` loops can be more convenient.