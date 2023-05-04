## Terminology
<hr />

* **Inheritance**:  The process by which children elements share the properties of their parent elements. The **cascading** in cascading style sheets also refers to this phenomenon.

* **Specificity**:  In the instance that two styles conflict, the style that is applied will be the most specific of the two. For example, a style for a paragraph tag would not be applied if there was a style for a link within a paragraph.  The link within the paragraph reference is more specific than paragraph.

* **Inline style**:  Style that is added directly into the HTML for an element.  Inline styling takes precedence over styling in your CSS files.  It is not considered good practice to style HTML this way.

## Examples
<hr />

Elements inherit styles from their parents. This rule gives every element on the page the San Serif font:

```css
body {
  font-family: sans-serif;
}
```

You can nest selectors:

<div class="filename">nesting-styles.css</div>

```css
.sidebar p img{
  display: block;
}
```

<div class="filename">nesting.html</div>

```html
<div class="sidebar">
  <p>This image: <img src="whatever.jpg" alt="whatever"> will be on its own line.</p>
</div>
```

More specific rules take precedence over less specific rules:

<div class="filename">specificity-styles.css</div>

```css
p {
  background-color: green;
}

p.slow {
  background-color: yellow;
}

p.slow .stop {
  background-color: red;
}
```

<div class="filename">specificity.html</div>

```html
<p>This will have a green background.</p>
<p class="slow">This will have a yellow background. <span class="stop">And this a red background.</span></p>
```

## Tips
<hr />

* In the case of conflicting rules, the last one wins. There are more complicated rules that we won't get into.
