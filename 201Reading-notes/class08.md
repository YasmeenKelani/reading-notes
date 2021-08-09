# Layout 

* The simplest and most popular way of creating layouts is using HTML < table> tag. These tables are arranged in columns and rows, so you can utilize these rows and columns in whatever way you like.
* for more information visit [html-Layout](https://www.geeksforgeeks.org/html-layout/).

**Key ConCepts in positioning eLements:**
1. Bulding block: CSS treats each HTML element as if it is in its own box. This box will either be a block-levelbox or an inline box.
2. containing element: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element. 
* containing ElEmEnts: If one block-level element sits inside another block-level element then the outer box is known as the containing or parent element.It is common to group a number of elements together inside a < div>(or other block-level) element. For example, you might group together all of the elements that form the header of a site (such as the logo and the main navigation). The < div> element that contains this group of elements is then referred to as the containing element.

<img src="https://slideplayer.com/slide/14545330/90/images/3/KEY+CONCEPTS+IN+POSITIONING+ELEMENTS+Lorem+Ipsum+BUILDING+BLOCKS.jpg" alt="domain" width="600"/>

**Controlling the Positin of Elemet**
CSS has the following positioning schemes that allow you to control the layout of a page: normal flow, relative positioning, and absolute positioning. You specify the positioning scheme using the positionproperty in CSS. You can also float elements using the float property.

1. normaL fLow: In normal flow, each block-level element sits on top of the next one. Since this is the default way in which browsers treat HTML elements, you do not need a CSS property to indicate that elements should appear in normal flow, but the syntax would be:position: static;
 <img src="https://slideplayer.com/slide/14545330/90/images/13/NORMAL+FLOW+position%3A+static.jpg" alt="domain" width="600"/>

 2. Relative Position: Relative positioning moves an element in relation to where it would have been in normal flow.For example, you can move it 10 pixels lower than it would have been in normal flow or 20% to the right
 
 ```
 p.example {  position: relative;  top: 10px;  left: 100px;}
 ```

 3. absoLute positioning: 
 ```
 h1 {  position: absolute;  top: 0px;  left: 500px;  width: 250px;}p {  width: 450px;}
 ```

 4. fixed positioning: 
 ```
 h1 {  position: fixed;  top: 0px;  left: 50px;  padding: 10px;  margin: 0px;  width: 100%;  background-color: #efefef;}p.example {  margin-top: 100px;}
 ```
 ### floating eLements:
 The float property allows you to take an element in normal flow and place it as far to the left or right of the containing element as possible. When you use the floatproperty, you should also use the width property to indicate how wide the floated element should be. If you do not, results can be inconsistent but the box is likely to take up the full width of the containing element (just like it would in normal flow).

<img src=" https://stuyhsdesign.files.wordpress.com/2015/10/float-rt-lt.png" alt="domain" width="600"/>
 
* Clearing Floats:
```
body {  width: 750px;  font-family: Arial, Verdana, sans-serif;  color: #665544;}p {  width: 230px;  float: left;  margin: 5px;  padding: 5px;  background-color: #efefef;}.clear {  clear: left;}
```
* Summary layout:
1. < div>X elements are often used as containing elements to group together sections of a page.
2. Browsers display pages in normal flow unless you Xspecify relative, absolute, or fixed positioning.
3. The Xfloat property moves content to the left or right of the page and can be used to create multi-column layouts. (Floated items require a defined width.)
4. Pages can be fixed width or liquid (stretchy) layouts.XDesigners keep pages within 960-1000 pixels wide, Xand indicate what the site is about within the top 600 pixels (to demonstrate its relevance without scrolling).
5. Grids help create professional and flexible designs.
6. CSS Frameworks provide rules for common tasks.
7. You can include multiple CSS files in one page.
