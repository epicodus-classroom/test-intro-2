## Terminology
<hr />

* **Variable:** Variables can be thought of as containers used to store information. They allow for a way to label data with a descriptive name.

* **Lower camel case:** Use `lowerCamelCase` when naming JavaScript variables. Start with a lowercase letter, and if the variable name is more than one word, remove all spaces and capitalize the first letter of each subsequent word.

* **var:** The old way of declaring a variable in JavaScript. You should recognize it but not actually use this way of doing things! A JavaScript **statement**.

* **let:** The modern way of declaring a variable that changes in JavaScript. A JavaScript **statement**.

* **const:** The modern way of declaring a variable that should never change in JavaScript. This is short for constant. A JavaScript **statement**.

* **assignment operator:** This is the equals sign `=`; what we use to assign a value to a variable.

* **statement:** The technical term to group reserved keywords in JavaScript that serve a specific purpose, like variable declaration with `let`, `const`, or `var`.

## Tips
<hr />

* Variables should begin with a letter.

* Variables are case sensitive (`myNumber` is a _different_ variable than `myNUMBER`).

* Use clear names that describe the value being stored like `myNumber`.

* Always name your variables in a manner that will be easy for other developers to understand. Avoid vague letters or initials. (For example: `const x = 45` doesn't tell us what the value is.  Is 45 an age, a distance, size, a time?...)

## Examples
<hr />

Set a variable equal to a number:

```javascript
let myNumber = 45;
let favoriteNumber = 22;
```

Use a variable without modifying its value:

```javascript
favoriteNumber * 4;
```

Use a variable and modify it:

```javascript
favoriteNumber = favoriteNumber * 4;
```

Shortcut:

```javascript
favoriteNumber *= 4;
```

Use multiple variables:

```javascript
const myNumber = 45;
const otherNumber = 12;
const result = myNumber + otherNumber;
```


