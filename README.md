# Webattacks-
**Identifying web Attacks Through logs**

In this we gonna learn following topics together:- 

1. WebApplication Architecture 
2. Web Server Logs Review
3. Tips and common issues 
4. Web Application Attacks Review 
5. Vulnerability Scans
6. Brute Force Attacks
7. SQL Injection 
8. File Inclusion 
9. XSS:Cross-site Scripting 
10. CSRF: Cross-Site Request Forgery
11. Other Log sources



#1. Web Application Architecture 

So here comes the Question What is **WebApp**?

Answer :- According to the wiki, "In Computing, a web application or web app is a client-server computer program which the client(including the user interface and client-side logic) runs in a web browser"

For example :- Static Webpage:---> Provides information 
               Dynamic Webpage:--> Provides information and features
               
     Usualluy Dynamic server are controlled by the Application server !          

Let's understand afew basics once again :-

**Internet** :-

A huge network composed of many smaller networks.

**WWW** :- 

World Wide Web - A specific portion of the Internet knwon as the "WEB " is a protocol 

**HTML** :- Hyper Text Markup Language 

Default Language to build web pages and web applications 

# Basic Web Application Architecture 

uses a 

* client server Model 
* Client makes a request and server answers the request
* And the porotocol is "http/https"


The client(web browsers) talks with the *web server* which is none other than **Presentation Layer**  and Web server talks with the **Application server** Middle/Business and Application server gonna connect with the Database server **Data Access**

**Important Note** 

Clients can't talk directly with Application or Database servers never ever.They can only talk with the **Web Server**

**Web Clients** 

Web Clients are also know as User Agents responsible for the followings :- 

* Sending requests to servers
* Web Browsers / Web crawlers 
* Mozilla Firefox, Microsoft Edge, Google Chrome
* ncat, telenet,curl,wget,programming languages..

![image](https://user-images.githubusercontent.com/42417756/210399658-e7ae9254-2d88-421b-b968-dadaf83b9fc6.png)
 Usecase of Telnet command 

wget can be considered as the text based web browser.It will send a request.

**Web Servers**

* The Primary function of a web server is to store, process and deliver web pages to the clients.
* Responsible for answering request to the clients.
* A few common Web Servers are :- 

* Apache :-https://httpd.apache.org
* Ngix   :- https://ngix.org
* Microsoft IIS :- https://www.iis.net/

Spoiler Alerts :- Apache and Ngix logs looks like almost the same, but Microsoft IIS have different log structures.

_www_ uses the protocol _HTTP_ to transmit message through computer networks. It uses the _client-server_ model to operate. Mozilla Firefox,Google chrome, and Microsoft Edge are examples of _web Browsers_.They are programs that send requests to web _servers_ like APache,Ngix and Microsoft IIS.

GET is an example of a HTTP _method_ and 200 is an example of a HTTP _status_ code.

**Question** 

Why TCP is known as connection orientation while UDP is called connectionless?

Since there are 3 ways handshakes in TCP but UDP directly sends tha packets so.

# HTTP Review:- 

* HTTP - HyperText Transfer Protocol 

what does meaning of a protocol?

In Telecommunication, a communication protocol is a system of rules that allow two or more entities of a communications system to transmit information via any kind of variation of a physical quantity.

* RFC7231 -https://tools.ietf.org/html/rfc7231

* Request Methods - sent by clients 

* Response status codes - sent by servers.

What is HTTP methods:-

GET :- Transfer a current representation of the target resource. Safe

HEAD :- Same as GET, but only transfer the satus the line and header section.

POST :- Perform resource-spacific processing on the request payload 
PUT :-  Replace all current representations of the target resource with the request payload.
DELETE:- Remove all current representations of the target resouces
CONNECT:- Establish a tunnel to the server identified by the target resource
OPTIONS:- Describe the communication options for the target resource.
TRACE:-  Perform a message loop-back test along the path.