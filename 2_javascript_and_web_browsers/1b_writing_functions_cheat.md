## Terminology

---

* An **argument** is what you pass into a function or method when you are calling it.

* A **parameter** is a placeholder variable for the data we pass into a function via the argument. The value of a parameter is set to the argument we pass into the function when we are calling the function. In the example below, `number1` and `number2` are parameters while `1` and `2` are arguments.

## Sample code
---

This function takes 2 arguments (expecting two numbers) and assigns them to the parameters `number1` and `number2`. The function returns a number:

```javascript
function add(number1, number2) {  // function declaration
  return number1 + number2; 
}
> add(1, 2);                      // function call
3                                 // returned value from the function
```

### Parts of a function

* A **function declaration** starts with the `function` keyword.
* Next comes the name. It should be descriptive and clear. In the example above, the name is `add`. Always use lower camel case for function names.
* The name is always followed with parens. These parens may or may not include **parameters**. In the `add` function above, `number1` and `number2` are parameters.
* The function **body** is enclosed in curly brackets. The code inside the curly brackets is the code that will be executed when the function is called.
* Generally, you will want to `return` a value from your function. It's very common for beginners to forget the `return`, which means that the function will return `undefined` instead of a value. In the example above, the `add` function will return the value of `number1 + number2`.

### Conventions

* Use lower camelCase for function names.
* Use descriptive variable names so that your code is easy to understand. Don't be tempted to abbreviate.

