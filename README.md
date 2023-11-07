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

## 4xx 	
> Client Error
<br>

**400 - Bad Request**
---
> The request cannot be processed by the server because of a client error such as syntax, framing, or routing.
<br>

**401 - Unauthorized**
---
> Indicates that authentication is required and was either not provided or has failed. If the request already included authorization credentials, then the 401 status code indicates that those credentials were not accepted.
<br>

**402 - Payment Required**
---
> Reserved for future use. Originally intended to be part of a digital cash or micropayment model, this code is not currently widely used.
<br>

**403 - Forbidden**
---
> Indicates that though the request was valid, the server refuses to respond to it. Unlike the 401 status code, providing authentication will not change the outcome.
<br>

**404 - Not Found**
---
> Indicates that the requested resource could not be found but may be available in the future.
<br>

**405 - Method Not Allowed**
---
> The request method is not supported by the resource requested, as when using GET on a form that requires data to be presented via POST.
<br>

**406 - Not Acceptable**
---
> The requested content is not acceptable according to the requestÕs Accept headers.
<br>

**407 - Proxy Authentication Required (RFC 7235)**
---
> The client must first authenticate itself with the proxy.
<br>

**408 - Request Timeout**
---
> Indicates that the server timed out while waiting for the request, though the client may repeat the request without modifications.
<br>

**409 - Conflict**
---
> There is a conflict in the request that prevents it from being processedÑfor example, an edit conflict in the case of multiple updates.
<br>

**410 - Gone**
---
> The requested resource is no longer available and will not be available again, as when a resource has been intentionally removed and should be purged. The client should not request the resource again.
<br>

**411 - Length Required**
---
> The request did not specify the length of its content, though length is required by the requested source.
<br>

**412 - Precondition Failed (RFC 7232)**
---
> Indicates that the server does not meet the request preconditions as specified by requester.
<br>

**413 - Request Entity Too Large**
---
> Indicates that the request is larger than the server can or will process.
<br>

**414 - Request-URI Too Long**
---
> The provided URI was too long to be processed by the server. When resulting from too much data encoded as GET request query-string, convert to a POST request.
<br>

**415 - Unsupported Media Type**
---
> The server does not support the media type included by the request entity.
<br>

**416 - Requested Range Not Satisfiable (RFC 7233)**
---
> Indicates that the client has requested a portion of the file that the server is unable to provide, such as a part of the file that lies beyond the end of the file.
<br>

**417 - Expectation Failed**
---
> Indicates that the server is unable to meet the requirements of Expect request-header field.
<br>

**418 - I'm a teapot (RFC 2324)**
---
> Defined in 1998 as a traditional IETF April FoolÕs joke and is not expected to be implemented by actual HTTP servers. The RFC specifies that this code should be returned by teapots requested to brew coffee.
<br>

**419 - Authentication Timeout (not in RFC 2616)**
---
> Indicates that previously valid authentication has expired. Though not a part of the HTTP standard, the 419 status code is used as an alternative to 401 to differentiate from unauthorized clients being denied access.
<br>

**420 - Method Failure (Spring Framework)**
---
> Defined by Spring in the HttpStatus class to be used when a method fails. Not a part of the HTTP standard, this status code is deprecated by Spring.
<br>

**420 - Enhance Your Calm (Twitter)**
---
> Returned by version 1 of the Twitter Search and Trends API when the client is being rate limited. Not a part of the HTTP standard.
<br>

**421 - Misdirected Request (HTTP/2)**
---
> Indicates that the request is directed at a server that is unable to produce a response.
<br>

**422 - Unprocessable Entity (WebDAV; RFC 4918)**
---
> Indicates that the request is unable to be followed due to semantic errors.
<br>

**423 - Locked (WebDAV; RFC 4918)**
---
> Indicates that the resource that is being accessed is locked.
<br>

**424 - Failed Dependency (WebDAV; RFC 4918)**
---
>Indicates that the request failed because of the failure of a previous request.
<br>

**426 - Upgrade Required**
---
> Indicates that the client should switch to a different protocol as specified in the Upgrade header field.
<br>

**428 - Precondition Required (RFC 6585)**
---
> Indicates that origin server requires the request to be conditional to prevent the Òlost updateÓ problem.
<br>

**429 - Too Many Requests (RFC 6585)**
---
> Occurs when the user has sent too many requests in a given amount of time. For use with rate limiting.
<br>

**431 - Request Header Fields Too Large (RFC 6585)**
---
> Indicates that the request cannot be processed by the server because a single header field or all headers are collectively too large.
<br>

**440 - Login Timeout (Microsoft)**
---
> Microsoft extension indicating that the session has expired.
<br>

**444 - No Response (Nginx)**
---
> In Nginx logs as a malware deterrent, indicates that the server returned no information and closed the connection.
<br>

**449 - Retry With (Microsoft)**
---
> Microsoft extension indicating that the request should be retried after performing a specific action.
<br>

**450 - Blocked by Windows Parental Controls (Microsoft)**
---
> Microsoft extension indicating that Windows Parental Controls are turned on and blocking access to the page in question.
<br>

**451 - Unavailable For Legal Reasons (Internet draft)**
---
> Indicates that resource access has been denied for legal reasons such as censorship or government-mandated blocked access. Defined in the Internet draft as "A New HTTP Status Code for Legally-restricted Resources." References the dystopian novel Fahrenheit 451 (1953), in which books are outlawed.
<br>

**451 - Redirect (Microsoft)**
---
> In Exchange ActiveSync, used when there is a more efficient server or the server cannot access the clientÕs mailbox. The client should re-run the HTTP Autodiscovery protocol to find a better-suited server.
<br>

**494 - Request Header Too Large (Nginx)**
---
> Similar to 431, Nginx internal code earlier in version 0.9.4.
<br>

**495 - Cert Error (Nginx)**
---
> Nginx internal code indicating that SSL client certificate error has occurred
<br>

**496 - No Cert (Nginx)**
---
> Nginx internal code indicating that the client didn't provide a certificate.
<br>

**497 - HTTP to HTTPS (Nginx)**
---
> Nginx internal code indicating that plain HTTP requests were sent to the HTTPS port.
<br>

**498 - Token Expired/Invalid (Esri)**
---
> Returned by ArcGIS for Server when the token is expired or otherwise invalid.
<br>

**499 - Client Closed Request (Nginx)**
---
> In Nginx logs, indicates that the connection has been closed by the client while the server is still processing its request, in which case the server is unable to send a status code back.
<br>

**499 - Token Required (Esri)**
---
> Returned by ArcGIS for Server when a token is required but was not submitted.
<br>

## 5XX 	
> This category includes errors on the server side.
<br>

**500 - Internal Server Error**
---
> The server has encountered an unexpected error and cannot complete the request. 
<br>

**501 - Not Implemented**
---
> The server can’t fulfill the request or doesn’t recognize the request method. 
<br>

**502 - Bad Gateway**
---
> The server acts as a gateway and gets an invalid response from an inbound host.
<br>

**503 - Service Unavailable**
---
> The server is unable to process the request. This often occurs when a server is overloaded or down for maintenance. 
<br>

**504 - Gateway Timeout**
---
> The server was acting as a gateway or proxy and timed out, waiting for a response. 
<br>

**505 - HTTP Version Not Supported**
---
> The server doesn’t support the HTTP version in the request.
<br>

**506 - Variant Also Negotiates**
---
> The server has an internal configuration error. 
<br>

**507 - Insufficient Storage**
---
> The server doesn’t have enough storage to process the request successfully. 
<br>

**508 - Loop Detected**
---
> The server detects an infinite loop while processing the request. 
<br>

**511 - Network Authentication Required**
---
> The client must be authenticated to access the network. The error should include a link where the user can submit credentials.
<br>
