## Using DevTools Console
<hr />

* _Always_ have the DevTools console open when debugging.

* In the console, errors that need to be fixed show up in red while warnings (that don't need to be fixed immediately) show up in yellow.

* The `Uncaught ReferenceError` means that a variable can't be found. Either it hasn't been defined yet or it doesn't exist. In the example we covered this error happened when we incorrectly entered `wndow` into the DevTools console:

```js
> wndow.innerWidth;
Uncaught ReferenceError: wndow is not defined at <anonymous>:1:1  VM70:1
```

* If you are running into an issue (like an undefined value) and there is no error message, a helpful starting point is to compare what you expect from the code you wrote to the actual result. Always start by reviewing the code you just wrote. This is the example we looked at involved a typo in the property name:

```js
> window.innerHeigt;
undefined
```