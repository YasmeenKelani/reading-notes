![debugging](https://images.slideplayer.com/31/9700382/slides/slide_2.jpg)

*  JavaScript can be hard to learn. Everyone makes mistakes when writing it. Error messages can help you understand what has gone wrong and how to fix it. You will learn about: The console and developer tools Common problems Handling errors. HOW JAVASCRIPT WORKS. To find the source of an error it helps to understand how scripts are processed. The order of execution is the order in which lines of code are executed or run.

* function greetUser() { return ‘Hello ’ + getName(); } function getName() { var name = ‘Molly’; return name; } var greeting = greetUser(); alert(greeting); LOOK AT THIS SCRIPT:
* function greetUser() { return ‘Hello ’ + getName(); } function getName() { var name = ‘Molly’; return name; } var greeting = greetUser(); alert(greeting); 
* There are execution contexts: One global context And a new execution context for each new function
* function greetUser() { return ‘Hello ’ + getName(); } function getName() { var name = ‘Molly’; return name; } var greeting = greetUser(); alert(greeting); GLOBAL CONTEXT (global scope) FUNCTION CONTEXT (function-level scope)