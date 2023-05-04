## Example Code
<hr />

<div class="filename">calculator.html</div>

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <title>Calculator</title>
  <link href="css/styles.css" rel="stylesheet" type="text/css">
  <script src="js/scripts.js"></script>
</head>
<body>
  <h1>Calculator</h1>
  <form id="calculator">
    <label for="input1">1st number:</label>
    <input id="input1" type="text">
    <label for="input2">2nd number:</label>
    <input id="input2" type="text">

    <label>
      <input type="radio" name="operator" value="add">
      add
    </label>
    <label>
      <input type="radio" name="operator" value="subtract">
      subtract
    </label>
    <label>
      <input type="radio" name="operator" value="multiply">
      multiply
    </label>
    <label>
      <input type="radio" name="operator" value="divide">
      divide
    </label>

    <button type="submit" class="btn">Go!</button>
  </form>

  <h2>Results</h2>
  <p id="output"></p>
</body>
</html>
```

<div class="filename">js/scripts.js</div>

```javascript
// Business Logic
function add(num1, num2) {
  return num1 + num2;
}

function subtract(num1, num2) {
  return num1 - num2;
}

function multiply(num1, num2) {
  return num1 * num2;
}

function divide(num1, num2) {
  return num1 / num2;
}

// User Interface Logic
function handleCalculation(event) {
  event.preventDefault();
  const number1 = parseInt(document.querySelector("input#input1").value);
  const number2 = parseInt(document.querySelector("input#input2").value);
  const operator = document.querySelector("input[name='operator']:checked").value;

  let result;
  if (operator === "add") {
    result = add(number1, number2);
  } else if (operator === "subtract") {
    result = subtract(number1, number2);
  } else if (operator === "multiply") {
    result = multiply(number1, number2);
  } else if (operator === "divide") {
    result = divide(number1, number2);
  }

  document.getElementById("output").innerText = result;
}

window.addEventListener("load", function() {
  const form = document.getElementById("calculator");
  form.addEventListener("submit", handleCalculation);
});
```
