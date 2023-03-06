---
title: "Mastering Debugging with console.log()  in JavaScript"
datePublished: Sun Mar 05 2023 07:05:23 GMT+0000 (Coordinated Universal Time)
cuid: clev1tvol000909l6exjk6teq
slug: mastering-debugging-with-consolelog-in-javascript
cover: https://cdn.hashnode.com/res/hashnode/image/upload/v1677999884542/08323a95-0d60-490a-ab67-30a4ab74f6ea.png
ogImage: https://cdn.hashnode.com/res/hashnode/image/upload/v1677999915063/fdc32dc3-a528-4a0c-b447-081624bbeb2d.png
tags: javascript, consolelog

---

## Introduction

When it comes to debugging in JavaScript, console.log() is one of the most commonly used functions. It allows developers to log messages, variables, and objects to the console, providing insights into how their code is executing. In this article, we’ll explore the top 13 [console.log(](https://javascript.info/devtools)) statements in JavaScript and provide examples of how to use them.

## Log a simple message to the console:

```javascript
console.log("Hello, world!");
```

This statement prints "Hello, world!" to the console.

## Print the value of a variable to the console:

```javascript
let name = "John";
console.log(name);
```

This statement prints the value of the `name` variable to the console, which in this case is "John".

## Print a string with the value of a variable to the console:

```javascript
let age = 25;
console.log("I am " + age + " years old.");
```

This statement prints "I am 25 years old." to the console.

## Use template literals to print a string with the value of a variable:

```javascript
let city = "New York";
console.log(`I live in ${city}.`);
```

This statement prints "I live in New York." to the console.

## Print the type of a variable to the console:

```javascript
let number = 42;
console.log(typeof number);
```

This statement prints "number" to the [console](https://javascript.info/devtools), indicating that the `number` variable is of type number.

## Print a message when a function is called:

```javascript
function greet(name) {
  console.log(`Hello, ${name}!`);
}
greet("John");
```

This statement logs "Hello, John!" to the console when the `greet()` function is called.

## Print a message with the returned value of a function:

```javascript
function add(a, b) {
  let result = a + b;
  console.log(`The result is ${result}.`);
  return result;
}
add(2, 3);
```

This statement logs "The result is 5." to the console and returns the value 5.

## log an error message to the console:

```javascript
console.error("Oops! Something went wrong.");
```

This statement logs an error message to the console.

## Log a warning message to the console:

```javascript
console.warn("Warning! This action cannot be undone.");
```

This statement logs a warning message to the console.

## Print the contents of an array to the console:

```javascript
let numbers = [1, 2, 3, 4, 5];
console.log("Array contents: ", numbers);
```

This statement logs "Array contents: \[1, 2, 3, 4, 5\]" to the console.

## Print the contents of an object to the console:

```javascript
let person = { name: "John", age: 25 };
console.log("Person details: ", person);
```

This statement logs "Person details: {name: 'John', age: 25}" to the console.

## Log the time taken to execute a block of code:

```javascript
console.time("Code execution time");
// Code to be timed
console.timeEnd("Code execution time");
```

This statement logs the time taken to execute the block of code between `console.time()` and `console.timeEnd()`.

## Log the number of times a particular code block has been executed:

```javascript
for (let i = 0; i < 5; i++) {
  console.count("Code block executed");
}
```

This statement logs the message "Code block executed: 1

## Conclusion

console.log() is a powerful tool in JavaScript that allows developers to log messages, variables, and errors to the console during runtime. It is a simple and effective way to debug code, monitor variable values, and provide useful information about the code's behavior.

Developers can use different console methods to format messages and debug information in different ways, making it easier to identify and fix issues in their code. Additionally, console.log() can be used in various environments, including web browsers and Node.js, making it a versatile tool for developers to use.

Overall, console.log() is an essential feature in JavaScript that can help developers to write more efficient and effective code by allowing them to easily track and monitor the behavior of their programs.