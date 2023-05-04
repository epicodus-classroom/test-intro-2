## Terminology
<hr />

* **CSS**:  Stands for Cascading Style Sheets. A language used to program the visual appearance of HTML elements.

* **Rule**:  A block of CSS that details particular stylistic instructions to be applied to an HTML element.

* **Selector**:  The part of a CSS rule that determines which HTML elements the rule applies to.

* **Declaration Block**:  Designated by curly brackets `{ }`, this is where we define the CSS styles. 

* **Property**:  The characteristic a CSS rule is altering. (For example, `color`, or `font-size`).

* **Value**:  The attribute a CSS rule is applying to the specified property.

* **Declaration**: The combination of a property and value together, for example `color: blue`; every declaration block can have multiple declarations separated by a semicolon `;`.

## Inline Styles Examples

* **Inline Styles**: CSS styles listed directly within the HTML body. To add inline styles, you need to add a `style` attribute to the element that you wish to style. 
  * **Note:** We won't use inline styles frequently.

```html
  <h1 style="color:blue;background-color:hotpink">My favorite things</h1>
```

## External Stylesheet Examples
<hr />

* **External Stylesheet**: CSS styles listed in a separate `.css` file. 
* Even though we can set inline styles for our HTML elements using the `style` attribute, it's best practice to list CSS styles in a separate file (with a `.css` extension) for these reasons:
  * We can set styles that apply to multiple elements.
  * When we separate our code into multiple files, it's easier to read and update. 

### Linking to an External Stylesheet from HTML Document

To tell an HTML document to use a `css/styles.css` file for your website's CSS styles, add a new `<link>` tag to the `<head>` tags of our document: 

<div class="filename">favorite-things.html</div>

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <link href="css/styles.css" rel="stylesheet" type="text/css">
  <title>Michael's favorite things</title>
</head>
<body>
  ...
</body>
</html>
```

**HTML Link elements** direct our HTML document to load resources stored in separate files:

* To specify where the resource is located, we give a value to the `href` attribute that contains the path to our file. Our `href` attribute contains `css/styles.css` as the value, because _in relation to this favorite-things.html file_, the `styles.css` file is in a subdirectory named `css`. 
  * If the `styles.css` file were in the same directory as the favorite-things.html file, then the link would just be to `"styles.css"` rather than to `"css/styles.css"`.
* To describe what type of resource we're loading we specify two additional attributes:
  * `rel` specifies the relationship of the resource to our HTML document. In this case, the external resource is a `stylesheet`!
  * `type` specifies the media type of the resource. We list `text/css` because our resource is a CSS stylesheet.

### Example CSS Rules in an External Stylesheet

<div class="filename">styles.css</div>

```css
h1 {
  color: #0000ff;
  text-align: center;
}

h2 {
  font-style: italic;
  text-align: center;
}

p {
  font-family: sans-serif;
}

ul {
  font-size: 20px;
  line-height: 30px;
}
```

In the code above...

* Each individual block is a **rule**.
* `h1`, `h2`, `p`, and `ul` are all **selectors**.
* `color`, `text-align`, `font-style`, `font-family`, `font-size` and `line-height` are all **properties**.
* `blue`, `center`, `italic`, `sans-serif`, `20px` and `30px` are all **values**.
* The entire file `styles.css` is a **stylesheet**.

## Additional Resources
<hr />

* [W3School's CSS Reference](https://www.w3schools.com/css/default.asp)
* [MDN Web Doc's CSS Reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
* [CSS Zen Garden](http://csszengarden.com/)