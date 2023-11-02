# HTTP Status Code

  An HTTP status code is a message a website's server sends to the browser to indicate whether or not that request can be fulfilled.

  The W3C sets status codes specs. Status codes are embedded in the HTTP header of a page to tell the browser the result of its request.

## The different status codes and what they say
There are five ranges of HTTP status codes. Each range defines where the error was encountered and the number defines what the actual error was.

Here are the 5 ranges and what they mean:


## Table of Contents

- [1xx: Informational](#1xx)
- [2xx: Success!](#2xx)
- [3xx: Redirect. The requested page has moved somewhere else.](#3xx)
- [4xx: Client error. There's something wrong with the way the browser asked for the page.](#4xx)
- [5xx: Server error. Something went wrong with the way the server tried to send the page.](#5xx)

## HTTP Status Codes Important for SEO
   Obviously, all status codes are important "You should know how healthy your site is" but there are certain ones that are particularly important for SEO(Search Engine Optimization) and anyone working on a website.


## 1xx
 **HTTP Informational Codes**

**100**
---
>  The HTTP 100 Continue informational status response code **indicates that everything so far is OK and that the client should continue with the request or ignore it if it is already finished.**
<br>

**101**
---
>  The HTTP 101 Switching Protocols response code **indicates a protocol to which the server switches.** The protocol is specified in the Upgrade request header received from a client. The server includes in this response an Upgrade response header to indicate the protocol it switched to
<br>

**102**
---
> The HTTP 102 Processing informational status response code **indicates to the client that a full request has been received and the server is working on it.** This status code is only sent if the server expects the request to take significant time. It tells the client that your request is not dead yet.
<br>

**103**
---
> The HTTP 103 **Early Hints** information response may be sent by a server while it is still preparing a response, with hints about the resources that the server is expecting the final response will link. This allows a browser to start preloading resources even before the server has prepared and sent that final response.
<br>

**122**
---
> An IE7-only code that indicates that the URI is longer than the maximum 2,083 characters.
<br>

## 2xx
> This status code category encompasses successful responses. 
<br>

**200 - OK**
---
> This is the standard response for successful HTTP requests. The actual meaning of the response depends on the request method used:

> **GET:** Resource obtained and is in the message body.

> **HEAD:** Headers are included in the response.

> **POST or PUT:** The Resource describing the result of the action sent is in the message body.

> **TRACE:** Message body contains the request message as received by the server.
<br>

**201 - Created:** 
> The request succeeded and a new resource was created. This is usually the response after POST or PUT requests. 
<br>

**202 — Accepted:** 
> The request was accepted but is still in progress. It’s used for cases where another server handles the request or for batch processing. 
<br>

**203 — Non-Authoritative Information:** 
> The data returned isn’t from the origin server. Instead, it’s a modified version collected from a third party. 
<br>

**204 — No Content:** 
> The request was successfully processed, but there is no content. The headers may be useful. 
<br>

**205 — Reset Content:** 
> The server fulfilled the request but asked the user to reset the document.
<br>

**206 — Partial Content:** 
> The server is delivering part of the resource. This response is used when the client sends a Range header to request only part of a resource. 
<br>

**207 — Multi-Status:** 
> Provides the statuses of multiple resources, depending on how many sub-requests were made. 
<br>

**208 — Already Reported:** 
> The members of a DAV:propstat element have already been listed and won’t be included again. 
<br>

**226 — IM used:** 
> The server completed a GET request. And the response indicates one or more instance-manipulation results.
<br>

## 3xx
> Redirection

**300 - Multiple Choices**
---
> Indicates multiple options for the resource delivered, such as format options for video or list files with different extensions. The user can select preferred representation and redirect the request to that location.
<br>

**301 - Moved Permanently**
---
> This request and all future ones should be directed to the given URI.
<br>

**302 - Found**
---
> Indicates that the requested resource can be found temporarily via an alternative URI. Because many popular user agent implementations treat 302 responses similar to 303 responses, both status codes 303 and 307 were added to allow servers more specificity.
<br>

**303 - See Other (since HTTP/1.1)**
---
> Indicates the response to the request can be found via alternative URI using GET method. Many pre-HTTP/1.1 user agents do not recognize 303, in which case the 302 status code can be used instead.
<br>

**304 - Not Modified (RFC 7232)**
---
> Indicates that the resource has not been modified since last requested, and there is no need to retransmit as the client has a previously downloaded copy.
<br>

**305 - Use Proxy (since HTTP/1.1)**
---
> Requested resource is located elsewhere and can be accessed through a proxy provided in the response. For security reasons, HTTP clients like Firefox and Internet Explorer do not correctly handle 305 responses.
<br>

**306 - Switch Proxy**
---
> Originally indicated that subsequent requests should use the proxy specified. This status code is no longer used.
<br>

**307 - Temporary Redirect (since HTTP/1.1)**
---
> Indicates that the request should be repeated with a different URI as specified, but future requests should use the original URI.
<br>

**308 - Permanent Redirect (RFC 7538)**
---
> This and all future requests should be repeated using a different URI as specified. Unlike 301 and 302, with 307 and 308 status codes the HTTP method should not change.
<br>
