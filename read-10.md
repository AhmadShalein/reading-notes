# Read 10: In memory storage:

## Understanding the JavaScript Call Stack:

**What is a ‘call’?**

- Call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).

**How many ‘calls’ can happen at once?**

- It is single-threaded. Meaning it can only do one thing at a time.

**What does LIFO mean?**

- Last In, First Out, which basically means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();

```

>> For this example, The target is to excute the thirdFunction(), but to get this secondFunction() need to be excuted first, but its block contains firstFunction() which is another function has to be excuted. So, at the ends you'll see that the last function which is firstFunction() has excuted first, and that's exactly the meaning of LFIO.

<cite>All the information for the call stack was taken from</cite> 
[Resource](https://www.freecodecamp.org/news/understanding-the-javascript-call-stack-861e41ae61d4/)

**What causes a Stack Overflow?**

```
function callMyself(){
  callMyself();
}

callMyself();
```

>> By looking at the previous example, we'll find out that we're calling the function inside its block.. that causes ``Stack Overflow``, There's no exit point and it will be calling itself until reaching maximum stack of the browser.

---------------------------------------------------------------------

## JavaScript error messages:

**What is a ‘refrence error’?**

- Using a variable has not declared.

**What is a ‘syntax error’?**

- Error occurs when you type the syntax incorrectly, for example missing a comma or curly brackets.

**What is a ‘range error’?**

- Manipulate the object/array with their lengths.

**What is a ‘type error’?**

- Occurs when a misspelling found.

**What is a breakpoint?**

- It's simply a point in your code, could be a console or condition..etc, to check a block of code (Debugging).

**What does the word ‘debugger’ do in your code?**

- A way of reaching the breakpoint, it shows you the history of the code block that set above it. givs you details of what this block of code contained.

---------------------------------------------------------------------

### Things I want to know more about:

- Call Stacks and how they work.
- How to read and handle errors properly.
