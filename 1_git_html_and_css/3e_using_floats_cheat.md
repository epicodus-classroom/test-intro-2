## Terminology
<hr />

* **Float**: A CSS option that assists in layout by allowing elements on the page to be placed next to each other in the layout (values include right or left).

## Examples
<hr />

Use floats to make elements float to one side of the page. Other elements will wrap around that element.

Float an image to the left:

<div class="filename">floating-image.html</div>

```css
<img class="main" src="img/walrus.jpg" alt="A walrus basking on a rock.">
```

<div class="filename">styles.css</div>

```css
img.main {
  float: left;
}
```

Create a sidebar:

<div class="filename">sidebar.html</div>

```html
<h1>Title</h1>
<div class="sidebar">
  <h2>Sidebar</h2>
  <p>Some sidebar stuff.</p>
</div>
<p>Main page stuff.</p>
```

<div class="filename">sidebar-styles.css</div>

```css
.sidebar {
  float: right;
}
```

Make a column layout:

<div class="filename">columns.html</div>

```html
<div class="column">
  <p>Column 1</p>
</div>
<div class="column">
  <p>Column 2</p>
</div>
<div class="column">
  <p>Column 3</p>
</div>
```

<div class="filename">column-styles.css</div>

```css
.column {
  width: 300px;
  float: left;
}
```
