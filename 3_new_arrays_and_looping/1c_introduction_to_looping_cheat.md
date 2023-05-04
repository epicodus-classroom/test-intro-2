## Terminology
<hr />

**Loop:** A piece of code that repeats until a condition is met.

**Callback function:** A function that is passed as an argument into another functions to be executed later.

**Anonymous function:** An unnamed function. They can be stored using a function expression or used as a callback in another function such as `Array.prototype.forEach()`.

**syntactic sugar**: syntax that makes a piece of code easier to write or use.

## Example
<hr />

```js
const languages = ['HTML', 'CSS', 'JavaScript'];
languages.forEach(function(language) {
  alert('I love ' + language + '!');
});
```