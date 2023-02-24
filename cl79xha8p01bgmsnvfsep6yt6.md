# Callback Hell - JavaScript

Before diving into the central concept i.e. Callback Hell, let's first understand What is Callback and why it is used?

“a callback is a function passed as an argument into another function”

Callbacks ensure that a function does not run before a task is completed, but only after the task has been completed. It aids in the development of asynchronous JavaScript code and protects us from problems and errors.

callbacks are superpowerful asynchronous operations to run your code.

Now, Let’s understand the CallBack Hell

Callback Hell is one of the issues we face while writing Asynchronous code in JavaScript. Another problem that we face is the Inversion of Control. So, What is Callback Hello?

Asynchronous operations in JavaScript can be achieved through callbacks. Whenever there are multiple dependent Asynchronous operations it will result in a lot of nested callbacks. This will cause a ‘pyramid of doom’ like structure.


![1_44rK1Neb2E2P7zbDCkyl8A.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661485183412/0ebnheNtJ.png align="left")

Let’s take an example here to understand better about the callback hell. Here is a code of e-commerce. let’s suppose we are working with the API to call the function and there will be functions like createOrder(), proceedToPayment(), and orderSummary().


![1_gg2OY6UXygQB_rCLT1LnQw.png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661485195828/NmVoEKO9X.png align="left")

Now, you have understood this example, where you can see the callback are nested inside one another. this creates a callback hell. Developers face big issues while dealing with the callback hell. Sometimes we can able to understand the code .i.e working behind the code.

Issues with the callback:-

1. Callback hell: callback inside another callback and a lot of nested loops become unmaintainable.
2. Inversion control: when we lose our program while giving control of our function to another function and we are not sure about that function is ever gonna execute or not.

I hope this article will give you an understanding of Callback Hell if you like this article please click on the like button and subscribe to my profile. so that you can get more updates related to JavaScript.

Thanks for Reading! 😃
