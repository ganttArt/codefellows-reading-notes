# Class 10

## Duckett JS Ch. 10, “Error Handling & Debugging”

- Builtin error objects in JS: Error, SyntaxError, ReferenceError, TypeError, RangeError, URIError, EvalError
- Use browser console to debug errors in console.
- Use console.log() to help with debugging in browser console
- Also available: console.info, console.warn, console.error
- console.group() and console.groupend() to group console logs in code
- console.table() to log objects in a tabular format
- console.assert() you can test if a condition is met.
- Add **breakpoints** in chrome using Sources option.
- Conditional breakpoints can be used
- Can use *debugger* keyword in javascript to automatically create a breakpoint.
- exception handling with: try, catch(exception), finally. This looks like  normal conditional formatting in JS but with different key words.
- `throw new Error('message');`
- NaN is not an error. To catch it you have to use a conditional if (!isNan()){}

## Git Notes from Lab10c

- echo '*.tmp' > .gitignore
- git diff
  - will show differences in working directory and last commit, does not include changes staged
- git show
  - will show changes staged for upcoming commit
- use ‘q’ to get out of git log
- git revert
  - to undo last commit
- git rebase
  - a potentially dangerous way to resolve merge conflicts

[<== Back](../README.md)
