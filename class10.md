# In memory storage

## Understanding the JavaScript Call Stack

1. What is a ‘call’?
**the call stack is single, function(s) execution, is done, one at a time, from top to bottom. It means the call stack is synchronous.**
2. How many ‘calls’ can happen at once?
**It is single-threaded. Meaning it can only do one thing at a time.**
3. What does LIFO mean?
**data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.**
4. Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.
`function sum (a, b) {`
   ` return a + b;`
`}`
`function avg(a, b) {`
    `return sum (a, b) / 2;`
`}
`let average = avg(10, 20);`

5. What causes a Stack Overflow?

**A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point.**

## JavaScript error messages

1. What is a ‘refrence error’?
**This is as simple as when you try to use a variable that is not yet declared you get this type os errors.**
`console.log(foo) // Uncaught ReferenceError: foo is not defined`

2. What is a ‘syntax error’?
**this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.**
3. What is a ‘range error’?
**When manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.**
4. What is a ‘tyep error’?
**this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable**
5. What is a breakpoint?
**The breakpoint can also be achieved by putting a debugger statement in your code in the line you want to break.**
6. What does the word ‘debugger’ do in your code?
**hen running the code above you can see the “history” before reaching that breakpoint.**

## Things I want to know more about

1. Hndling the different error types.

### Resources used in this reading

1. <https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/>
2. <https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c>
3. <https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors>