# Search Engine Structure

This project concerns the implementation of a simple search engine.
The Applications is devided into two parts. Front-End and Back-End. Below you can see in more detail the structure of the software.

**FRONT END**

Fornt-end is actually a simple interface where the user can access the search engine.
```
  index.html
  script.js
  style.css
```


**BACK END**

All the work for crawling, indexing and pricessing queries is done here.

- application
  ```
  Application.java
  Response.java
  RouteController.java
  ```
- services
  - crawler
    ```
    CrawlTask.java
    Crawler.java
    ```
  - indexer
    ```
    Indexer.java
    IndexingTask.java
    ```
  - query_processor
    ```
    Query.java
    ```
- util
  ```
  ArrayIndexerComparator.java
  HtmlDocument.java
  StopWords.java
  Tupple.java
  ```
 
 ## How to run?
 
 ### Requirements
 
 * Chrome extension : [Allow CORS: Access-Control-Allow-Origin](https://chrome.google.com/webstore/detail/allow-cors-access-control/lhobafahddgcelffkeicbaginigeejlf?hl=en)
 * [Java 13.0.2](https://www.oracle.com/technetwork/java/javase/downloads/jdk13-downloads-5672538.html) or higher
 * [intellij idea](https://www.jetbrains.com/idea/) (if you choose the second option)
 * [maven](https://maven.apache.org/) (if you choose the second option)
 
 ### Options to run the project 
 
 * First Way : download the precompiled .jar file from the repository
    1. Download search-engine-1.0-SNAPSHOT.jar
    2. Open the command-line at the folder you have downloaded the .jar file
    3. Use the following command ```java -jar <website> <number of pages to crawl> <number of threads> <usel old data?(true/false)> <no crawling?(true/false)> ```
  
 * Second Way : download the whole project and using maven generate your own jar file
