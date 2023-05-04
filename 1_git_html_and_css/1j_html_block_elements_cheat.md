## Terminology
<hr />

* **Block elements**: HTML elements that create a "block" in the display by appearing on their own line.

* **Tags**: HTML annotations which indicate how the text should be formatted.

* **P tag**: An HTML tag that indicates text should be formatted in a paragraph.

* **Opening tag**:  An HTML tag that appears before the text that will be formatted in an  HTML document.  For example, the `<p>` in ` <p> This is a paragraph. </p>` is the opening tag.

* **Closing tag**: An HTML tag that appears after the text that is formatted.  It matches the opening tag but begins with a `/`.  For example, the `</p>` in ` <p> This is a paragraph. </p>` is the closing tag.

* **End tag**:  An alternative name for a closing tag.

* **Heading**:  An HTML tag to indicate the text being formatted is a heading.  There are 6 sizes of HTML headings `<h1>` through `<h6>`.

* **Whitespace**:  All of the "empty" space that includes spaces, indentation, blank lines, etc.

* **Unordered list**: A list of items that are designated with bullet points.

* **Ordered list**: A list of items designated with numbers.

* **List item**:  An item in an ordered or unordered list.

## HTML block Element Tags
<hr />

*  **`<head>`**:  Head

*  **`<body>`**:  Body

*  **`<p>`**:  Paragraph

*  **`<ul>`**:  Unordered list

*  **`<li>`**:  List item (must exist within a set of `<ul>` or `<ol>` tags)

*  **`<ol>`**:  Ordered list

*  **`<h1>`** through **`<h6>`**:  Headings

*  **`<title>`**:  Title

## Example
<hr />

<div class='filename'>my-first-webpage.html</div>

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <title>Web page #1!</title>
</head>
<body>
  <h1>My first web page</h1>
  <h2>Written with the guidance of Epicodus</h2>

  <p>This is my first web page!</p>
  <p>Isn't it nice?</p>

  <p>Here are some things I'm going to learn about coding:</p>
  <ul>
    <li>HTML</li>
    <li>CSS</li>
    <li>JavaScript</li>
    <li>And a lot more!</li>
  </ul>
</body>
</html>
```
