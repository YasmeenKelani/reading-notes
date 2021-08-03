# Lists
![html lists](https://www.techfry.com/images/articles/html/html-lists.jpg)
* There are lots of occasions when we need to use lists. HTML provides us with three different types:
1. Ordered lists: are lists where each item in the list is numbered. For example, the list might be a set of steps for a recipe that must be performed in order, or a legal contract where each point needs to be identified by a section number.

![ordered list](https://i2.wp.com/blog.thejaytray.com/wp-content/uploads/2015/04/005-Music-HTML-List-Code-Ordered-List.png)

2. Unordered lists: are lists that begin with a bullet point (rather than characters that indicate order).

!(unordered list)(https://www.wikitechy.com/step-by-step-html-tutorials/img/html-images/code-explanation-unordered-tag-in-html.png)

3. Definition lists: are made up of a set of terms along with the definitions for each of those terms. plese visit this site [Definition ists](https://www.w3.org/MarkUp/html3/deflists.html).

## Boxes
* At the beginning of this section on CSS, you saw how CSS treats each HTML element as if it lives in its own box. You can set several properties that affect the appearance of these boxes. In this chapter you will see how to: 
1. Create borders around boxes.
2. Set margins and padding for boxes.
3. Control the dimensions of your boxes.
4. Show and hide boxes.

### Box Dimensions width, height:
* By default a box is sized just big enough to hold its contents. To set your own dimensions for a box you can use the height and width properties. The most popular ways to specify the size of a box are to use pixels, percentages, or ems. Traditionally, pixels have been the most popular method because they allow designers to accurately control their size.

### Limiting width min-width, max-width:
* Some page designs expand and shrink to fit the size of the user's screen. In such designs, the min-width property specifies the smallest size a box can be displayed at when the browser window is narrow, and the max-width property indicates the maximum width a box can stretch to when the browser window is wide.

### Limiting height min-height, max-height:
* In the same way that you might want to limit the width of a box on a page, you may also want to limit the height of it. This is achieved using the min-heightand max-height properties. The example on this page demonstrates these properties in action. It also shows you what happens when the content of the box takes up more space than the size specified for the box. 

### css3: Border images border-image

![css border-img](https://www.pvgr.eu/assets/img/articles/border-image-css-and-svg.png)

* The border-image property applies an image to the border of any box. It takes a background image and slices it into nine pieces. Here is the image. I have added marks where it is sliced in the example, taking 18 pixels from each corner to place an entire circle in each corner. The corner slices are always placed in the four corners of the box, but we have a choice whether the sides are stretched or repeated. 


### css3: elli  Ptic  Al s  hAP esborder-radius
* To create more complex shapes, you can specify different distances for the horizontal and the vertical parts of the rounded corners.For example, this will create a radius that is wider than it is tall: border-radius: 80px 50px; You can target just one corner using the individual properties for that corner: border-top-left-radius: 80px 50px; There is also a shorthand for targetting all four corners at once; first you specify the four horizontal values, then the four vertical values, as shown in the second shape on the left. You can even create a circle by taking a square box and making the border-radius the same height as the square, as shown in the third shape on the left.

```
p.one {  border-top-left-radius: 80px 50px; 
 -moz-border-radius-top-left: 80px 50px;
  -webkit-border-radius-top-left: 80px 50px;}p.two {  border-radius: 1em 4em 1em 4em / 2em 1em 2em 1em; 
   -moz-border-radius: 1em 4em 1em 4em      / 2em 1em 2em 1em;  -webkit-border-radius:  1em 4em 1em 4em  
       / 2em 1em 2em 1em;}p.three {  padding: 0px;  border-radius: 100px; 
        -moz-border-radius: 100px;  -webkit-border-radius: 100px;}
```
## Basic JavaScript Instructions

![JS](https://slideplayer.com/slide/16731500/97/images/2/CHAPTER+2+BASIC+JAVASCRIPT+INSTRUCTIONS.jpg)

* Using quotes inside a String: Sometimes you will want to use a double or single quote mark within a string. Because strings can live in single or double quotes, if you just want to use double quotes in the string, you could surround the entire string in single quotes. If you just want to use single quotes in the string, you could surround the string in double quotes (as shown in the third line of this code example).

* Using a Variable to store a Boolean: A Boolean variable can only have a value of true or fa 1 se, but this data type is very helpful. In the example on the right, the values true or fa 1 se are used in the cl ass attributes of HTML elements. These values trigger different CSS class rules: true shows a check, fa 1 se shows a cross. (You learn how the class attribute is set in Chapter 5.) It is rare that you would want to write the words true or false into the page for the user to read, but this data type does have two very popular uses: First, Booleans are used when the value can only be true/ fa 1 se. You could also think of these values as on/off or 0/1: true is equivalent to on or 1, fa 1 se is equivalent to off or 0 Second, Booleans are used when your code can take more than one path. Remember, different code may run in different circumstances (as shown in the flowcharts throughout the book).

```
JS
var i nStock; var shipping; inStock = true; 
shipping= fa l se; 
JAVASCRIPT var elStock = document.getElementByld('stock'); 
elStock.className =  inStock; var el Ship = document. getElementByid('shipping');
 elShip.className = shipping; 
```

```
HTML
<hl>Elderflower</hl>
 <div id="content"> <div class="message">Available: 
<span id="stock"></span></div> <div class="message">Shipping: 
<span id="shipping">~/span></div> </div> <script src="js/boolean-variable.js"></script> 
```
Visit this site [JavaScript Booleans](https://www.w3schools.com/js/js_booleans.asp)

* Changing the Value of a Variable: Once you have assigned a value to a variable, you can then change what is stored in the variable later in the same script. Once the variable has been created, you do not need to use the var keyword to assign it a new value. You just use the variable name, the equals sign (also known as t he assignment operator), and the new value for that attribute. 

### Decisions and Loops
* Comparing two Expressions: In this example, there are two rounds to the test and the code will check if the user has achieved a new high score, beating the previous record. The comparison operator checks if the user's total score is greater than the highest score for the test and stores the result in a variable called comparison. 

```
var scorel = 90; 
var score2 = 95;
 var highScorel 75; 
 var highScore2 = 95;
  II Round 1  score II Round 2  score II Round 1 high score II Round 2 high score II Check if scores are higher than current high scores var comparison= (score!+ score2) > (highScorel + highScore2); II Write the message into the page var el = document.getElementByid(' answer'); 
  el . textContent ='New high score:'+ comparison; 
  New high score: true 
```
* Using Logical AND: In this example, a math test hastworounds.Foreach round there are two variables: one holds the user's score for that round; the ot her holds the pass mark for t hat round. The logical AND is used to see if the user's score is greater than or equal to t he pass mark in both of the rounds of the test. The result is stored in a variable called passBoth. The example finishes off by letting the user know whether or not t hey have passed both rounds.

```
c04/js/ logical-and.js var scorel = 8;
 II Round 1 score var score2 = 8;
  II Round 2 score var passl 6; 
  II Round 1 pass mark var pass2 = 6; 
  II Round 2 pass mark II Check whether user passed both rounds,  store result in variable var passBoth = (scorel > = passl) && (score2 >= pass2);
   II Create message var msg = 'Both rounds passed: ' + passBoth; II Write the message  into the page var el = document.getElementBy!d(' answer'); el.textContent = msg; 
```
* Using IF statements: In th is example, the i f statement is checking if the value currently held in a variable called score is 50 or more. In this case, the statement evaluates to true (because the score is 75, which is greater than 50). Therefore, the contents of the statements within the subsequent code block are run, creating a message that congratulates the user and tells them to proceed. After the code block, the message is written to the page. If the value of the score variable had been less than 50, the statements in the code block would not have run, and the code would have continued on to the next line after the code block. On the left is an alternative version of the same example that demonstrates how lines of code do not always run in the order you expect them to. If the condition is met then: 1. The first statement in the code block calls the congratulate() fu nction. 2. The code within the congratulate() function runs. 3. The second line within the if statement's code block runs. 

```
 var score = 75; var msg = ' ' ; 
 II Score II Message dfunction congratulate() { L} msg += 'Congratulations! ' ;
  CD ® if (score>= 50) { II If score is 50 or more congratulate(); msg += 'Proceed to the next round . ' ;
   var el = document.getElementByld('answer') ; el . i nnerHTML = msg;

 ```
 * Using Switch statements: In this example, the purpose of the switch statement is to present the user with a different message depending on which level they are at. The message is stored in a variable called msg. The variable called l eve 1 contains a number indicating which level the user is on. This is then used as the switch value. (The switch value could also be an expression.) In the following code block (inside the curly braces), there are three options for what the value of the 1eve1 variable might be: t he numbers 1, 2, or 3. If the value of the 1eve1 variable is the number 1, the value of the msg variable is set to 'Good luck on the first test'. If the value is 2, it will read: 'Second of three -  keep going!· If the value is 3, the message w ill read: 'Final round, almost there!' If no match is found, t hen the value of the msg variable is set to 'Good l uck!' Each case ends wit h the break keyword which will tell the JavaScript interpreter to skip the rest of this code block and continue onto the next. 

 ```
 var msg; var level = 2; 
 II Message 11  / I Determine message based on level switch (level) { case 1: msg = 'Good luck on the first test' ;
  break; 
  case 2: msg = 'Second of three -keep going!';
   break;
    case 3: msg = ' Final round, almost there!'; 
    break;
     default: msg = 'Good luck!';
      break;
       var el = document.getEl ementByld('answer'); el . textContent = msg; 
``` 

* Using DO WHILE loops: The key difference between a whi 1 e loop and a do whi 1 e loop is that the statements in the code block come before the condition. This means that those statements are run once whether or not the condition is met. If you take a look at t he condition, it is checking that t  he value of the variable called i  i   s less than 1, but that vari able has already been set to a value of 1. Therefore, in this example the result is that the 5 times table is written out once, even though the counter is not less than 1. Some people like to write while on a separate line from the closing curly brace before it. 

![DoWhile](https://cdn.educba.com/academy/wp-content/uploads/2019/11/Do-While-Loop-in-JavaScript-main.png)

* Summarization :
1. Conditional statements allow your code to make decisions about what to do next. 
2. Comparison operators (===, ! ==,  ==, ! =, <, >, <=, =>) are used to compare two operands. Logical operators allow you to combine more than one set of comparison operators.
3. if ... else statements allow you to run one set of code if a condition is true, and another if it is false.
4.  switch statements allow you to compare a value against possible outcomes (and also provides a default option if none match). 
5. Data types can be coerced from one type to another.
6. All values evaluate to either truthy or falsy. 
7. There are three types of loop: for, while, and do ... while. Each repeats a set of statements. 






