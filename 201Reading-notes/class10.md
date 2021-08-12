# Error Handling & Debugging

<img src="https://0701.static.prezi.com/preview/v2/h3j5rflrkheepc5js3m7tae7e76jc3sachvcdoaizecfr3dnitcq_3_0.png" alt="summary" width="700"/>

*  JavaScript can be hard to learn. Everyone makes mistakes when writing it. Error messages can help you understand what has gone wrong and how to fix it. You will learn about: The console and developer tools Common problems Handling errors. HOW JAVASCRIPT WORKS. To find the source of an error it helps to understand how scripts are processed. The order of execution is the order in which lines of code are executed or run.

* JS Debugger: Debugging is not easy. But fortunately, all modern browsers have a built-in JavaScript debugger. Built-in debuggers can be turned on and off, forcing errors to be reported to the user. With a debugger, you can also set breakpoints (places where code execution can be stopped), and examine variables while the code is executing. Normally, otherwise, follow the steps at the bottom of this page, you activate debugging in your browser with the F12 key, and select “Console” in the debugger menu.

<img src="https://www.oreilly.com/library/view/javascript-and-jquery/9781118531648/images/p452-001.jpg" alt="summary" width="700"/>

* The debugger Keyword: The debugger keyword stops the execution of JavaScript, and calls (if available) the debugging function. This has the same function as setting a breakpoint in the debugger. If no debugging is available, the debugger statement has no effect. With the debugger turned on, this code will stop executing before it executes the third line. ___

**Why is Debugging Important?**
* Debugging is done mostly to avoid the incorrect operation of an application by fishing out bugs and incorrect code. Let’s look at some of the importance of debugging and why developers should meticulously and efficiently debug their applications. Bugs can make your application crash. With proper debugging, you can spot bugs from your code and avert unexpected behavior.

* UNDERSTANDING SCOPE : In the interpreter, each execution context has its own va ri ables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent’s v a ri ables object. Functions in JavaScript are said to have lexical scope. They are linked to the object they were defined within. So, for each execution context, t he scope is the current execution context’s variables object, plus the variables object for each parent execution context.

* UNDERSTANDING ERRORS: If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handling code. If you are anticipating that something in your code may cause an error, you can use a set of statements to handle the error (you meet them on p480). This is important because if the error is not handled, the script will just stop processing and the user will not know why. So exception-handling code should inform users when there is a problem. please visit [Debugging](https://economictimes.indiatimes.com/definition/debugging) for more information.

* Here’s the debugging process:

1. Reproduce the problem.
2. Describe the bug. Try to get as much input from the user to get the exact reason.
3. Capture the program snapshot when the bug appears. Try to get all the variable values and states of the program at that time.
4. Analyse the snapshot based on the state and action. Based on that try to find the cause of the bug.
5. Fix the existing bug, but also check that any new bug does not occur.

<img src="https://www.edureka.co/blog/wp-content/uploads/2019/08/debuuging-steps-528x294.png" alt="summary" width="700"/>