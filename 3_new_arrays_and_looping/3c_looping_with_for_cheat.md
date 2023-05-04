## Terminology
<hr />

* **For loop**: The "traditional" way to write loops in JavaScript. Creates a loop without needing to call a method on an array.

* **Initialization parameter**:  Initializes a variable with the denoted value, which usually is a number. This only happens once, when the loop is first triggered. It needs to be initialized with `let`. Usually this variable is called `index` or `i`, but it could be called anything, depending on what the loop is used for and what's most descriptive.

* **Condition parameter**:  Tells the loop under what conditions to _continue_ running the loop. As long as the condition is true, the loop will continue running.

* **Final expression parameter**: Usually changes the initial value in some way, often by incrementing or decrementing it.


## Examples
<hr />

Example `for` loop:

```javascript
sfor (let index = 1; index <= 3; index += 1) {
  console.log(index);
}
```
In the code above...

* `let index = 1;` is the **initialization parameter**.
* `index <=3;` is the **condition**.
* `index += 1` is the **final expression**.


Example of using a `for` loop with an array:

```javascript
const languages = ['HTML', 'CSS', 'Javascript'];
for (let index = 0; index < languages.length; index += 1) {
  console.log('I love ' + languages[index] + '!');
}
```
