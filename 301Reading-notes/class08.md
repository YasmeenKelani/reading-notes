# Readings: APIs
 ## It stands for **Representational State Transfer**.

<img src="https://i.ytimg.com/vi/LooL6_chvN4/maxresdefault.jpg" alt="http" width="400"/>

+ ## REST APIs are designed around a **resource**.

> Resource identification refers to the unambiguous reporting of research resources such as genes, organisms, tools, and reagents (such as antibodies). These resources should be reported within publications with enough information that reviewers and subsequent researchers can identify the exact strain or reagent used. Preferably, authors should provide the full, descriptive name of the resource, its source and a unique identifier. Doing so allows for:

+ Better evaluation of the methods and interpretation of results
+ Reproducibility of the research
+ Machine readability and potential text mining applications

> Many reporting standards will include guidance on how to identify such resources. This page provides further information and sources for unambiguous identifiers.

for more information please visit: [bulding strategy and performance](https://saylordotorg.github.io/text_building-strategy-and-performance/s03-02-identifying-resources.html)

***
+ `GET`
+ `POST`
+ `PUT`
+ `PATCH`
+ `DELETE`

***
*What should the URIs be based on*?

**URIs** should be *based* on **nouns** and not **verbs**.

 *Give an example of a good URI*. [source](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

**ex**: *https://adventure-works.com/orders*

* What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

It means that there will be a **larg number of small resources for the API**, which will *result* in **load on the server**
Reason why chatty APIs are considered poor quality is because requiring multiple network calls will slow down an application. This is because each call contains data overhead (i.e. sender information, headers, authentication) which will slow down an application as well as network latency per each request.

* What status code does a successful `GET` request return?

It *returns* an **HTTP status code 200 (OK)**.

 * What status code does an unsuccessful `GET` request return?

It *returns* a **404 (Not Found)**.

* What status code does a successful `POST` request return?

It *returns* an **HTTP status code 201 (Created)**.

 * What status code does a successful `DELETE` request return?

It *returns* an **HTTP status code 204 (No Content)**.

<img src="https://miro.medium.com/proxy/1*EbBD6IXvf3o-YegUvRB_IA.jpeg" alt="http" width="400"/>