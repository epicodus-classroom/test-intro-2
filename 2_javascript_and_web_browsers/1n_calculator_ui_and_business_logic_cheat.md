## Example
<hr />

The following code prompts the user for two numbers, uses the included `add()` function to add these two numbers together, and provides the sum to the user in an alert box:

<div class="filename">js/scripts.js</div>

```javascript
// business logic
function add(number1, number2) {
  return number1 + number2;
}

// user interface logic 
const number1 = parseInt(prompt("Enter a number:"));
const number2 = parseInt(prompt("Enter another number:"));

window.alert(add(number1, number2));
```

## Debugging JavaScript
---

* The `Failed to load resource: net::ERR_FILE_NOT_FOUND` means that a file can't be found. This can occur because the file doesn't exist, it's in a different directory than the one we specified, or its in the correct place but the name doesn't match the name specified.