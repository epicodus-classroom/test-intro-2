## Examples
<hr />

### Logging Values to the Console:

```js
const array = [0,1,2,3,4,5];
array.forEach(function(number) { 
  console.log(number * 2);
});
```

### Creating a New Array with Modified Elements

```js
const array = [0,1,2,3,4,5];
let doubledArray = [];
array.forEach(function(element) {
  doubledArray.push(element * 2);
});
```

### Using a Loop to Sum Numbers

```js
const array = [0,1,2,3,4,5];
let sum = 0;
array.forEach(function(element) {
  sum += element;
});
```

### Using a Loop to Make a String

```js
let thingsILike = "I like...";
const arrayOfThingsILike = ["bubble baths", "kittens", "good books", "clean code"];
arrayOfThingsILike.forEach(function(thing) {
  thingsILike = thingsILike.concat(" " + thing + "!");
});
```

### Using A Loop to Add Elements to the DOM

```js
const arrayOfThingsILike = ["bubble baths", "kittens", "good books", "clean code"];
const ul = document.querySelector("ul#likable-things");
arrayOfThingsILike.forEach(function(thing) {
  const li = document.createElement("li");
  li.append(thing);
  ul.append(li);
});
```