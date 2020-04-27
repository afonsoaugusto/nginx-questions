# Nginx

## **Questions**

---

@snap[north-west span-50 text-center]

### What is NGINX

@snapend

nginx [engine x] is an HTTP and reverse proxy server, a mail proxy server, and a generic TCP/UDP proxy server, originally written by [Igor Sysoev](http://sysoev.ru/en/).

---
@snap[north-west span-50 text-center]

### Use Cases

@snapend

@snap[span-50 text-07]
@ul
- High performance web server:
    - Used by over 50% of the top 1,000 sites
- Reverse proxy :
    - SSL/TLS Termination
    - Content caching and compression
- Load Balancer
@ulend
@snapend

---
@snap[north-west span-50 text-center]

#### Proxy vs. Reverse-Proxy

@snapend

@snap[span-50 text-07]
@ul
- Proxy:
    - Sits between our clients and the internet
    - Intermediate layer often used within organizations to monitor web traffic
- Reverse proxy :
    - Sits between internet traffic and our servers
    - Intermediate layer often used to load balance traffic & serve content from a cache.
@ulend
@snapend

---
@snap[north-west span-50 text-center]

#### Proxy vs. Reverse-Proxy

@snapend

![IMAGE](assets/img/proxy-reverse-proxy.png)

---

```sql
CREATE TABLE "topic" (
    "id" serial NOT NULL PRIMARY KEY,
    "forum_id" integer NOT NULL,
    "subject" varchar(255) NOT NULL
);
ALTER TABLE "topic"
ADD CONSTRAINT forum_id
FOREIGN KEY ("forum_id")
REFERENCES "forum" ("id");
```

---

@snap[north-west span-50 text-center]

### What are locations?

@snapend

```nginx
Syntax:	location [ = | ~ | ~* | ^~ ] uri { ... }
location @name { ... }
Default:	—
Context:	server, location
```

















---

@snap[north-east span-100 text-pink text-06]
Let your code do the talking!
@snapend

```sql zoom-18
CREATE TABLE "topic" (
    "id" serial NOT NULL PRIMARY KEY,
    "forum_id" integer NOT NULL,
    "subject" varchar(255) NOT NULL
);
ALTER TABLE "topic"
ADD CONSTRAINT forum_id
FOREIGN KEY ("forum_id")
REFERENCES "forum" ("id");
```

@snap[south span-100 text-gray text-08]
@[1-5](You can step-and-ZOOM into fenced-code blocks, source files, and Github GIST.)
@[6,7, zoom-13](Using GitPitch live code presenting with optional annotations.)
@[8-9, zoom-12](This means no more switching between your slide deck and IDE on stage.)
@snapend
