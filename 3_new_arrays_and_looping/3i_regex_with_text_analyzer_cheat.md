## Code
---

We can **create**s a `RegExp` object like this:

```js
> const word = "red";
> const regex = new RegExp(word, "gi");
```

This is the best way to pass a variable into a regular expression.

We can **use** the `RegExp` object like this:

```js
> const text = "RED red red! Green GREEN green.";
> const word = "red";
> const regex = new RegExp(word, "gi");
> text.match(regex);
["RED", "red", "red"]
```

`numberOfOccurrencesInText()` with regex:

```js
function numberOfOccurrencesInText(word, text) {
  if (isEmpty(word)) {
    return 0;
  }
  const regex = new RegExp(word, "gi");
  return text.match(regex).length;
}
```