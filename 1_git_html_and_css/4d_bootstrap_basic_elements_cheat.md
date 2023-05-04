## Overview
<hr />

Here's a brief overview of the Bootstrap elements covered in this lesson:

### Container

A [container](https://getbootstrap.com/docs/5.2/layout/containers/) wraps content and adds padding. We can implement a container like this:

```html
<div class="container">
  ...
</div>
```

It's generally recommended to house the entirety of a document's `<body>` in a container, to provide padding to all content.

### Blockquotes

[blockquotes](https://getbootstrap.com/docs/5.2/content/typography/#blockquotes) are used to create nicely-formatted quote blocks. We can implement them like this:

```html
<figure>
   <blockquote class="blockquote">
      <p>"It's been really good working with you!"</p>
   </blockquote>
   <figcaption class="blockquote-footer">
      My partner the first day
   </figcaption>
</figure>
```

### Built-in Classes

We can use built-in classes to add formatting to almost any Bootstrap element. There are many different helper classes. One example is adding background color, which we can do like this:

```html
<p class="bg-success">This text has a green background!</p>
<p class="bg-danger">This text has a red background!</p>
```

To see all of the built-in classes for background colors, [visit the background color documentation](https://getbootstrap.com/docs/5.2/utilities/background/#background-color).

To see a list of the ways that we can style text, [visit the text color documentation](https://getbootstrap.com/docs/5.2/utilities/colors/) and the more general documentation for [text](https://getbootstrap.com/docs/5.2/utilities/text/).

### Cards

[card](https://getbootstrap.com/docs/5.2/components/card/) add a visual effect that makes content appear inset or embossed into the page. We can create a card like this:

```html
<div class="card">
   <div class="card-body">
   <h5 class="card-title">Command Line</h5>
   <ul class="card-text">
      <li>Navigating my documents through the command line.</li>
      <li>Creating new files and folders through the command line.</li>
      <li>Moving and deleting files and folders through the command line.</li>
      <li>Retrieving my current location from the command line.</li>
   </ul>
   </div>
</div>
```

There are other things we can add to a card, likes images and links, so make sure to check out the documentation for more information.