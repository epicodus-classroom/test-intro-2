## JavaScript Data Types — Objects
---

You should understand this about objects: 

* Objects represent things and concepts, like cats, grocery bags, and shopping carts. 
* Objects bundle distinct and separate pieces of data into one package.
* Data is separated and saved into properties that have values; this is why objects are considered to be collections of properties.
* Objects can hold many pieces of data of any data type.
* Objects describe both what something is and what it can do.

### Objects versus Primitives

Primitives can only represent a singular piece of data and type, like the number `9` or the boolean `true`.

Primitives also can't do anything. This is because we can't assign methods to primitives.

### Methods versus Functions

Methods belong to objects. In other words, when a function belongs to an object, we call it a method. Also, we always have to call the method on an object of the same type it belongs to. This means we can call a string method only on strings and not any other object type.

## JavaScript Turns (Some) Primitives into Objects
---

JavaScript strings, numbers, and booleans are implicitly turned into objects when we use them. JavaScript does this so that it can give these data types more complex and built-in functionality, like methods. This is also why we are able to call built-in methods on strings, numbers, and booleans — it's because they have been turned into objects.

## Documentation on Built-In JavaScript Objects
---

Standard Built-In Objects:

* **<span class="glyphicon glyphicon-link"></span> [Standard built-in objects](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects)**

Scroll through the page (linked above) and find these objects:

* String — categorized as "text processing"
* Number — categorized as "numbers and dates"
* Boolean — categorized as "fundamental objects"

## Conventions
---

**Going forward, we won't worry about distinguishing between the primitive or the object of data types like strings, booleans, and numbers. It's not important.** However, knowing the difference between primitives and objects helps us better understand how JavaScript is structured and how to use the MDN documentation.
