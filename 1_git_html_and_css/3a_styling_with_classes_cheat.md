## Terminology
<hr />

* **Lorem ipsum**: Text that is used as filler to display or demonstrate an area of text; it looks like Latin and allows the user to focus on the overall layout without focusing on the meaning of words.  Fun fact: "lorem ipsum" derives from the Latin for "pain itself".

* **`class` attribute**: Does not have to be unique and can be applied to multiple elements. Classes are used to group one or more elements.
  * When referencing **classes** in CSS, use: `.` (e.g. `.intro`)

* **`id` attribute**: Must be unique and can only be applied to one element. Ids are used to distinguish one element from the rest.
  * When references **ids** in CSS, use: `#` (e.g. `#line2`)

## Examples
<hr />

<div class="filename">webpage-with-classes.html</div>

We can add one or more classes to one or more elements, but we can only add one id to an element and it must be unique in the webpage.

```html
<p class="important emphasize">Important stuff should be:</p>
<ul class="important">
  <li>red,</li>
  <li>bold, and</li>
  <li id="large">big, but only for paragraphs.</li>
</ul>
```

Create CSS rules for that class:

<div class="filename">styles-for-classes.css</div>

```css
.important {
  color: red;
}

.emphasize {
  font-weight: bold;
}

#large {
  font-size: 40px;
}
```

To create a CSS rule for only a specific a tag with a class:

<div class="filename">styles-for-classes.css</div>

```css
p.important {
  font-size: 24px;
}
```