# Code in a Content Management System
* If you are working with a content
management system, blogging
platform, or e-commerce
application, you will probably
log into a special administration
section of the website to control
it. The tools provided in the
administration sections of these
sites usually allow you to edit
parts of the page rather than
the entire page, which means
you will rarely see the < html>,
< head>, or < body> elements.
 ## Looking at How Other sites are Built:
 * When the web was first taking
off, one of the most common
ways to learn about HTML and
discover new tips and techniques
was to look at the source code
that made up web pages.
![sites build](https://rawinfopages.co.uk/wp-content/uploads/2018/06/how-sites-built.jpg)

* Summary Structure:
1. HTML pages are text documents.
2. HTML uses tags (characters that sit inside angledbrackets) to give the information they surround special meaning.
3. Tags are often referred to as elements.
4. Tags usually come in pairs. The opening tag denotes the start of a piece of content; the closing tag denotes the end.
5. Opening tags can carry attributes, which tell us more about the content of that element.
6. Attributes require a name and a value.
7. To learn HTML you need to know what tags are available for you to use, what they do, and where they can go.

### Semantics in HTML:
* In programming, Semantics refers to the meaning of a piece of code — for example "what effect does running that line of JavaScript have?", or "what purpose or role does that HTML element have" (rather than "what does it look like?".
* In HTML, for example, the < h1> element is a semantic element, which gives the text it wraps around the role (or meaning) of "a top level heading on your page." For more information please visit [Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics).

![Semantics](https://www.w3schools.com/html/img_sem_elements.gif)

### Headings:
* Browsers display the contents of headings at different sizes. The contents of an < h1> element is the largest, and the contents of
an < h6> element is the smallest. The exact size at which each
browser shows the headings can vary slightly. Users can also adjust the size of text in their browser. You will see how to
control the size of text, its color, and the fonts used when we
come to look at CSS.
### Paragraphs:
* To create a paragraph, surround the words that make up the paragraph with an opening < p> tag and closing < /p> tag. By default, a browser will show each paragraph on a new line with some space between it and any subsequent paragraphs.

### Bold & Italic:
* By enclosing words in the tags < b> and < /b> we can make
characters appear bold. The < b> element also represents a section of text that would be presented in a visually different way (for example key words in a paragraph) although the use of the < b> element does not imply any additional meaning.

* By enclosing words in the tags < i> and < /i> we can make
characters appear italic. The < i> element also represents
a section of text that would be said in a different way from
surrounding content — such as technical terms, names of ships,
foreign words, thoughts, or other terms that would usually be italicized.

### Summary: 
* HTML elements are used to describe the structure of the page (e.g. headings, subheadings, paragraphs).
* They also provide semantic information (e.g. where emphasis should be placed, the definition of any acronyms used, when given text is a quotation).

## CSS
* CSS allows you to create rules that specify how the content of an element should appear. For example, you can specify that the background of the page is cream, all paragraphs should appear in gray using the Arial typeface, or that all level one headings should be in a blue, italic, Times typeface.
![Css](https://www.oxfordwebstudio.com/user/pages/06.da-li-znate/sta-je-css/sta-je-css.png)

### Using External CSS:
* < link> chapter-10/using-external-css.html HTML The < link> element can be used
in an HTML document to tell the browser where to find the CSS file used to style the page. It is an empty element (meaning it does not need a closing tag), and it lives inside the < head> element. It should use three attributes:
1. href: This specifies the path to the CSS file (which is often placed in a folder called css or styles).
2. type: This attribute specifies the type of document being linked to. The value should be text/css.
3. rel: This specifies the relationship
between the HTML page and the file it is linked to. The value should be stylesheet when linking to a CSS file.

### Using Internal CSS: 
* You can also include CSS rules within an HTML page by placing them inside a < style> element, which usually sits inside the < head> element of the page.
The < style> element should use
the type attribute to indicate
that the styles are specified in
CSS. The value should be text/
css. When building a site with more
than one page, you should use
an external CSS style sheet. This:
1. Allows all pages to use the
same style rules (rather than
repeating them in each page).
2. Keeps the content separate
from how the page looks.
3. Means you can change the
styles used across all pages
by altering just one file
(rather than each individual
page).
* please visit this site [how to add CSS](https://www.w3schools.com/css/css_howto.asp)

## Basic JavaScript Instructions
 ### Linking to JavaScript file from an HTML pages:
 When you want to use JavaScript with a web page, you use the HTML < script> element to tell the browser it is coming across a script.Its s re attribute tells people where the JavaScript file is stored. 

```
<!DOCTYPE html> 
<html> 
<head> 
<title>Constructive &amp; Co.</ title> 
<link rel ="stylesheet" href="css/ cOl.css" /> 
</ head> 
<body> 
<hl>Constructive &amp ; Co. </ hl> 
<script src="js/ add-content.js"></ script> 
<p>For all orders and i nquiries please cal l 
<em>SSS-3344</ em></ p> 
</ body> 
</html>
```
* C: How do I wirte a script for a web page? 
1. It is best to keep JavaScript code in its own JavaScript  file. JavaScript files are text files (like HTML pages and 
CSS style sheets), but they have the . js extension. 
2. The HTML < script> element is used in HTML pages to tell the browser to load the JavaScript file (rather like 
the < link> element can be used to load a CSS file). 
3. If you view the source code of the page in the browser, the JavaScript will not have changed the HTML, because the script works with the model of the web  page that the browser has created. 

## Statments:
* A script is a series of instructions that a computer can follow one-by-one. Each individual instruction or step is known as a statement.Statements should end with a semicolon. 

```
var today= new Date{); 
var hourNow = today.getHours{) ; 
var greeting; 
if (hourNow > 18) { 
greeting= 'Good evening';} 
else if (hourNow > 12) { 
greeting= 'Good afternoon';} 
else if (hourNow > O) { 
greeting 'Good morning';} 
else { 
greeting 'Welcome'; }
document.write(greeting) ; 
```
## Comments:
* You should write comments to explain what your code does. They help make your code easier to read and understand.This can help you and others who read your code. 

```
/* Th i s script displays a greeting to the user based upon the current time. 
It is an example from JavaScript & jQuer y book */ ;

```
## What is a Variable?
* A script will have to temporarily store the bits of information it needs to do its job. It can store this data in variables. When you write JavaScript, you have to tell the interpreter every individual step that you want it to perform. This sometimes involves more detail than you might expect. 

## Decisions & Loops
* please visit [Decisiona and loops](https://www.tutorialcup.com/cprogramming/decision-making-and-loops.htm#:~:text=If%20the%20condition%20in%20decision,set%20of%20instructions%20are%20executed.&text=When%20we%20have%20to%20execute,loops%20or%20DO%2FWHILE%20loops.).

![loops](https://www.tutorialcup.com/wp-content/uploads/2019/09/Decision-Making-and-Loops-in-C-Programming.jpg)

* EVALUATIONS :You can analyze values in your scripts to determine whether or note they match expected results.
* DECISIONS: Using the results of evaluations, you can decide which path your script should go down.
* lOOPS: There are also many occasions where you will want to perform the same set of steps repeatedly.
* Loops offer a quick and easy way to do something repeatedly. This chapter of the JavaScript Guide introduces the different iteration statements available to JavaScript. There are many different kinds of loops, but they all essentially do the same thing: they repeat an action some number of times. (Note that it's possible that number could be zero!).

![decision](https://siwdt.files.wordpress.com/2014/11/70-e1415207217526.jpg)

### evaluating conditions and conditional statements: 
`if(score > 50)`

### comparasion operators: evaluating conditions 
+ is equal to: `==`
+ is not equal to: `!=` 
+ strict equal to: `===`
+ greater than: `>`

## COMPARING TWO EXPRESSIONS:
``` 
var  scorel  = 90; var  score2  = 95; 
var  highScorel 75; 
var  highScore2 = 95; 

var  comparison= (score!+  score2) > (highScorel  + highScore2); 
var  el = document.getElementByid( ' answer'); el . textContent  =' New high  score:'+ comparison; 
```
![loops git](https://chris.beams.io/content/images/size/w2000/2021/01/git_commit_2x.png)