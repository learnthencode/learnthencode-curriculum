# Introduction to the Web

## Overview

Before learning how to build websites, it is important to understand the environment in which they exist.

Every day, billions of people use the web to search for information, communicate with others, shop online, learn new skills, and access countless digital services. Behind every webpage is a collection of technologies working together to deliver content from computers around the world to users' devices.

In this lesson, you will explore the foundations of the web. You will learn how the Internet and the World Wide Web differ, how browsers communicate with servers, and what happens behind the scenes when you visit a website.

The goal is not to memorize networking terminology.

The goal is to develop a mental model of how information travels across the web before you begin building websites.

---

## Learning Objectives

By the end of this lesson, you should be able to:

- Explain the difference between the Internet and the World Wide Web.
- Describe the roles of clients and servers.
- Explain how browsers request and display webpages.
- Understand the purpose of URLs and domain names.
- Explain the role of the Domain Name System (DNS).
- Describe the HTTP request-response cycle.
- Explain why HTTPS is important.

---

## Why This Matters

Every website you build will rely on the technologies introduced in this lesson.

Understanding how browsers communicate with servers helps developers:

- Debug problems more effectively.
- Build faster and more reliable websites.
- Understand how web applications exchange information.
- Prepare for learning JavaScript, APIs, and backend development.

Professional web developers understand not only how to create webpages but also how those webpages reach users.

---

# Sub-lessons

## The Internet and the World Wide Web

Many people use the terms **Internet** and **World Wide Web (Web)** interchangeably, but they are not the same thing.

### The Internet

The Internet is a global network of interconnected computers that communicate with one another.

It provides the infrastructure that allows devices around the world to exchange information.

The Internet supports many services, including:

- The World Wide Web.
- Email.
- Online gaming.
- Video conferencing.
- File sharing.
- Cloud computing.

Think of the Internet as a worldwide transportation network.

---

### The World Wide Web

The World Wide Web is one of the services that runs on the Internet.

It consists of interconnected webpages and websites that users access through web browsers.

The relationship can be represented as:

```
Internet
    ↓
Provides the Network
    ↓
World Wide Web
    ↓
Websites and Web Applications
```

Without the Internet, the Web could not function.

However, the Internet can still exist without the Web because it supports many other services.

---

## Clients and Servers

The Web operates using a client-server model.

### Client

A client is a device or application that requests information.

Examples include:

- Google Chrome.
- Mozilla Firefox.
- Microsoft Edge.
- Safari.

When you type a website address into your browser, the browser acts as the client.

---

### Server

A server is a computer that stores websites or applications and responds to requests from clients.

For example:

When you visit a news website, your browser requests the webpage from the news organization's server.

The server processes the request and sends the webpage back to your browser.

The relationship can be represented as:

```
Client (Browser)
        ↓ Request
      Server
        ↓ Response
Client Displays Website
```

---

## Web Browsers

A web browser is software that allows users to access and interact with websites.

Examples include:

- Google Chrome.
- Mozilla Firefox.
- Microsoft Edge.
- Safari.

Browsers are responsible for:

- Sending requests to web servers.
- Receiving webpage files.
- Rendering webpages.
- Allowing users to interact with websites.

When you visit a website, the browser downloads resources such as:

- HTML.
- CSS.
- JavaScript.
- Images.
- Fonts.

It then combines these resources to display the webpage.

---

## URLs

A URL (Uniform Resource Locator) is the address used to locate a resource on the Web.

Example:

```
https://www.example.com/about
```

A URL typically contains:

```
Protocol
    ↓
https://

Domain Name
    ↓
www.example.com

Path
    ↓
/about
```

Each part helps the browser locate the correct resource.

---

## Domain Names

Humans prefer names, while computers communicate using IP addresses.

A domain name provides a human-friendly way to identify a website.

For example:

```
learnthencode.com
```

is much easier to remember than a numerical IP address.

---

## DNS (Domain Name System)

The Domain Name System (DNS) translates domain names into IP addresses.

A simplified process looks like this:

```
Domain Name
      ↓
DNS Lookup
      ↓
IP Address
      ↓
Server Found
```

Without DNS, users would need to memorize IP addresses for every website they visit.

---

## HTTP and HTTPS

When browsers and servers communicate, they follow rules called protocols.

The most common web protocol is HTTP.

HTTP stands for:

```
HyperText Transfer Protocol
```

HTTP defines how browsers request webpages and how servers respond.

---

### HTTPS

HTTPS stands for:

```
HyperText Transfer Protocol Secure
```

HTTPS encrypts communication between browsers and servers.

Benefits include:

- Improved security.
- Protection of sensitive information.
- Verification of website identity.
- Greater user trust.

Modern websites should always use HTTPS whenever possible.

---

## The Request-Response Cycle

Every time you visit a webpage, a series of events occurs.

```
User
   ↓
Types URL
   ↓
Browser
   ↓
DNS Lookup
   ↓
Server
   ↓
Processes Request
   ↓
Returns Response
   ↓
Browser Displays Webpage
```

This entire process usually happens within fractions of a second.

Understanding this cycle forms the foundation for learning frontend and backend development later in the bootcamp.

---

# Key Takeaways

- The Internet is the global network that connects computers.
- The World Wide Web is a service that operates on the Internet.
- Browsers act as clients that request webpages from servers.
- Servers store and deliver websites.
- URLs identify resources on the Web.
- DNS translates domain names into IP addresses.
- HTTP and HTTPS define how browsers and servers communicate.
- Every webpage is delivered through a request-response cycle.

---

# Summary

In this lesson, you learned:

- The difference between the Internet and the World Wide Web.
- How clients and servers communicate.
- The role of web browsers.
- The purpose of URLs and domain names.
- How DNS helps locate websites.
- The difference between HTTP and HTTPS.
- How webpages are delivered using the request-response cycle.

Remember:

> **Every website begins with a request. Understanding how that request travels across the web is the first step toward becoming a web developer.**

---

# Before You Continue

Before moving to the next lesson, make sure you can confidently:

- [ ] Explain the difference between the Internet and the World Wide Web.
- [ ] Describe the roles of clients and servers.
- [ ] Explain how browsers retrieve webpages.
- [ ] Describe the purpose of DNS.
- [ ] Explain the request-response cycle.
- [ ] Differentiate between HTTP and HTTPS.

If you are unsure about any of the above, review this lesson before continuing.

---

# What's Next?

Now that you understand how the web works, the next lesson will explore:

**HTML Fundamentals**

You will learn how webpages are structured using HTML, the standard markup language of the Web.