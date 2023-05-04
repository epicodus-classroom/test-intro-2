## Examples
---

If we had the following form containing a group of checkboxes:

<div class="filename">transportation_survey/index.html</div>

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <title>Transportation Survey</title>
  <link href="css/styles.css" rel="stylesheet" type="text/css">
  <script src="js/scripts.js"></script>
</head>
<body>
  <h2>Transportation Survey</h2>
  <form id="transportation_survey">
    <p>In the past year, I have used the following modes of transportation to travel to work or school:</p>
    <label>
      <input type="checkbox" name="transportation-option" value="bike">
      Riding a bike.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="car">
      Driving a car.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="carpool">
      Carpooling with others.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="walk">
      Walking.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="bus">
      Riding the bus.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="train">
      Riding the train.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="streetcar">
      Riding the streetcar.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="taxi">
      Taking a taxi.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="rideshare">
      Using a rideshare service like Lyft or Uber.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="skateboard">
      Skateboarding.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="rollerblade">
      Rollerblading.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="scooter">
      Riding a scooter.
    </label><br />
    <label>
      <input type="checkbox" name="transportation-option" value="other">
      Another mode of transportation not listed here.
    </label><br />
    <button type="submit">Submit Survey</button>
  </form>
</body>
</html>
```

This JavaScript would retrieve all selected checkboxes, create a heading for the survey results, and append their values to a span in our HTML:

<div class="filename">transportation_survey/js/scripts.js</div>

```javascript
function handleForm(event) {
  event.preventDefault();
  const userSelections = document.querySelectorAll("input[name=transportation-option]:checked");
  const userSelectionsArray = Array.from(userSelections);

  const resultsHeading = document.createElement("h2");
  resultsHeading.append("You use the following methods of transportation to travel to work or school:");
  document.body.append(resultsHeading);

  userSelectionsArray.forEach(function(element) {
    const paragraph = document.createElement("p");
    paragraph.append(element.value);
    document.body.append(paragraph);
  });
}

window.addEventListener("load", function() {
  document.querySelector("form#transportation_survey").addEventListener("submit", handleForm);
});
```

* `event.preventDefault()` is added to prevent the 'submit' event's default action of refreshing the page.
* `const userSelections = document.querySelectorAll("input[name=transportation-option]:checked");` is added to get all of the checkbox inputs that have been checked. We could instead pass in these arguments to the `document.querySelectorAll()` method:
  * `"[name=transportation-option]:checked"`
  * `"input:checked"`
  * Whatever you choose really depends on what's easiest to read so that your code is easy to understand, and what other inputs and forms you have in your webpage.
* We turn the variable `userSelections` which is a `NodeList` object into an array with: `const userSelectionsArray = Array.from(userSelections);`
* We call `Array.prototype.forEach()` on the `userSelectionsArray` variable, passing in a callback function as the argument to the method.

### The Callback Function

The callback function is as follows:

```js
function(element) {
  const paragraph = document.createElement("p");
  paragraph.append(element.value);
  document.body.append(paragraph);
}
```

The `element` parameter is the placeholder for the actual array element. Each element in our array is an `HTMLInputElement` with a `value` property that gets the value of the input. So, for every element in our array, we: 

* Create a new HTML paragraph element, with `const paragraph = document.createElement("p");`.
* Add the input's value (`element.value`) as the text to that paragraph element, with `paragraph.append(element.value);`. 
* Add the new paragraph to the inside/end of our document's body tag with `document.body.append(paragraph);`. 

## An Alternate Way of Organizing Checkboxes
---

The following organization of checkboxes connects the label and the input by giving the same value to the `for` (on the label) and `id` (on the input) attributes:

```html
<label for="bike">Riding a bike.</label><br />
<input type="checkbox" name="transportation-option" value="car" id="car">
<label for="car">Driving a car.</label><br />
<input type="checkbox" name="transportation-option" value="carpool" id="carpool">
<label for="carpool">Carpooling with others.</label><br />
<input type="checkbox" name="transportation-option" value="walk" id="walk">
<label for="walk">Walking.</label><br />
<input type="checkbox" name="transportation-option" value="bus" id="bus">
<label for="bus">Riding the bus.</label><br />
<input type="checkbox" name="transportation-option" value="train" id="train">
<label for="train">Riding the train.</label><br />
<input type="checkbox" name="transportation-option" value="streetcar" id="streetcar">
<label for="streetcar">Riding the streetcar.</label><br />
<input type="checkbox" name="transportation-option" value="taxi" id="taxi">
<label for="taxi">Taking a taxi.</label><br />
<input type="checkbox" name="transportation-option" value="rideshare" id="rideshare">
<label for="rideshare">Using a rideshare service like Lyft or Uber.</label><br />
<input type="checkbox" name="transportation-option" value="skateboard" id="skateboard">
<label for="skateboard">Skateboarding.</label><br />
<input type="checkbox" name="transportation-option" value="rollerblade" id="rollerblade">
<label for="rollerblade">Rollerblading.</label><br />
<input type="checkbox" name="transportation-option" value="scooter" id="scooter">
<label for="scooter">Riding a scooter.</label><br />
<input type="checkbox" name="transportation-option" value="other" id="other">
<label for="other">Another mode of transportation not listed here.</label><br />
```
