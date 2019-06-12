---
title: What is AJAX and how it works
date: '2019-06-03 11:08:52'
description: ' ' 
---

---
## AJAX
---

**AJAX** stands for **A**synchronous **J**avascript **A**nd **X**ML

It is a technique by which we request data from a remote server without reloading the entire page.

#### Asynchronous in AJAX

Asynchronous in AJAX means that we are **exchanging data** to/from the server in the background **without having to refresh the page**.  

#### Standard Client Server Application

<!-- Insert Image Here -->

In standard client server applications, client requests data from the server, and in turn the server responds to the client with the appropriate data. 

The client has to wait for the server to respond to execute other tasks on the webpage.

These are also known as static application, not a dynamic application.

We want AJAX to make our application dynamic in nature.

#### Requests in Standard AJAX Application  

In standard ajax server applications, client can have multiple instances of request to the same server at the same time. 

Also, the client does not have to wait for the server to respond to make a new request.

>Multiple requests are happening concurrently and the client does't have to wait for a response from a server in order to make a new request.

#### Responses in Standard AJAX Application

Responses in standard AJAx applications are handled in the form of callbacks.

> A callback is a special function which is used in AJAX so the server can respond when it is ready to send data to the client.

---
## Implementation of AJAX into an application
---

#### Step 1: Create a XMLHttpRequest object

All modern browsers support XMLHttpRequest object.

The XMLHttpsRequest object can be used to exchange data with a server behind the scenes.  

This means that it is possible to update parts of a webpage, without reloading the whole webpage.

#### Syntax for XMLHttpRequest object

`var xhttp = new XMLHttpRequest();`

#### Step 2: Make a request to the server

`xhttp.open("GET", "ajax_info.txt", true);

##### to send a request to a server, use the open() and send() methods of the XMLHttpRequest object

##### .open method is used to make a request

##### "GET" : method used in request. It can be get or post

##### "ajax_info.txt" : URL of the file that we want to load into our webpage

##### true : indicates that we are making asynchronous request if we set it to false then it will not be a ajax request

#### Step 3: Handling the response from the server

##### The readyState property of XMLHttpsRequest object holds the status of the XMLHttpRequest.

##### The onreadystatechange property defines a function to be executed when the readyState changes.

##### The status property and the statusText property holds the status of the XMLHttpRequest object.

#### readyState: Holds the status of XMLHttpsRequest

- 0: request not initialized
- 1: server connection established
- 2: request received
- 3: processing request
- 4: request finished and response ready

#### status:

- 200: "OK"
- 403: "forbidden"
- 404: "page not found"