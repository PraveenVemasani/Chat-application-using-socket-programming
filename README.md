
# Simple Chat Connect

A simple chat system is a type of network application that allows communication between two users through the exchange of messages. The user can be any device that is connected to the network, such as a computer, smartphone, or tablet. 
In this project, one user sends a message to the other user and the other user receive and send messages to each other. 
To implement this application, you will need to use socket programming to create a server that listens for incoming connections and a client that connects to the server. The server and client can then exchange messages using the send and receive functions of the socket.
There are many variations of the client-server chat system, and the specific implementation will depend on the requirements and constraints of the application. However, the basic principles of communication between the client and server remain the same.



## Socket Programming

- Socket Programming is a Part of Transport Layer in a computer network.
- Java Socket programming is used for communication between the applications running on different JRE.
- Java Socket programming can be connection-oriented or connection-less(TCP and UDP are examples of protocols in Transport Layer.).
- TCP is a Connection-Oriented protocol whereas UDP is a connectionless protocol.
- In the world of Internet protocol traffic, user can choose between a TCP or UDP setup for their business or personal use. When it comes to TCP vs UDP features and functions, each brings its own set of advantages and challenges.


## Socket Programming in Java

- Socket programming is a way of connecting two nodes on a network to communicate with each other. One socket (node) listens on a particular port at an IP, while other socket reaches out to the other in order to form a connection. The server forms the listener socket while the client reaches out to the server. Socket and Server Socket classes are used for connection-oriented socket programming.

- In Java, a socket is a endpoint for sending or receiving data across a computer network. It is a way for a program to communicate with other programs running on the same or other computers.

- A socket is created using the java.net.Socket class. It represents the client side of a socket connection, and is used to establish a connection to a server and send and receive data over that connection. Once the connection is established, the client and server can communicate by reading and writing to the input and output streams of the socket.

## Client Side Programming

In the case of client-side programming, the client will first wait for the server to start. Once the server is up and running, it will send the requests to the server. After that, the client will wait for the response from the server. So, this is the whole logic of client and server communication.

**Establish a connection**
- The very first step is to establish a socket connection. A socket connection implies that the two machines have information about each other’s network location (IP Address) and TCP port.
**Communication**
- In order to communicate over a socket connection, streams are used for both input and output the data. After establishing a connection and sending the requests, you need to close the connection.
**Closing the connection**
- The socket connection is closed explicitly once the message to the server is sent.

## Server Side Programming

Basically, the server will instantiate its object and wait for the client request. Once the client sends the request, the server will communicate back with the response.

**Communication**
- getOutputStream() method is used to send the output through the socket.
**Close the Connection**
- It is important to close the connection by closing the socket as well as input/output streams once everything is done.

## Chat Application 
## Flow Diagram