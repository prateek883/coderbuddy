# Javascript Functions

## Introduction
When creating an application, you frequently need to perform the same action in multiple places. For instance, you might want to display a message whenever an error occurs.

To avoid repeating the same code in multiple places, you can wrap it in a function and reuse it.

Many built-in JavaScript functions, such as ```
parseInt()
``` and ```
parseFloat()
```, are available (). This tutorial will teach you how to create custom functions.

## Declare a function
To declare a function, use the function keyword, then the function name, a list of parameters, and the function body, as shown below:


```
function functionName(parameters) {
    // function body
    // ...
}
```

## Invoking a function
To use a function, you need to call it. Calling a function is also known as invoking a function. To call a function, you use its name followed by arguments enclosed in parentheses like this:

```
functionName(arguments);
```

When calling a function, JavaScript executes the code inside the function body. For example, the following shows how to call the say() function:

```
say('Hello World');
```

In this example, we call the say() function and pass a literal string 'Hello' into it.

## Parameters vs. Arguments

The terms parameters and arguments are often used interchangeably. However, they are essentially different.

When declaring a function, you specify the parameters. However, when calling a function, you pass the arguments that are corresponding to the parameters.

For example, in the ```
say()
``` function, the message is the parameter and the 'Hello'string is an argument that corresponds to the message parameter.


## Functions Hoisting

In JavaScript, you can use a function before declaring it. For example:


```
showMe(); // a hoisting example

function showMe(){
    console.log('Hello World');
}
```

This feature is called hoisting.

Function hoisting is a mechanism in which the JavaScript engine physically moves function declarations to the top of the code before executing them.

The following shows the version of the code before the JavaScript engine executes it:


```
function showMe(){
    console.log('Hello World');
}

showMe(); // a hoisting example
```


## Summary
In this blog, I just wanted to explore my knowledge related to functions. I hope you liked it.

Thanks for reading!