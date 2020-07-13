# Read 10 Notes

# CallStack
A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function

https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/

The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.

a call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

LIFO: When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

<img src="./images/reading10.png">

# stack overflow
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. 


## error messages
https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c


## Reference errors
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

## Syntax errors
I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.

## Range errors
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.

## Type errors
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible,

## Debugging
To debug your JS code, the easiest and maybe the most common way its to simply console.log() the variables you want to check or

## Call stack
The red part of our first example represents the call stack, which is the path that your program has taken to reach the point were you set a breaking point or were you have an error.

## Tools to avoid runtime errors
JS is not a compiled language like Java so your errors will happen at runtime, that means that you can only see whatever is wrong with your code after your run it.
Thankfully, to save us quite some time you can use tools like:
* quokka to evaluate your code as you type
* eslint to make sure your style guide is consistency and it will grab you an error or two along the way and
* For those of you looking to make JS a more strong typed experience you can check out stuff like TypeScript (like I said in a previous article, when learning I rather avoid libraries that abstract the core language so I wouldn’t recommend this last one when starting).

### [home](https://misalz.github.io/reading_notes2/)