# REST

* In the simplest term, REST considered to be a set of principles that assign how HTTP and URLs Web standards are used. The main idea is that if you comply with REST principles while developing your application you will have a system that uses the Web’s architecture to your benefit.
In order to get computers connected together through a network and talking the same language, hundreds of methods have grown up during the years. Each method or protocol address computer communication in a specific way. For instance, you have probably heard about such technologies as SOAP, JMS or XML-RPC. SOAP requires a plenty amount of data and big computer capacity which is not suitable for the limited mobile apps’ resources. JMS is a kind of formal communication known as massaging between computers in a network which is mostly related to Java applications. XML-RPC also makes procedure calls over the Internet and has the same problems as SOAP. However, SOAP or XML-RPC can be easy if you have appropriate tools, they are a kind of an old school and are favored the approach of Java developers.

<img src="https://d3g4zhtkdvou35.cloudfront.net/wp-content/uploads/2014/09/what-is-rest.png" alt="rest" width="400"/>

## Who is **`Roy Fielding`** ?
*`Roy Fielding`* he is a computer scientist, one of the principal authors of the **`HTTP`** specification and the originator of the **`Representational State Transfer`** (*`REST`*) architectural style. 


He write the first web servers, that sent documents across the internet and then he did a ton of research explaining why the web works the way it does. His name is on the specification for the protocol that is used to get pages from servers to your browser.

## Why don’t the techniques that we use today work well when we need to be able to talk to all of the machines in the world ?

Because they weren't designed to be used like that. When Fielding and his colleagues started building the web, being able to talk to any machine anywhere in the world was a primary concern. But most of the techniques developers later used to get computers to talk to each other didn't have those requirements. You just needed to talk to a small group of machines.

## What is the **`HTTP protocol`** that Fielding and his friends created ?
*`HTTP protocol`* Fielding and his friends created is all about applying verbs to nouns. For instance, when you go to a web page, the browser does an *`HTTP GET`* on the *`URL`* you typed in and back comes a web page.

## What does a **`GET`** do ?
Web pages usually have images, right? Those are separate resources. The web page just specifies the *`URLs`* to the images and the browser goes and does more *`GETs`* using the HTTP protocol on them until all the resources are obtained and the web page is displayed. But the important thing here is that very different kinds of nouns can be treated the same. Whether the noun is an image, text, video, an mp3, a slideshow, whatever. I can *`GET`* all of those things the same way given a *`URL`*.

![GET](https://developer.mozilla.org/en-US/docs/Web/HTTP/Conditional_requests/httpresume4.png)

* What does a **`POST`** do ?
*`POST`* is an HTTP verb it used If one system needs to add something to another system.

* What does **`PUT`** do ?
*`PUT`* is an HTTP verb it used If a system wants to replace something in another system.

* What does **`PATCH`** do ?
*`PATCH`* is an HTTP verb it used to do a partial update.