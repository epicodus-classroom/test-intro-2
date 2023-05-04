## Terminology
---

**Object**: a common data type in programming, objects are a collection of properties. Properties can be given a value of any data type, including other objects and methods. Objects are a data type in JavaScript as well as many other languages. Web browsers use objects to represent browser features like a browser window, which is represented by the `window` object. 

**dot notation**: we use dot notation to access object properties, which follows this syntax:

```js
// This is not real code! 
// This is pseudocode to explain the syntax of dot notation.
object.property 
```

Where `object` is the name of the object and `property` is the name of the property.

**nested objects**: an object is nested inside of another object when we set the value of an object's property to another object. `window.location` is a nested object inside of the `window` object.

**optional parameters**: methods can have optional parameters, which means that we can call those methods with and without passing in arguments for those parameters. Here's an example:

```js
// opens a new browser window or tab.
> window.open();
// opens a new browser window or tab to a specific website
> window.open("https://www.learnhowtoprogram.com/tracks");
```

## Sample code
---

```js
> window.innerHeight;
655
> window.innerWidth;
1123
> window.location.reload(); // calling this method will reload the page
```

### Conventions

Object and property names are written in lower camelCase.

