## Terminology
<hr />

* **Chaining methods**:  Calling a method directly on the return value of another method.

```javascript
"foo".concat("bar").toUpperCase();
```

* **Concatenation**:  Combining two strings together into one string. You can combine strings with `+` instead of `concat()`. This is still known as **concatenation** despite not using the `concat()` method:

```javascript
"I love" + " " + "Epicodus";
```

## Methods
<hr />

A few useful string methods:

* `charAt` — Returns the character at a particular location in a String.
* `toUpperCase` — Converts a string to uppercase.
* `toLowerCase` — Converts a string to lowercase.
* `concat` — Combines two strings.

A few useful number methods:

* `toString` — Converts a number into a string.
* `toFixed` — Converts a number into a string with only the number of decimal points that is specified in the argument.

## Other Notes
<hr />

You can call methods on strings or numbers, or variables assigned to strings or numbers:

```javascript
"supercalifragilisticexpialidocious".toUpperCase();
const word = "foo";
word.concat("bar");
```

You might wonder how we were able to use `concat` with a constant, but this method (and most others) doesn't change what's known as the **receiver** — the thing that a method is being called on. In the example above, `word` is the receiver. And if we check the value of `word`, it's still `"foo"`, not `"foobar"`. We would need to assign the return value of the expression above to a new variable for `"foobar"` to be saved.
