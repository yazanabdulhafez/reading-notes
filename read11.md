# Spring

## Serving Web Content with Spring MVC

![components of mvc](https://www.tutorialandexample.com/wp-content/uploads/2020/02/Components-of-Spring-Boot.png)

To build an application with spring mvc from scratch you need to do the following steps:

### 1.Starting with Spring Initializr

You can either choose a pre initialized project and download the zip file or you can
manually initialize the project as the following steps:

1. go to <https://start.spring.io>. This service pulls in all the dependencies you need.
2. Choose  Gradle.
3. Click Dependencies and select Spring Web, Thymeleaf, and Spring Boot DevTools.
4. Click Generate.
5. Download the resulting ZIP file.

### 2.Create a Web Controller

The HTTP requests are handled by using a controller. in spring we create controller by
the `@Controller` annotation.

### 3.Spring Boot Devtools

In all web application when we made a change in code we restart the app then refresh the browser to see the results,in spring Boot this can done fast using module known as spring-boot-devtools.

The benefits of this module:

1. Enables hot swapping.

2. Switches template engines to disable caching.

3. Enables LiveReload to automatically refresh the browser.

4. Other reasonable defaults based on development instead of production.

### 4.Run the Application

The main() method uses Spring Boot’s SpringApplication.run() method to launch an application.
In Gradle you can run the application by using `./gradlew bootRun`. Alternatively, you can build the JAR file by using `./gradlew` build and then run the JAR file, as follows:

```j
java -jar build/libs/gs-serving-web-content-0.1.0.jar
```

### 5.Test the Application

you can go to the request you create using client thunder or another tester.

### Add a Home Page

Static resources, including HTML and JavaScript and CSS, can be served from your Spring Boot application by dropping them into the right place in the source code. By default, Spring Boot serves static content from resources in the classpath at /static (or /public).

## how to access data from templates using Thymeleaf

### 1.Spring model attributes

There are a lot of methods to add attributes to a view in Spring MVC:

1. Add attribute to Model via its **addAttribute** method
2. Return **ModelAndView** with model attributes included
3. Expose common attributes via methods annotated with **@ModelAttribute**

### 2.Request parameters

Request parameters can be easily accessed in Thymeleaf views. Request parameters are passed from the client to server like:

```j
https://example.com/query?q=Thymeleaf+Is+Great!
```

### 3.Session attributes

the request parameters, session attributes can be accessed by using the **session** prefix

### 4.ServletContext attributes

The ServletContext attributes are shared between requests and sessions.on order to access them in Thymeleaf we can use the **#servletContext**.

### 5.Spring beans

Thymeleaf allows accessing beans registered at the Spring Application Context with the **@beanName** syntax, for example:

```java
<div th:text="${@urlService.getApplicationUrl()}">...</div>
```

## Resources used in this reading

1. [Serving Web Content with Spring MVC](https://spring.io/guides/gs/serving-web-content/)
2. [Spring MVC and Thymeleaf: how to access data from templates](https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)
