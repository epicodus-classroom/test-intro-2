## Terminology
<hr />

* **Media query**:  A block of CSS applied only when certain conditions about the size or type of screen/window a user is viewing our content with are true. (i.e.: CSS associated with a media query with a max-width of 500px would only apply its styles when the viewport width is below 500px).

* **Breakpoint**:  The point at which a media query's condition becomes true. A media query with a max-width of 500px will apply its styles when the viewport is less than 500px. 500px is then the break point.

* **Viewport**:  The tool a user is viewing content with. Usually a browser window on a computer, phone, or tablet.

* **Responsive web design**:  An approach to web design focused around providing the best viewing and navigation experience for the specific device and screen size a user is viewing content with.

* **Media types**:  The type of media device the user is viewing content with (such as print, screen, handheld, or all)

* **Media features**:  Specific properties about the manner the user is viewing content; including width and height of viewport, orientation of device, etc.

## Examples
<hr />

The following query will make the background red and text white when the browser window has a width below 768px:

```css
@media screen and (max-width:  768px)  {
    body {
        background:  #FF6347;
        color: #FFF;
    }
}
```

In the code above:

* `screen` is the **media type**.
* `768px` is the **breakpoint**.
* `max-width` is a **media feature**.
* `body` is a **selector**.
* `background` and `color` are **properties**.
* `#FF6347` and `#FFF` are **values**.

## Additional Resources
<hr />

* Mozilla Developer Network — [Using media queries](https://developer.mozilla.org/en-US/docs/Web/CSS/Media_Queries/Using_media_queries)
* Mozilla Developer Network — [@media](https://developer.mozilla.org/en-US/docs/Web/CSS/@media)
* Example usages of media queries — [Mediaqueri.es](http://mediaqueri.es/)
