## Terminology

---

**Don't Repeat Yourself**: Known as **DRY** for short. This is another essential programming concept. We should avoid repeating code where possible. There are a lot of good reasons not to repeat yourself:

* It results in unnecessary repeated code.
* It's harder to read and reason about because there's extra repeated code to deal with and read.
* If the code breaks or it needs to be updated, we have to change it in multiple places, not just one.

**Helper/Utility function:** A function, often small, with reusable code. We can use helper functions to DRY up our code by removing repeated code, moving it into the helper function, and then calling that helper function wherever that code is needed. Much less repetition!

## Code
---

### HTML

```html
<!DOCTYPE html>
<html lang="en-US">
<head>
  <title>Text Analyzer</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-rbsA2VBKQhggwzxH7pPCaAqO46MgnOM80zW1RWuH61DGLwZJEdK2Kadq2F9CUG65" crossorigin="anonymous">
  <link href="css/styles.css" rel="stylesheet" type="text/css">
  <script src="js/scripts.js"></script>
</head>
<body>
  <div class="container">
    <h2>Text Analyzer</h2>
    <form id="word-counter">
      <div class="form-group">
        <p>Input a text passage to get a total word count:</p>
        <textarea id="text-passage" name="text-passage" class="form-control"></textarea>
        <p>Optionally enter a word to count the number of times it occurs in the passage:</p>
        <input type="text" id="word" name="word" class="form-control">
        <br />
        <button type="submit" class="btn btn-success">Submit Survey</button>
      </div>
    </form>
    <p>Total Word Count: <span id="total-count"></span></p>
    <br />
    <p>Selected Word Count: <span id="selected-count"></span></p>
    <div id="bolded-passage">

    </div>
  </div>
</body>
</html>
```

### JS

```js
// Utility Logic

function isEmpty(testString) {
  return (testString.trim().length === 0);
}

// Business Logic

function wordCounter(text) {
  if (isEmpty(text)) {
    return 0;
  }
  let wordCount = 0;
  const textArray = text.split(" ");
  textArray.forEach(function(element) {
    if (!Number(element)) {
      wordCount++;
    }
  });
  return wordCount;
}

function numberOfOccurrencesInText(word, text) {
  if (isEmpty(word)) {
    return 0;
  }
  const textArray = text.split(" ");
  let wordCount = 0;
  textArray.forEach(function(element) {
    if (element.toLowerCase().includes(word.toLowerCase())) {
      wordCount++;
    }
  });
  return wordCount;
}

// UI Logic

function boldPassage(word, text) {
  if (isEmpty(word) || isEmpty(text)) {
    return null;
  }
  const p = document.createElement("p");
  let textArray = text.split(" ");
  textArray.forEach(function(element, index) {
    if (word === element) {
      const bold = document.createElement("strong");
      bold.append(element);
      p.append(bold);
    } else {
      p.append(element);
    }
    if (index !== (textArray.length - 1)) {
      p.append(" ");
    }
  });
  return p;
}

function handleFormSubmission() {
  event.preventDefault();
  const passage = document.getElementById("text-passage").value;
  const word = document.getElementById("word").value;
  const wordCount = wordCounter(passage);
  const occurrencesOfWord = numberOfOccurrencesInText(word, passage);
  document.getElementById("total-count").innerText = wordCount;
  document.getElementById("selected-count").innerText = occurrencesOfWord;
  let boldedPassage = boldPassage(word, passage);
  if (boldedPassage) {
    document.querySelector("div#bolded-passage").append(boldedPassage);
  } else {
    document.querySelector("div#bolded-passage").innerText = null;
  }
}

window.addEventListener("load", function() {
  document.querySelector("form#word-counter").addEventListener("submit", handleFormSubmission);
});
```