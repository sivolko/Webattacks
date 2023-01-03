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

