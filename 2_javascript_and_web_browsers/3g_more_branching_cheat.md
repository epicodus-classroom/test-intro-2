## Terminology
<hr />

Logical operators:

* `&&` means **and**: `age >= 12 && height >= 60`
* `||` means **or**: `age >= 12 || height >= 48`
* `!` means not: `!age || !height`
*  Empty strings, the number `0`, the number `NaN`, `undefined`, `null`, and `false` itself are **falsey**. If JavaScript sees any of these as a branching condition, it will treat them as false. **Everything else is truthy**, including numbers and strings with values like `3` or `"hello world"`.

## Completed Code
---

<div class="filename">css/styles.css</div>

```css
.hidden {
  display: none;
}

#error-message {
  font-weight: 600; 
  color: red;
}
```

<div class="filename">amusement-park.html</div>

```html
<!DOCTYPE html>
<html lang="en-US">
  <head>
    <link rel="stylesheet" href="css/styles.css" type="text/css">
    <script src="js/scripts.js"></script>
    <title>Amusement Park</title>
  </head>
  <body>
    <div>
      <h1>Fun 4 All</h1>

      <p>Welcome to the Fun 4 All amusement park!</p>
      <p>At Fun 4 All you need to be a certain age and height to ride on our rides.</p>
      <p>Enter your age and height in the form below and we'll show you what rides you can go on.</p>

      <form id="userInfo">
        <p id="error-message" class="hidden">Please enter an age and height in whole numbers.</p>
        <label for="age">Age</label>
        <input id="age" type="text">
        <label for="height">Height in inches</label>
        <input id="height" type="text">
        <button type="submit">Show me what I can ride!</button>
      </form>

      <div id="swings" class="hidden">
        <h1>You can ride the Swings.</h1>
        <p>To ride the Swings you need to be at least 6 years old.</p> 
      </div>
      <div id="coaster" class="hidden">
        <h1>You can ride the Roller Coaster.</h1>
        <p>To ride the Roller Coaster you need to be either 12 years old or 48 or more inches tall.</p> 
      </div>
      <div id="tower" class="hidden">
        <h1>You can ride the Tower of Doom.</h1>
        <p>To ride the Tower of Doom you need to be at least 12 years old and 60 or more inches tall.</p> 
      </div>
      <div id="sorry" class="hidden">
        <h1>You are too young to ride! Sorry!</h1>
        <p>Come back when you are 6 years old.</p> 
      </div>
    </div>
  </body>
</html>
```

<div class="filename">js/scripts.js</div>

```js
// User Interface Logic

function hideResultsAndError() {
  document.getElementById("error-message").setAttribute("class", "hidden");
  document.getElementById("swings").setAttribute("class", "hidden");
  document.getElementById("coaster").setAttribute("class", "hidden");
  document.getElementById("tower").setAttribute("class", "hidden");
  document.getElementById("sorry").setAttribute("class", "hidden");
}

window.onload = function() {
  hideResultsAndError();

  document.querySelector("form").onsubmit = function(event) {
    event.preventDefault();
    hideResultsAndError();
    const age = parseInt(document.querySelector("input#age").value);
    const height = parseInt(document.querySelector("input#height").value);

    if (age && height) {
      if (age >= 12 && height >= 60) {
        document.getElementById("swings").removeAttribute("class");
        document.getElementById("coaster").removeAttribute("class");
        document.getElementById("tower").removeAttribute("class");
      } else if (age >= 12 || height >= 48) {
        document.getElementById("swings").removeAttribute("class");
        document.getElementById("coaster").removeAttribute("class");
      } else if (age >= 6) {
        document.getElementById("swings").removeAttribute("class");
      } else {
        document.getElementById("sorry").removeAttribute("class");
      }
    } else {
      document.getElementById("error-message").removeAttribute("class");
    }
  };
};
```