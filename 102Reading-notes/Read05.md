# JvaScript
## Expressions and operators 
* Operators: JavaScript has the following types of operators. This section describes the operators and contains information about operator precedence.Assignment operators, Comparison operators, Arithmetic operators, Bitwise operators, Logical operators, String operators, Conditional (ternary) operator, Comma operator, Unary operators and Relational operators.
![assignment operator](https://slidetodoc.com/presentation_image_h/b10c92ba5ddd372dedea57349c7e2fe0/image-12.jpg)
* Expressions: An expression is any valid unit of code that resolves to a value.
Every syntactically valid expression resolves to some value but conceptually, there are two types of expressions: with side effects (for example: those that assign value to a variable) and those that in some sense evaluate and therefore resolve to a value.
 The expression x = 7 is an example of the first type. This expression uses the = operator to assign the value seven to the variable x. The expression itself evaluates to seven.
 The code 3 + 4 is an example of the second expression type. This expression uses the + operator to add three and four together without assigning the result, seven, to a variable.
* JavaScript has the following expression categories:
1. Arithmetic: evaluates to a number, for example 3.14159. (Generally uses arithmetic operators.)
2. String: evaluates to a character string, for example, "Fred" or "234". (Generally uses string operators.)
3. Logical: evaluates to true or false. (Often involves logical operators.)
4. Primary expressions: Basic keywords and general expressions in JavaScript.
5. Left-hand-side expressions: Left values are the destination of an assignment.
![expression](https://images.slideplayer.com/16/5210712/slides/slide_2.jpg)

# Loops and iteration
* Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript. There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. (Note that it's possible that number could be zero!).
* The statements for loops provided in JavaScript are:
1. for statement.
2. while statement.
3. labeled statement.
4. do...while statement.
5. break statement.
6. continue statement.
## For Statement:
* A for loop repeats until a specified condition evaluates to false. The JavaScript for loop is similar to the Java and C for loop. When a for loop executes, the following occurs:
1. The initializing expression initialExpression, if any, is executed. This expression usually initializes one or more loop counters, but the syntax allows an expression of any degree of complexity. This expression can also declare variables.
2. The conditionExpression expression is evaluated. If the value of conditionExpression is true, the loop statements execute. If the value of condition is false, the for loop terminates. (If the condition expression is omitted entirely, the condition is assumed to be true.)
3. The statement executes. To execute multiple statements, use a block statement ({ ... }) to group those statements.
4. If present, the update expression incrementExpression is executed.
5. Control returns to Step 2.
![For statement](https://cdn.educba.com/academy/wp-content/uploads/2019/10/For-Loop-in-JavaScript.png)
## While statement:
* A while statement executes its statements as long as a specified condition evaluates to true, If the *condition *becomes false, statement within the loop stops executing and control passes to the statement following the loop. The condition test occurs before statement in the loop is executed. If the condition returns true, statement is executed and the condition is tested again. If the condition returns false, execution stops, and control is passed to the statement following while.To execute multiple statements, use a block statement ({ ... }) to group those statements.
![While statement](https://i.ytimg.com/vi/kUkqapBCsdE/hqdefault.jpg)
* For more information please visit this site [Loops and Iteration](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Loops_and_iteration)