# Document Object Model

The words “the DOM” are used all over developer documentation sites and tutorials on writing interactive JavaScript code

When you request a website, no matter what backend language is powering that website, it will respond with HTML. The browser receives a stream of HTML. The bytes are run through a complicated (but fully documented) parsing process that determines the different characters (e.g. the start tag character `<`, an attribute like `href`, a closing angle bracket like \`\`\`

```javascript

1. DOCTYPE
2. start-tag
3. end-tag
4. comment
5. character
6. end-of-file

Let’s take a break for a second. At this stage, the browser has received the bytes that’ve been sent by a server. The browser has converted the bytes to tags and has read through the tags to create a list of tokens.

This list of tokens then goes through the tree construction stage. The output of this stage is a tree-like structure — this is the DOM!

I want to point out two important quotes that Illya said in the video:
**a tree structure that captures the content and properties of the HTML and all the relationships between the nodes the DOM is the full, parsed representation of the HTML**

So the DOM is a model (representation) of the relationships and attributes of the HTML document that was received. Remember that DOM stands for “Document Object Model”. Something that I’ve found to be true as I’ve been learning is that to break something down, just read the thing backwards:

Document Object Model

…would become…

Object Model of the Document!

Remember that a JavaScript object is a tree-like structure that has properties and values. So the DOM can be accessed using a special object provided by the browser: ```
document
```

Try this:

1. open the console on this page
    
2. type out the word document
    
3. careful not to declare it const document
    
4. careful not to wrap it in quotes document
    

press enter

![Screenshot (313).png](https://cdn.hashnode.com/res/hashnode/image/upload/v1661237271584/wmX1SxUyu.png align="left")

Viewing the document object in the DevTools' Console pane.

The document the object is provided by the browser and is a representation of the HTML document. This object is not provided by the JavaScript language. ECMAScript is the language specification that JavaScript is based on, and it only references the document object model in one place, in its "Global Object" section:

In addition to the properties defined in this specification, the global object may have an additional host-defined property. This may include a property whose value is the global object itself; for example, in the HTML document object model, the window property of the global object is the global object itself. (source)

Basically, this says that the document object is not part of JavaScript, but is expected to already exist and be freely accessible to JavaScript code.

The DOM is standardized by the W3C. There are a number of specifications that make up the DOM, here are a few:

1. Core Specification
    
2. Events Specification
    
3. Style Specification
    
4. Validation Specification
    
5. Load and Save Specification