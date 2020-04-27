# Nginx Questions

## Tutorial

* [Course: NGINX Web Server Deep Dive](https://linuxacademy.com/cp/modules/view/id/169)

## Questions

* What are locations? Where are they configured?
* How to configure new routes, for example, "/hi-am-a-route" send to XPTO api endpoint.
* The log files (/ var / log / nginx) of the routes and their structure.
* Relevant information about Proxypass.
* Throttled configuration
* How the relationship between the proxypass and the nginx of the apis that receive requests works.

### What is NGINX

nginx [engine x] is an HTTP and reverse proxy server, a mail proxy server, and a generic TCP/UDP proxy server, originally written by [Igor Sysoev](http://sysoev.ru/en/).

### Use Cases

* High performance web server:
  * Used by over 50% of the top 1,000 sites
* Reverse proxy :
  * SSL/TLS Termination
  * Content caching and compression
* Load Balancer

### Proxy vs. Reverse-Proxy

* Proxy:
  * Sits between our clients and the internet
  * Intermediate layer often used within organizations to monitor web traffic
* Reverse proxy :
  * Sits between internet traffic and our servers
  * Intermediate layer often used to load balance traffic & serve content from a cache

![IMAGE](img/proxy-reverse-proxy.png)

### What are locations

```nginx
Syntax:	location [ = | ~ | ~* | ^~ ] uri { ... }
location @name { ... }
Default:	—
Context:	server, location
```