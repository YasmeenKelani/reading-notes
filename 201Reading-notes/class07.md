# Domain Modeling 
* Domain modeling is the process of creating a conceptual model in code for a specific problem. A model describes the various entities, their attributes and behaviors, as well as the constraints that govern the problem domain. An entity that stores data in properties and encapsulates behaviors in methods is commonly referred to as an object-oriented model. Visit [Domain Modeling](https://olegchursin.medium.com/a-brief-introduction-to-domain-modeling-862a30b38353)

<img src="https://miro.medium.com/max/1400/1*UuZRQ57iPmEKsY5wsgGBLA.jpeg" alt="domain" width="700"/>

**Model epic fails videos**
* Imagine you've been tasked to build a program that models the popularity of epic fail videos. After months of painstaking research, you've determined that the two essential metrics for gauging popularity are an epic rating and whether or not the video has animals. Since you'll be modeling the popularity of many types of videos—parkour epic fails, corgi epic fails, etc.—you'll want to build self-contained objects with the same attributes and behaviors. That way, when you need to change the algorithm for determining popularity, the changes will be small and targeted. As you read this article, type out and run all code samples you come across. Do not copy and paste. Writing out and testing your code will help you remember how to implement domain models in JavaScript later.
**Summary**
* Domain modeling is the process of creating a conceptual model for a specific problem. And a domain model that's articulated well can verify and validate your understanding of that problem.
* Here's some tips to follow when building your own domain models: 
1. When modeling a single entity that'll have many instances, build self-contained objects with the same attributes and behaviors.
2. Model its attributes with a constructor function that defines and initializes properties.
3. Model its behaviors with small methods that focus on doing one job well.
4. Create instances using the new keyword followed by a call to a constructor function.
5. Store the newly created object in a variable so you can access its properties and methods from outside.
6. Use the this variable within methods so you can access the object's properties and methods from inside

## Tables
* WhaT's a Table? 
* A table represents information in a grid format. Examples of tables include financial reports, TV schedules, and sports results.

<img src="https://cf2.ppt-online.org/files2/slide/x/x03e9GTk5pRrMdEywnDSZbjBHJ2zoYaFmfuKsh/slide-5.jpg" alt="table" width="700"/>

* basic Table Structure

```
<table>  <tr>    <td>15</td>    <td>15</td>    <td>30</td>  </tr>  <tr>    <td>45</td>    <td>60</td>    <td>45</td>  </tr>  <tr>    <td>60</td>    <td>90</td>    <td>90</td>  </tr></table>
```

* HtMl Table headings

```
<table>  <tr>    <th></th>    <th scope="col">Saturday</th>    <th scope="col">Sunday</th>  </tr>  <tr>    <th scope="row">Tickets sold:</th>    <td>120</td>    <td>135</td>  </tr>  <tr>    <th scope="row">Total sales:</th>    <td>$600</td>    <td>$675</td>  </tr></table>
``` 

* spanning columns:
Sometimes you may need the entries in a table to stretch across more than one column.The colspan attribute can be used on a < th> or < td> element and indicates how many columns that cell should run across.In the example on the right you can see a timetable with five columns; the first column contains the heading for that row (the day), the remaining four represent one hour time slots.

* long Tables

```
<table>  <thead>    <tr>      <th>Date</th>      <th>Income</th>      <th>Expenditure</th>    </tr>  </thead>  <tbody>    <tr>      <th>1st January</th>      <td>250</td>      <td>36</td>    </tr>    <tr>      <th>2nd January</th>      <td>285</td>      <td>48</td>    </tr>    <!-- additional rows as above -->    <tr>      <th>31st January</th>      <td>129</td>      <td>64</td>     </tr>  </tbody>  <tfoot>    <tr>      <td></td>      <td>7824</td>      <td>1241</td>    </tr>  </tfoot></table>
```

* summary:
1. The < table> element is used to add tables to a web page.
2. A table is drawn out row by row. Each row is created Xwith the < tr> element.
3. Inside each row there are a number of cells Xrepresented by the < td> element (or < th> if it is a header).
3. You can make cells of a table span more than one row Xor column using the rowspan and colspan attributes.
4. For long tables you can split the table into a X< thead>, < tbody>, and < tfoot>.

## Functions, Methods, and Objects
 
* This example is split into two parts. The first shows you the details about the hotel, room rate, and offer rate. The second part indicates when the offer expires. 

* EXAMPLE 

```
c03/js/example.js JAVASCRIPT I* The  sc r i pt is placed  inside an  immediately invoked function expression which helps protect  the scope of variabl es *I -(function() { II PART ONE:  CREATE HOTEL OBJECT AND WRITE OUT THE OFFER DETAILS II Create a  hotel obj ect usin g  object l i t eral syntax var hotel =  { name: 'Park', roomRate: 240, II Amount in dollars discount: 15, II Percentage discount offerPrice: function() { var offerRate = this.roomRate * ((100 -this. discount) I 100); return offerRate; II Wr ite out the hotel name, standard rate, and the special ra t e var hotelName, roomRate, specialRate; I I Declare variables hotelName = document.getElementByid('hotelName'); roomRate = document.getElementByid('roomRate'); specialRate = document. getElementByld('specialRate'); II Get element s hotelName.textContent = hotel .name; I I Write hotel  name roomRate.textContent = '$' + hotel.roomRate. toFixed(2); II Write room rate specialRate. textContent = '$' +hotel .offerPrice(); II Write offer price
```

* EXAMPLE: 

```
II PART TWO: CALCULATE ANO WRITE OUT THE EXPIRY DETAILS FOR THE OFFER var expiryMsg; II Message displayed t o  user s var  today; II Today's dat e var el Ends; II The element that s hows the message about  the offer ending f unction offerExpires (today) { II Decl are variables within the function  for l ocal  scope var weekFromToday, day, date, month, year, dayNames , monthNames; II Add 7 days time (added i n mi lliseconds) weekFromToday =new Date(today. getTime()  +  7 * 24 * 60 * 60 * 1000); I I Create arrays to hol d  t he names of days I months dayNames =  [ 'Sunday',   'Monday', 'Tuesday' , 'Wednesday', 'Thursday', 0 ' Friday', 'Saturday' ] ; monthNames =['January', ' February', 'March', 'April', 'May' ,   'June' , 0 ' July' , 'August ' ,   'September' , 'October' ,   'November' , 'December' ] ; II Collect the parts of the dat e  t o  show on t he page day = dayNames [weekFromToday. getOay ()]; date= weekFromToday. getOate(); month= mont hNames[weekFromToday .getMonth()]; year= weekFromToday. getFullYear(); I I Create the message expiryMsg = 'Offer expires  next ' ; expiryMsg +=day  +  ' <br I>(' +date+ '   ' +month+ '   ' +year+ ')'; retur n expiryMsg; today= new Date () ; elEnds = document.getEl ementByid(' of ferEnds'); elEnds.innerHTML = of fe rExpires(today); II Put t oday's date in variable II Get  t he  offerEnds element II Add the expi ry  message II Finish the immediatel y  invoked function  expression } ()) ; 
```
* Summary:
1. Functions allow you to group a set of related statements together that represent a single task.
2. Functions can take parameters (informatiorJ required to do their job) and may return a value.
3. An object is a series of variables and functions that represent something from the world around you. 
4. In an object, variables are known as properties of the object; functions are known as methods of the object.
5. Web browsers implement objects that represent both the browser window and the document loaded into the browser window. 
6. JavaScript also has several built-in objects such as String, Number, Math, and Date. Their properties and methods offer functionality that help you write scripts.
7. Arrays and objects can be used to create complex data sets (and both can contain the other).
