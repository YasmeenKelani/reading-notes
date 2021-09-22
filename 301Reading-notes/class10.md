# In memory storage

## What is a ‘call’ ?

At the most basic level, a *`call`* stack is a data structure that uses the Last In, First Out (*`LIFO`*) principle to temporarily store and manage function invocation (*`call`*).

## How many ‘calls’ can happen at once ?

Only one call can be happen at time.

## What does LIFO mean ?

**`LIFO`** :
*  When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

## Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.

```
function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();
```

## What causes a Stack Overflow ?

A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.

## What is a ‘refrence error’ ?

**`Reference errors`** :
* This is as simple as when you try to use a variable that is not yet declared you get this type os errors.

## What is a ‘syntax error’ ?

**`Syntax errors`** :
* I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.
