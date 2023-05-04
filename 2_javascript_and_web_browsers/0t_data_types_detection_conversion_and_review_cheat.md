## JavaScript Data Types — Primitives
---

* **Boolean**: `true` or `false`.

* **Number**:  A numerical value, like `5`, `8.39`, `-Infinity`, or `NaN`.

* **String**:  Content inside of quotes. Such as `"This is a string!"`.

* **Undefined**:  An object (such as a variable) without a defined value.

* **Null**:  For now, know that this represents nothingness. We'll explore this more later.

## Functions and Methods for Data Type Conversion
<hr />

* `parseInt()`:  Converts a string to a number.

* `Number.prototype.toString()`:  Converts a number to a string.

* `Boolean.prototype.toString()`:  Converts a boolean to a string.

## Examples
<hr />

### Data Type Detection
To check the data type of a variable or value:

```javascript
> typeof 5;
"number"
```

### Data Type Conversion
To convert a string to a number:

```javascript
> const myNumber = parseInt("42")
> myNumber;
42
```

To convert a number to a string:

```javascript
> const convertedNumber = 42..toString();
> convertedNumber;
"42"
```

To convert a boolean to a string:

```javascript
> const convertedBool = true.toString();
> convertedBool;
"true"
```
