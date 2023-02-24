# Bun - JavaScript Runtime better than Deno and Node

## Introduction

Today [Bun](https://bun.sh/) has been a talking point for everyone regarding JavaScript runtime. Bun is the new fastest runtime compared to [Node.js](https://nodejs.org/) and [Deno.js](https://deno.land/). To understand more about [Bun.js](https://bun.sh/). Let's first understand the history of JavaScript.

## JavaScript Engine

A JavaScript engine is a computer program that interprets and executes JavaScript code. It takes the code written in JavaScript and converts it into machine-readable instructions that can be executed by the computer's hardware.

JavaScript engines are commonly found in web browsers, where they are used to execute JavaScript code that is embedded in web pages. They are also used in server-side environments, where they power back-end web applications and other server-side programs.

Some examples of popular JavaScript engines include V8 (used in Google Chrome and Node.js), SpiderMonkey (used in Firefox), and JavaScriptCore (used in Safari). Each engine has its own unique set of features and performance characteristics, but they all share the same basic goal of executing JavaScript code efficiently and accurately.

## What is a Bun?

Node.js and Deno, get out of here. The JavaScript/TypeScript runtime arena is seeing the emergence of Bun as a potential rival.

Bun, which is now in beta testing, is marketed as a contemporary JavaScript runtime similar to Deno or Node that is designed to start quickly, provide new levels of performance, and be a complete tool including a bundler, transpiler, and package manager. The Node module resolution technique is implemented by the NPM client included in Bun.

Bun is aspirational. The project's objective is to "execute much of the world's JavaScript outside of browsers," improving the infrastructure's performance and complexity.

## Getting started with Bun

Bun must first be installed before we may use it. The documentation for Bun states that only the following command is necessary for installation:

`curl https://bun.sh/install | bash`

This command only works for Mac and Linux for windows you need to follow the [windows subsystem for](https://docs.microsoft.com/en-us/windows/wsl/about) Linux.

After installation is complete, carefully read the confirmation popup for instructions on how to add Bun to your `PATH`. You must include the following lines in your `.bashrc` or `.zshrc` files to accomplish this:

`BUN INSTALL="/home/<username>/.bun"`

Now that you have installed it correctly, running the `bun --version` should print the version number.

# Write and Run the First Bun Script File

Create a file called script.js and add the following code inside the file:

```javascript
Bun.serve({
    fetch(request){
        return new Response("Hello Bun!")
    }
})
console.log("Listening on Port 3000")
```

`Bun.serve` - starts the server and accepts an object containing the server settings. The fetch property on the configuration object stores a function that receives the request object for each request.

By launching `Bun.serve` using the command bun run `script.js` and then navigating to [`localhost:3000`](http://localhost:3000) to view the outcome of our request, we may use this tool. The object supplied to `Bun.serve` can have a port property added if we wanted to modify which port it will serve on.

## Writing files with Bun

Bun's API for writing to files is quite basic. Let's change our script so that it creates a file each time a request is made:

```javascript
let count = 1
Bun.serve({
    fetch(request){
        Bun.write(`${count}.txt`, request.url)
        count += 1
        return new Response("Hello Bun!")
    },
})
console.log("Listening on Port 3000")
```

After you run the aforementioned code and go to [localhost:3000/cheese](http://localhost:3000/cheese), two new files, `1.txt` and `2.txt`, will have been created. The target of the write, such as a file or stdout, is the first argument to `Bun.write`, and the second argument is the content of the write.

## .env files with Bun

The capability to use `.env` files straight out of the box is another really great addition. You don't need to install any libraries in order to access them; simply use `process.env` as you would in Node.js. Use the command below to create an `.env` file:

`VARIABLE = "cheddar"`

Now, let’s update our `script.js` with the following code:

```javascript

Bun.serve({
    fetch(request){
        return new Response(process.env.VARIABLE)
    },
})
console.log("Listening on Port 3000")
```

Now, when we execute bun run `script.js` and go to [localhost:3000](http://localhost:3000), the data from our `.env` file ought to be returned.

## Conclusion

Bun has some great features that, in addition to being extremely quick, make many of the more tedious tasks—like writing files, managing basic databases, and using environmental variables—quite simple.