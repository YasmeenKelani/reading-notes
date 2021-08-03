# links

* Links are the defining feature of the web because they allow you to move from one web page to another — enabling the very idea of browsing or surfing.

* Writing links: 
1. Links are created using the < a> element. Users can click on anything between the opening < a> tag and the closing < /a> tag. You specify which page you want to link to using the href attribute.
2. The text between the opening < a> tag and closing < /a> tag is known as link text. Where possible, your link text should explain where visitors will be taken if they click on it (rather than just saying "click here"). Below you can see the link to IMDB that was created on the previous page.  
3. To write good link text, you can think of words people might use when searching for the page that you are linking to. (For example, rather than write "places to stay" you could use something more specific such as "hotels in New York.")

**Linking to other pages on the same site:**

```
<p>  <ul>    
  <li><a href="index.html">Home</a></li> 
       <li><a href="about-us.html">About</a></li> 
            <li><a href="movies.html">Movies</a></li> 
                 <li><a href="contact.html">Contact</a></li>
                   </ul></p>
```

**Directory structure:**

![directory](https://openlab.bmcc.cuny.edu/mmp-240-fall-19-stein/wp-content/uploads/sites/100/2019/09/WebsiteFolderStructure-1024x768.png)

* On larger websites it's a good idea to organize your code by placing the pages for each different section of the site into a new folder. Folders on a website are sometimes referred to as directories.
* structure: The diagram on the right shows the directory structure for a fictional entertainment listings website called ExampleArts. 

* Relative URL: 
Relative URLs can be used when linking to pages within your own website. They provide a shorthand way of telling the browser where to find your files. for more information please visit [More about Relative URL](https://www.seoclarity.net/resources/knowledgebase/difference-relative-absolute-url-1532)

### Layout 

* The simplest and most popular way of creating layouts is using HTML <table> tag. These tables are arranged in columns and rows, so you can utilize these rows and columns in whatever way you like.

**Key ConCepts in positioning eLements:**
1. Bulding block: CSS treats each HTML element as if it is in its own box. This box will either be a block-levelbox or an inline box.
2. containing element: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. 

**Controlling the Positin of Elemet**
CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the positionproperty in CSS. You can also float elements using the float property.

### JavaScript

**Functions, Methods, and Objects**

* Browsers require very detailed instructions about what we want them t o do. Therefore, complex scripts can run to hundreds (even thousands) of lines. Programmers use functions, methods, and objects to organize their code. 

* what is Function? Functions let you group a series of statements together to perform a specific task. If different parts of a script repeat the same task, you can reuse the function (rather than repeating the same set of st atements). 

* A basic function in HTML & JAVASCRIPT:

```
<!DOCTYPE html> <html> <head> Before the closing </body> tag, you can see the link to the JavaScript file. The JavaScript fi le starts with a variable used to hold a new message, and is followed by a function called updateMessage(). <tit le>Basic Function</title> <l ink rel ="stylesheet"  href="cs s/ c03. css"  / > </head> <body> <hl>TravelWorthy</ hl> <div id="message">Welcome to our site!</ div> <script src="js/ basic-function. js"></ script> </body> </html> 
```
```
var msg =  'Sign up to receive our newsletter for 10% off!'; function updateMessage() { var el = document.getElementByld('message'}; el .textContent = msg; } updateMessage(}; 
```
**Article** 
* 6 Reasons for Pair programming:
1. Greater efficiency: It is a common misconception that pair programming takes a lot longer and is less efficient. In reality, when two people focus on the same code base, it is easier to catch mistakes in the making. Research indicates that pair programing takes slightly longer, but produces higher-quality code that doesn’t require later effort in troubleshooting and debugging (let alone exposing users to a broken product). So, in the long-run, it’s often actually more efficient than two people working on separate features. When coming up with ideas and discussing solutions out loud, two programmers may come to a solution faster than one programmer on their own.
2. Engaged collaboration: When two programmers focus on the same code, the experience is more engaging and both programmers are more focused than if they were working alone. It is harder to procrastinate or get off track when someone else is relying on you to complete the work. Popping open your Facebook timeline is just that less enticing when someone else is looking at your screen.
3. Learning from fellow students:
Everyone has a different approach to problem solving; working with a teammate can expose developers to techniques they otherwise would not have thought of. If one developer has a unique approach to a specific problem, pair programming exposes the other developer to a new solution.
4.  Social skills: This has long-term career impacts. As much as employers want strong programmers, they know it’s essential to hire people who can work well with others.
5.  Job interview readiness: For most roles, the ability to work with and learn from others and stellar communication skills are as (or more!) important to a company than specific technical skills. Pair programming strengthens all of those skills.
6. Work environment readiness: Many companies that utilize pair programing expect to train fresh hires from CS-degree programs on how they operate to actually deliver a product. Code Fellows graduates who are already familiar with how pairing works can hit the ground running at a new job, with one less hurdle to overcome.

