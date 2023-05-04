## Tips
---

* Marking your HTML input field as _number_, _date_, or _tel_, doesn't mean it will automatically be a JavaScript **number** type. `type="number"` just means that the form field will only accept number values. But when you access the `.value` property to get the input value, it will still come in as a JavaScript _string_, not a _number_.

## Resources
---

* **<span class="glyphicon glyphicon-link"></span> [MDN Reference Page on the HTML `<input>` element](https://developer.mozilla.org/en-US/docs/Web/HTML/Element/input#input_types)** 
* **<span class="glyphicon glyphicon-link"></span> [An Article on Using HTML5 Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)** 
* **<span class="glyphicon glyphicon-link"></span> [Bootstrap's Styling Documentation for Forms](https://getbootstrap.com/docs/5.2/components/forms/)** 

## Code Examples
---

### Select Boxes

![select-boxes-form-input-type](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/INTRO/week2-js-jquery/select-box-form-input.png)

#### HTML

```html
<form id="select-form">
  <select id="beverage">
    <option>Coffee</option>
    <option>Tea</option>
    <option>Kombucha</option>
    <option value="4">Water</option>
  </select>
  <button type="submit">Submit Selection</button>
</form>
```

* We can optionally set a `value` attribute to give our `<option>` a different value that the text. For example, the option for "Water" will now have a value of the string `"4"`.

#### JavaScript

```javascript
function handleSelect(event) {
  event.preventDefault();
  const selection = document.getElementById("beverage").value;
}

window.addEventListener("load", function() {
  document.getElementById("select-form").addEventListener("submit", handleSelect);
});
```

### Radio Buttons

![form-input-types-radio-buttons](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/INTRO/week2-js-jquery/radio-button-form-input.png)

#### HTML

```html
<form id="radio-form">
  <label>
    <input type="radio" name="flavor" value="chocolate" checked>
    Chocolate
  </label><br />
  <label>
    <input type="radio" name="flavor" value="vanilla">
    Vanilla
  </label><br />
  <label>
    <input type="radio" name="flavor" value="cookies and cream">
    Cookies & Cream
  </label><br />
  <button type="submit">Submit Selection</button>
</form>
```

Or, not nesting the `<input>` elements and appropriately using `for` and `id` attributes:

```html
<form id="radio-form">
  <input type="radio" name="flavor" value="chocolate" id="choc" checked>
  <label for="choc">Chocolate</label><br />
  <input type="radio" name="flavor" value="vanilla" id="van">
  <label for="van">Vanilla</label><br />
  <input type="radio" name="flavor" value="cookies and cream" id="cookies">
  <label for="cookies">Cookies & Cream </label><br />
  <button type="submit">Submit Selection</button>
</form>
```

* `checked` is used to check a radio button by default.
* Including the same `name` attribute and value on every radio button input is crucial to the function of this form type. The `name` attribute groups all of the radio buttons together in order to ensure that only one radio button is selected at a time.

#### JavaScript

```javascript
function handleRadio(event) {
  event.preventDefault();
  const radioSelection = document.querySelector("input[name='flavor']:checked").value;
}

window.addEventListener("load", function() {
  document.getElementById("radio-form").addEventListener("submit", handleRadio);
});
```

`"input[name='flavor']:checked"` is a newer, more complicated query selector. Let's break this down:

* `input` targets any inputs in the DOM
* `[name='flavor']` tells the querySelector method to look only at elements with a `name` attribute set to `'flavor'`. This ensures that we're looking at all of our radio button inputs, which all share the same `name` attribute and value.
* `:checked` makes sure that we grab the value of only the radio input that is checked.

### Date Picker

![form-input-type-date-picker](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/INTRO/week2-js-jquery/date-select-form-input.png)

#### HTML

```html
<label for="born">Date of birth:</label>
<input id="born" type="date">
```

#### JavaScript

```javascript
const dob = document.getElementById("born").value;
```

### Color Picker

#### HTML

```html
<label for="color">What is your favorite color?</label>
<input id="color" type="color">
```

#### JavaScript

```javascript
const favoriteColor = document.getElementById("color").value;
```

## Button Types — A Review
---

The `type` attribute that we set for a `<button>` element will change how we can use it in our HTML. 

```js
<button type="submit">Submit Form</button>
```

A button with a `type` attribute set to `"submit"` is meant to be used in form elements and causes a submission event on a form. The default reaction to a submission event is to refresh the page. 

```js
<button type="button">Show More Information</button>
```

A button with a `type` attribute set to `"button"` makes the button element have no default behavior and do nothing when pressed by default. If we are targeting a submit event with an event listener and we use `type="button"` on our form's button, our code will break. This is because we can target a click event on a button with `type="button"`, but not a form submission event, so we cannot use `type="button"` in a button within an HTML form. Using `type="button"` on a button element is great for showing/hiding elements, or changing styles.

```js
<button>Click Me</button>
```

What about a `<button>` element with no `type` attribute specified? This comes down to context. When unspecified, the default `type` attribute value for buttons `type="submit"`. So, if the button is used in a form without a `type` attribute, we can still target and respond to a submission event. If a button is used outside of a form, we can also target and respond to a click event.
