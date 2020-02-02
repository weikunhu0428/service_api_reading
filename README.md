# service_api_reading 
https://programminghistorian.org/en/lessons/creating-apis-with-python-and-flask

Start on Jan 21, 2020

quote useful information from above link
A web API allows for information or functionality to be manipulated by other programs via the internet. For example, with Twitter’s web API, you can write a program in a language like Python or Javascript that can perform tasks such as favoriting tweets or collecting tweet metadata.

the term API, short for Application Programming Interface, refers to a part of a computer program designed to be used or manipulated by another program, as opposed to an interface designed to be used or manipulated by a human

__HTTP__ (Hypertext Transfer Protocol) is the primary means of communicating data on the web. HTTP implements a number of “methods,” which tell which direction data is moving and what should happen to it. The two most common are GET, which pulls data from a server, and POST, which pushes new data to a server.

__URL__ (Uniform Resource Locator) - An address for a resource on the web, such as https://programminghistorian.org/about. A URL consists of a protocol (http://), domain (programminghistorian.org), and optional path (/about). A URL describes the location of a specific resource, such as a web page. When reading about APIs, you may see the terms URL, request, URI, or endpoint used to describe adjacent ideas. This tutorial will prefer the terms URL and request to avoid complication. You can follow a URL or make a GET request in your browser, so you won’t need any special software to make requests in this tutorial.

The query parameters follow the ? in the request, and are seperated from one another by the & symbol. 

First, examine the provided URL for an id and select the books that match that id. The id must be provided like this: ?id=0. Data passed through URLs like this (after the ?) are called query parameters—we’ve seen them before when we worked with the Chronicling America API. They’re a feature of HTTP used for filtering for specific kinds of data.

This part of the code determines if there is a query parameter, like ?id=0, and then assigns the provided ID to a variable.

Example
'/api/v1/resources/books',
http://127.0.0.1:5000/api/v1/resources/books?id=0


The prevailing design philosophy of modern APIs is called REST. For our purposes, the most important thing about REST is that it’s based on the four methods defined by the HTTP protocol: POST, GET, PUT, and DELETE. These correspond to the four traditional actions performed on data in a database: CREATE, READ, UPDATE, and DELETE. 

Continue (feb 20 2020)
Connecting Our API to a Database
