## The DOM
---

We reviewed information about the DOM that we already learned in previous lessons:

* The DOM is a Web API specification.
* The `document` object is the entry point to the DOM.
* The `document` object is a Web API interface.

We also learned new information about the DOM:

* The DOM is a tree made up of nodes, organized hierarchically. Each node is an object, so the HTML DOM is effectively a series of nested objects that stem from the `document` object.
* Just as we view our website within the browser window, the `document` object is nested inside of the `window` object. By definition a `window` object represents our current browsing context with an HTML DOM inside of it.

## Visualizations
---
 
### A Tree (Data Structure)
 
At its most basic, a tree consists of a root node that branches to child nodes, which in turn branch off into more child nodes. By default, nodes don't have any value — they can be of any data type. A node is just a data point along the tree, and it is always in relation to the nodes that it is connected to. The following image from [Wikipedia](https://en.wikipedia.org/wiki/Tree_(data_structure)) shows a tree with a root node of `2`, and a series connected and branching nodes, going downwards:
 
![This is an images of a tree data structure with a single root node at the top, and a series of child nodes.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/new-section2-js-and-web-browsers/tree-data-structure-from-wikipedia.png)
 
### HTML Document as Source Code and as DOM
 
This image shows one HTML document: on the left it is represented as source code, and on the right it represented as a Document Object Model. In the DOM tree, the root node is the `document` object (provided by the browser, like the `window` object), and every node that branches from the `document` object represents either an HTML element or text. **The `document` object** is the entry point to accessing the DOM, and all of the HTML, including HTML elements, attributes, and text.
 
![This image shows one HTML document as source code (on the left) and as a DOM (on the right).](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/new-section2-js-and-web-browsers/html-source-simple-with-tree.png)
 
### The DOM `document` Nested inside of `window`
 
The image shows the DOM tree next to the DOM in the browser. In the DOM tree, we can see that we've added `window` above `document`. Because trees show hierarchical relationships, what this means is that the `document` object is nested inside of the `window` object. Or, in other words, the `document` object is a property of the `window` object.
 
![This image shows a DOM tree with the root node as `window`, next to a browser window that shows two nested squares that represent the `document` object inside of the `window` object.](https://learnhowtoprogram.s3.us-west-2.amazonaws.com/new-section2-js-and-web-browsers/window-is-global-object.png)