# Spring and Sockets

In this reading we try to build a server that accepts a message that carries a user’s name. In response, the server will push a greeting into a queue to which the client is subscribed.

## Starting with Spring Initializr

in this step we creat apre initalized project and build it after decopress the zipped file.

## Adding Dependencies

The Spring Initializr does not provide everything,so we need to add the following dependencies in build.gradle:

```java
implementation 'org.webjars:webjars-locator-core'
implementation 'org.webjars:sockjs-client:1.0.2'
implementation 'org.webjars:stomp-websocket:2.3.3'
implementation 'org.webjars:bootstrap:3.3.7'
implementation 'org.webjars:jquery:3.1.1-1'
```

## Create a Resource Representation Class

In this step we create STOMP message service.

## Create a Message-handling Controller

In this step we create a controller to receive the hello message and send a greeting message.

## Configure Spring for STOMP messaging

configure Spring to enable WebSocket and STOMP messaging.
Create a Java class named WebSocketConfig .

## Create a Browser Client

* With the server-side pieces in place we can turn our attention to the JavaScript client that will send messages to and receive messages from the server side.

* This HTML file imports the SockJS and STOMP javascript libraries that will be used to communicate with our server through STOMP over websocket.

## Make the Application Executable

The main() method uses Spring Boot’s SpringApplication.run()  to launch an application.we can build a jar file contain all the necessary dependencies, classes, and resources and run that. by that we can easly deploy the app as running application.

## Test the service

The last thing to do is testing the app at the browser.

## Reading Resources

1. [Using WebSocket to build an interactive web application](https://spring.io/guides/gs/messaging-stomp-websocket/)
