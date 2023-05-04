## JavaScript Conventions
---

### Use `let` or `const` to Declare Variables

* Do not use `var` to declare variables, because it is outmoded. Instead use [`let` or `const`](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements#declarations), which both have improved scoping. We'll revisit scope later in this section.

### Use Lower camelCase in Variable Names

* Variable names should always be written in [lower camelCase](https://developer.mozilla.org/en-US/docs/MDN/Guidelines/Code_guidelines/JavaScript#variable_naming), where there are no spaces in the name, the first letter is lowercase, and the first letter of every subsequent word in the variable name is uppercase.
* Variable names need to begin with a letter
* Variable names are case sensitive. This means,  `myNumber` is a _different_ variable than `myNUMBER`.

### Use Descriptive Names for Variables

* Make sure the name you use to for a variable is descriptive of what it represents: its data type, its value, or purpose in the code.

### Use Semicolons after Statements and Expressions

* Semicolons are used to indicate the end of a statement.
* JavaScript automatically adds semicolons to our JS code, and this is called "automatic semicolon insertion". However, in some cases this can break our code, and the situations in which this happens can be tricky to learn. Because of this, **at Epicodus we add semicolons at the end of (most) statements and expressions.**
* A [**statement**](https://developer.mozilla.org/en-US/docs/Glossary/Statement) is a piece of code that tells our computer to do something. A computer program is essentially made up of a list of statements. Statements can contain operators, keywords, and expressions.
* [An **expression**](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#expressions) is a piece of code that evaluates to a value. 
* The difference between statements and expressions can get technical and detailed. However in simple terms we can distinguish the two like so: expressions are a piece of code that evaluates to a value, a "statement" is used more generally to describe code that performs actions, whether or not they evaluate to a value. 