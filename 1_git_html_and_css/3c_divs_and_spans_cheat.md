## Examples
<hr />

Group elements together with similar styles using `<div>`s. For example, change this:

<div class="filename">stuff.html</div>

```html
<h2 class="important">You better read this</h2>
<p class="important">Here are the things you really need to know.</p>
<img class="important" src="scary.png" alt="This is what will happen if you don't read it.">
```

to this:

<div class="filename">stuff.html</div>

```html
<div class="important">
  <h2>You better read this</h2>
  <p>Here are the things you really need to know.</p>
  <img src="scary.png" alt="This is what will happen if you don't read it.">
</div>
```

Create in-line styles using `<span>`s:

<div class="filename">different.html</div>

```html
<p>Something is <span class="special">different</span> in this sentence.</p>
```

Style `<div>`s and `<span>`s just like you would any other element, without explicitly using `div` or `span` in the selector:

<div class="filename">styles.css</div>

```css
.important {
  color: red;
}
```

## CSS Sizing Units
---

In the following video, we cover:

* `px` for pixels, which sets an element to a fixed size on the page.
* `%` for percentage, which sets an element to a percentage of its parent element.
* `vh` or `vw`, which sets an element to a percentage of the viewport's width or height. The **viewport** is the area of a webpage that's visible to a user.
* `em` or `rem`. Using `em` sets the size of an HTML element relative to its parent element's font-size. Using `rem` sets the size of an HTML element relative to the root element's font-size. We won't use `em` or `rem` in the program, so further exploration is up to you.
* We'll also learn how `%`, `vh`, `vw`, `em`, and `rem` are sizing units that are **responsive**, which means they are not fixed sizes, but change based on the size of HTML elements that they are relative to.

<p align="center">
  <iframe title="vimeo-player" src="https://player.vimeo.com/video/778165971?h=786697deea" width="640" height="360" frameborder="0" allowfullscreen></iframe>
</p>