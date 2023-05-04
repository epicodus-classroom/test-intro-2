## Terminology
<hr />

* **`for...of`**: A technique we can use to loop through arrays, strings, and other types of iterable objects.

## Examples
<hr />

### Example Using an Array

```js
const array = [0,1,2,3,4,5];
let doubledArray = [];
for (const element of array) {
  doubledArray.push(element * 2);
}
doubledArray;
(6) [0, 2, 4, 6, 8, 10]
```

### Example Using a String

```js
const consonantString = "bdfmxtgl"
let vowelizedString = "";
for (const letter of consonantString) {
  vowelizedString = vowelizedString.concat(letter + "a");
}
vowelizedString;
"badafamaxatagala"
```