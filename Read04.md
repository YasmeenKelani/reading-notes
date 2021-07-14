# JavaScript 
## What is JavaScript? 
*  JavaScript (often shortened to JS) is a lightweight, interpreted, object-oriented language with first-class functions, and is best known as the scripting language for Web pages, but it's used in many non-browser environments as well. It is a prototype-based, multi-paradigm scripting language that is dynamic, and supports object-oriented, imperative, and functional programming styles.

* JavaScript runs on the client side of the web, which can be used to design / program how the web pages behave on the occurrence of an event. JavaScript is an easy to learn and also powerful scripting language, widely used for controlling web page behavior.
## Semantics in JavaScript:
![JS Semantic and Synatx](https://image1.slideserve.com/3265474/syntax-and-semantics-n.jpg)
* In JavaScript, consider a function that takes a string parameter, and returns an < li> element with that string as its textContent. Would you need to look at the code to understand what the function did if it was called build('Peach'), or createLiWithContent('Peach')?
* We can distinguish 3 major parts of what we usually refer to as "JavaScript":
1. The language itself. This is fairly standard among the various environments, both in the various browsers and in the various server-side environments.
2. The DOM API - how the language can interact with the various parts of a web page while in the browser. While in this respect the various browsers are getting closer to each other they still differ. Several libraries, most prominently JQuery, is trying to provide a unified API.
3. The server API (or just API) provided by Node.js or one of the other server-side systems.
* ** JavaScript input with prompt and confirm: ** Visit [JS prompt and confirm](https://code-maven.com/javascript-input-with-prompt-and-confirm)
1. The fist one is called prompt: It will show a pop-up window with the text provided as the first parameter and with a textbox the user can fill in. When the user presses OK, the value in the text box will be returned by the prompt() function. Then, in this example we use the document.write method to update the html with the text.
#### examples/js/prompt.html
![prompt](https://csharpcorner-mindcrackerinc.netdna-ssl.com/UploadFile/26b237/dialog-box-in-javascript/Images/prompt%20dialog%20box.jpg)

2. confirm: The other pop-up is not really an input method. It allows the developer to ask a Yes/No question. Calling the confirm() function will show a pop-up window with the provided texts and with two buttons. If the user presses OK the confirm() function will return true, if the user presses cancel or hits the ESC key, the function will return false. 
#### examples/js/confirm.html
![confirm](https://csharpcorner-mindcrackerinc.netdna-ssl.com/UploadFile/26b237/dialog-box-in-javascript/Images/confirm%20dialog%20box.jpg)