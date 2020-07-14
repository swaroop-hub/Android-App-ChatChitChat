# Android-App-ChatChitChat
It's a chatroom Android app using java8 tools like websocket,okhttp3 where MULTIPLE devices can connect to a particular websocket and can chat share text ,images and vedios.

ABSTRACT
Chat application is a feature or a program on the Internet to communicate directly among Internet users who are online or who were equally using the internet. Chat applications allow users to communicate even though from a great distance.

PROBLEM STATEMENT
The project is designed to implement a chatroom android application using  java 8  tools like websocket,okhttp3  where multiple users can connect to the server and exchange information in the form of text ,images and videos.

software specifications :-
4.	Operating system :- windows 10
5.	software :- android studio, visual studio, node.js
6.	Libraries-websocket,okhttp3,websocketlistner etc 


INTRODUCTION
Java Networking
Java Networking is a concept of connecting two or more computing devices together so that we can share resources.
Java socket programming provides facility to share data between different computing devices.

Advantage of Java Networking
 	* sharing resources
 	* centralize software management
. 
The widely used java networking terminologies are given below:
->IP Address
->Protocol
->Port Number
->MAC Address
->Connection-oriented and connection-less protocol
->Socket


OVERVIEW OF THE PROJECT


Client Side Programming


1. Establish a Connection-A socket connection implies that the two machines have information about each other’s network location (IP Address) and TCP port.
 	Socket socket = new Socket(“127.0.0.1”, 5000)
 	Here, the first argument represents the IP address of Server.
 	The second argument represents the TCP Port. (It is a number that represents which application should run on a server.)
 	2. Communication 
 	In order to communicate over a socket connection, streams are used for both input and output the data. After establishing a connection and sending the requests, you need to close the connection.
 	3. Closing the connection 
            The socket connection is closed explicitly once the message to the server is sent
            
            
  Server Side Programming

 	Basically, the server will instantiate its object and wait for the client request. Once the client sends the request, the server will communicate back with the response.
 	In order to code the server-side application, you need two sockets and they are as follows:
 	A ServerSocket which waits for the client requests (when a client makes a new Socket())
 	A plain old socket for communication with the client. After this, you need to communicate with the client with the response.
 	Communication 
 	getOutputStream() method is used to send the output through the socket.
 	Close the Connection 
 	It is important to close the connection by closing the socket as well as input/output streams once everything is done.




HIGH LEVEL DESIGN

What is a Socket in Java? 
A socket in Java is one endpoint of a two-way communication link between two programs running on the network. A socket is bound to a port number so that the TCP layer can identify the application that data is destined to be sent to. An endpoint is a combination of an IP address and a port number. The package in the Java platform provides a class, Socket that implements one side of a two-way connection between your Java program and another program on the network


 Okhttp3
OkHttp is an HTTP client that’s efficient by default:
•	HTTP/2 support allows all requests to the same host to share a socket.
•	Connection pooling reduces request latency (if HTTP/2 isn’t available).
•	Transparent GZIP shrinks download sizes.
•	Response caching avoids the network completely for repeat requests.
OkHttp perseveres when the network is troublesome: it will silently recover from common connection problems. If your service has multiple IP addresses OkHttp will attempt alternate addresses if the first connect fails. This is necessary for IPv4+IPv6 and services hosted in redundant data centers. OkHttp supports modern TLS features (TLS 1.3, ALPN, certificate pinning). It can be configured to fall back for broad connectivity.











