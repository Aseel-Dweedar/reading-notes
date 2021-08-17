# Spring and Sockets

## Using WebSocket to build an interactive web application

How to build a server that accepts a message that carries a user’s name:

- **Starting with Spring Initializr.**

- **Adding Dependencies.**

- **Create a Resource Representation Class:**

  - The service will accept messages that contain a name in a STOMP message whose body is a JSON object.

  - Upon receiving the message and extracting the name, the service will process it by creating a greeting and publishing that greeting on a separate queue to which the client is subscribed. The greeting will also be a JSON object.

  - To model the message that carries the name, you can create a plain old Java object with a name property and a corresponding `getName()` method.

- **Create a Message-handling Controller**

  - In Spring’s approach to working with STOMP messaging, STOMP messages can be routed to `@Controller` classes.

  - Internally, the implementation of the method simulates a processing delay by causing the thread to sleep for one second.

- **Configure Spring for STOMP messaging**

- **Create a Browser Client**

  - With the server-side pieces in place, you can turn your attention to the JavaScript client that will send messages to and receive messages from the server side.

  - This HTML file imports the SockJS and STOMP javascript libraries that will be used to communicate with our server through STOMP over websocket.

- **Make the Application Executable**

> Spring Boot creates an application class for you. In this case, it needs no further modification. You can use it to run this application.

- **Build an executable JAR**

  - You can run the application from the command line with Gradle or Maven. You can also build a single executable JAR file that contains all the necessary dependencies, classes, and resources and run that.

- Test the service.

<hr>
<br>

**Sources**

- Using WebSocket to build an interactive web application / Spring Documentation.

**Go back -->** [Reading Notes](https://aseel-dweedar.github.io/reading-notes/)
