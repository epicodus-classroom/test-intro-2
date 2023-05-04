## Terminology
<hr />

* **Test-Driven Development**: A workflow used by developers across coding languages. In TDD, we write tests that describe our application's behavior. Then we write the minimal amount of code we need to get the test passing. The goal is to break larger problems into more manageable steps and also to make sure our code is working correctly.

* **Tests**, **Specifications** or **Specs**:  Examples of small, isolated behaviors a program should demonstrate, including input and output examples. "Spec" and "test" are interchangeable terms.

## Example
<hr />

Here's an example of a pseudocode test:

```
Describe: wordCounter()

Test: "It should return 1 if a passage has just one word."
Code:
const text = "hello";
wordCounter(text);
Expected Output: 1
```

### Parts of a Test

* **Describe** is used to organize a group of tests, such as all tests for a specific function.

* **Test** is a description, in plain English, of what the test will do.

* **Code** is any code that needs to run in order to get the expected output.

* **Expected Output** is the output we expect for the test to correctly pass.