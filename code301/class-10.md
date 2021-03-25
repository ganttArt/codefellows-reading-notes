# Class 10 - The call stack, errors and debugging

## [The JavaScript Call Stack - What It Is and Why It's Necessary](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

- The call stack is primarily used for function invocation (call). Since the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.
- a call stack is a data structure that uses the Last In, First Out (LIFO)
- The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.
- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.
- A function invocation creates a stack frame that occupies a temporary memory.

## [JavaScript error messages && debugging](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)

- Types of Errors:
  - Reference error: you referred to something that doesn't currently exist
  - Syntax error: you typed something wrong
  - Range error: invalid range/array length
  - Type error: the thing that you're trying to use is the wrong type than what is trying to be used here.
- Debugging:
  - Set **Breakpoints** in the console or on vscode to help look individually at sections of code
- Use `try` and `catch` to gracefully handle errors
- JS is not a compiled language like Java so your errors will happen at runtime, that means that you can only see whatever is wrong with your code after your run it.
  - Tools to elieviate this reality:
    - quokka: to evaluate your code as you type
    - eslint: style/error checking
    - try TypeScript for a more strongly typed approach.

### For reference: [MDN JS Error docs](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)
