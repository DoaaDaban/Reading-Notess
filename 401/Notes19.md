# Spring and Sockets

## Real time messaging with websockets

* The WebSocket protocol is one of the ways to make The application handle real-time messages.

* The WebSocket protocol allows you to implement bidirectional communication between applications. It is important to know that HTTP is used only for the initial handshake. After it happens, the HTTP connection is upgraded to a newly opened TCP/IP connection that is used by a WebSocket.

* The WebSocket specification allows using of sub-protocols that operate on a higher, application level. One of them, supported by the Spring Framework, is **STOMP**.

* To build the WebSocket server-side, we will utilize the Spring Boot framework which significantly speeds up the development of standalone and web applications in Java. Spring Boot includes the spring-WebSocket module

### Implementing the WebSocket server-side with Spring Boot:

1. First, we should add these Dependencies:

```
implementation 'org.webjars:webjars-locator-core'
implementation 'org.webjars:sockjs-client:1.0.2'
implementation 'org.webjars:stomp-websocket:2.3.3'
implementation 'org.webjars:bootstrap:3.3.7'
implementation 'org.webjars:jquery:3.1.1-1'
```
2. Then, we can configure Spring to enable WebSocket and STOMP messaging.

3. Implement a controller that will handle user requests. It will broadcast received message to all users subscribed to a given topic.

4. Configure Spring for STOMP messaging
   
    * Annotat a `WebSocketConfig` by `@Configuration` to indicate that it is a Spring configuration class.

    * Also annotated with `@EnableWebSocketMessageBroker` to enables WebSocket message handling, backed by a message broker. 

### Implementing the WebSocket Client

1. Autowire Spring STOMP client.

2. Open a connection.