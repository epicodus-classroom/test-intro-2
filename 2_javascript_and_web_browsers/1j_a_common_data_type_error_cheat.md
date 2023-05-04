## Summary
<hr />

* All values returned from a prompt are saved as strings.

* To collect a value from a user with `window.prompt()`, and perform arithmetic with this value, we need to convert it into a number with JavaScript's [`parseInt()` function](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/parseInt). If not, we'll receive some very unexpected output.

* The *Int* part of `parseInt()` is short for integer, which means it's a whole number. If we wanted to convert something into a number with a decimal, we'd use `parseFloat()`. Floating point numbers are numbers with decimals. We'll explore these more later! 

* Data type coercion in JavaScript is when JavaScript decides on its own to force a piece of data to change into another data type. We see data type coercion come up when we use JavaScript arithmetic, comparison, and equality operators on incompatible data types. Here are a bunch of examples:

```js
> true + true;
2;
> true + false;
1;
> false - false;
0;
> true * false;
0
> true * 6;
6
> true + " or false: do you like data type coercion?";
"true or false: do you like data type coercion?"
> true * "false";
NaN
> "I am " + 54 + " years old.";
"I am 54 years old."
> 54 + " years old am I.";
"54 years old am I."
> 6 + 2 + 1 + 1 + "45";
"1045"
> "45" + 54 + 3;
"45543"
> "45" - 54 + 3;
-6
> "55" * 2;
110
> 10 / "2";
5
```