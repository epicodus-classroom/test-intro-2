## Examples
---

### Function Declaration

You should generally default to using function declarations.

```js
// this is a function declaration
function add(number1, number2) {
   return number1 + number2;
}
```

### Anonymous Function Expression

We'll use these in event handling.

```javascript
// this is a function expression
const add = function(number1, number2) {
  return number1 + number2;
};
```

### Named Function Expression

We won't use these in the program.

```javascript
// this is a **named** function expression
const calc = function add(number1, number2) {
  return number1 + number2;
};
```

