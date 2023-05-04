## Terminology
<hr />

* **Function:** A function is a bundle of code that performs a set of procedures.

* **Method:**  A method is a type of function. It is an action run on a piece of data; you can think of it as a message you send to a piece of data, and the result is the response.

* **Receiver:** The data that the method is called on. In the example below, `toUpperCase` is called on `"hi"` and `"hi"` is the receiver.

```js
> "hi".toUpperCase();
HI
```

* **Function declaration:** This is when we define what a function does — its "functionality". This is also called **function definition**. Here's an example:

```js
function addEmphasis(stringParam) {
  const result = stringParam.toUpperCase().concat("!!!");
  return result;
}
```

* **Return value:**  The return value is the method or function's response.

* **Argument:**  Some methods/functions take one or more arguments that provide the method/function with additional information to help it perform its action.

* **Parameter:**  This is a placeholder variable that is included in the definition of a function. There is no value for parameters. Once the function is called, an argument is passed into the parameter and gives it a value. Methods also can have parameters, but we won't create our own methods until Intermediate JavaScript.

* **Parens:** A shorthand for saying parentheses.

* **Calling a function/method:** This means that we are executing a function/method's actions. We must include parentheses at the end of a function/method name to call a function/method. Here's an example method call and function call:

```js
// calling the toUpperCase method
"hello".toUpperCase()
```

```js
// calling the addEmphasis function
addEmphasis("I love cats");
```