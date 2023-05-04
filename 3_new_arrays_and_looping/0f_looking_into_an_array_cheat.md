## Terminology and Examples
<hr />

**Index:** The index of an element in an array is its numerical position. The first element has an index of 0.

**OBOE:** An off-by-one error. Watch out for these!

**bracket notation:** we can access array elements using square brackets `[]` and entering in the index:

```javascript
> const letters = ['a', 'b', 'c'];
> letters[0];
'a'
```
Start counting elements at 0.

**the `length` property:** you can check the length of an array by accessing its `length` property:

```js
> letters.length
3
```

**You can get elements from the end of an array like this:**

```js
> letters[letters.length - 1]
'c'
```