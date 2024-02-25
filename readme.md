# Welcome to HTTP-Status-Code-Guide

This repository provides a comprehensive list of HTTP status codes along with their categories and descriptions.

# HTTP Status Code Definitions

HTTP status codes are standard response codes given by web servers on the internet. They communicate the status of the HTTP request made by a client, such as a web browser or an API consumer. These status codes are three-digit numbers grouped into different categories, each representing a specific outcome of the request-response cycle. They provide valuable information about whether a request was successful, encountered an error, or requires further action.

# Types of status codes
| Type | Name            | Description                                                                                   |
|------|-----------------|-----------------------------------------------------------------------------------------------|
| 1xx  | Informational   | The server has received the request and is continuing the process.                          |
| 2xx  | Success         | The request was received, understood, and accepted by the server.                            |
| 3xx  | Redirection     | Further action needs to be taken to complete the request.                                    |
| 4xx  | Client Error    | There was an error on the client side.                                                       |
| 5xx  | Server Error    | The server encountered an error while processing the request.                                 |

## Informational (1xx)

| Code | Name                | Description                                                            |
| ---- | ------------------- | ---------------------------------------------------------------------- |
| 100  | Continue            | The client should continue with its request.                           |
| 101  | Switching Protocols | The server is changing protocols, for example, switching to WebSocket. |

## Success (2xx)

| Code | Name                          | Description                                                                                                                                      |
| ---- | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------ |
| 200  | OK                            | The request was successful.                                                                                                                      |
| 201  | Created                       | The request has been fulfilled, and a new resource is created.                                                                                   |
| 202  | Accepted                      | The request has been accepted for processing, but the processing has not been completed.                                                         |
| 203  | Non-Authoritative Information | The server is a transforming proxy that received a 200 OK response from its origin but is returning a modified version of the origin's response. |
| 204  | No Content                    | The server successfully processed the request but is not returning any content.                                                                  |
| 205  | Reset Content                 | The server successfully processed the request, and the user agent should reset the document view which caused the request to be sent.            |
| 206  | Partial Content               | The server is delivering only part of the resource due to a range header sent by the client.                                                     |

|

## Redirection (3xx)

| Code | Name               | Description                                                                               |
| ---- | ------------------ | ----------------------------------------------------------------------------------------- |
| 300  | Multiple Choices   | The requested resource has multiple representations, each with its own specific location. |
| 301  | Moved Permanently  | The requested resource has been permanently moved to a new location.                      |
| 302  | Found              | The requested resource temporarily resides under a different URI.                         |
| 303  | See Other          | The response to the request can be found under a different URI.                           |
| 304  | Not Modified       | The client can use cached data.                                                           |
| 307  | Temporary Redirect | The requested resource resides temporarily under a different URI.                         |

## Client Error (4xx)

| Code   | Name                                | Description                                                                                                      |
| ------ | ----------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| 400    | Bad Request                         | The server cannot process the request due to a client error.                                                     |
| 401    | Unauthorized                        | The request requires user authentication.                                                                        |
| 402    | Payment Required                    | This code is reserved for future use.                                                                            |
| 403    | Forbidden                           | The server understood the request but refuses to authorize it.                                                   |
| 404    | Not Found                           | The server cannot find the requested resource.                                                                   |
| 405    | Method Not Allowed                  | The method specified in the request is not allowed for the resource identified by the request URI.               |
| 406    | Not Acceptable                      | The server cannot generate a response that the client will accept.                                               |
| 407    | Proxy Authentication Required       | The client must first authenticate itself with the proxy.                                                        |
| 408    | Request Timeout                     | The server timed out waiting for the request.                                                                    |
| 409    | Conflict                            | The request could not be completed due to a conflict with the current state of the target resource.              |
| 410    | Gone                                | The requested resource is no longer available at the server and no forwarding address is known.                  |
| 411    | Length Required                     | The server requires a content-length header.                                                                     |
| 412    | Precondition Failed                 | The precondition given in the request evaluated to false by the server.                                          |
| 413    | Payload Too Large                   | The server refuses to process the request because the payload is too large.                                      |
| 414    | URI Too Long                        | The server refuses to process the request because the URI is too long.                                           |
| 415    | Unsupported Media Type              | The server refuses to process the request because the entity's media type is unsupported.                        |
| 416    | Range Not Satisfiable               | The client has asked for a portion of the file, but the server cannot supply that portion.                       |
| 417    | Expectation Failed                  | The server cannot meet the requirements of the Expect request-header field.                                      |

| 418    | I'm a teapot                        | This code was defined in 1998 as one of the traditional IETF April Fools' jokes.                                 |
| 421    | Misdirected Request                 | The request was directed at a server that is not able to produce a response.                                     |
| 422    | Unprocessable Entity                | The request was well-formed but was unable to be followed due to semantic errors.                                |
| 423    | Locked                              | The resource that is being accessed is locked.                                                                   |
| 424    | Failed Dependency                   | The request failed due to failure of a previous request.                                                         |
| 425    | Too Early                           | Indicates that the server is unwilling to risk processing a request that might be replayed.                      |
| 426    | Upgrade Required                    | The client should switch to a different protocol.                                                                |
| 428    | Precondition Required               | The server requires the request to be conditional.                                                               |
| 429    | Too Many Requests                   | The user has sent too many requests in a given amount of time.                                                   |
| 431    | Request Header Fields Too Large     | The server refuses to process the request because the request's headers are too large.                           |
| 451    | Unavailable For Legal Reasons       | This status code indicates that the server is denying access to the resource as a consequence of a legal demand. |

## Server Error (5xx)

| Code | Name                       | Description                                                                                                 |
| ---- | -------------------------- | ----------------------------------------------------------------------------------------------------------- |
| 500  | Internal Server Error      | A generic error message, given when an unexpected condition was encountered on the server.                  |
| 501  | Not Implemented            | The server does not support the functionality required to fulfill the request.                              |
| 502  | Bad Gateway                | The server received an invalid response from an upstream server.                                            |
| 503  | Service Unavailable        | The server is currently unable to handle the request due to temporary overloading or maintenance.           |
| 504  | Gateway Timeout            | The server was acting as a gateway or proxy and did not receive a timely response from the upstream server. |
| 505  | HTTP Version Not Supported | The server does not support the HTTP protocol version used in the request.                                  |
| 506  | Variant Also Negotiates    | Transparent content negotiation for the request results in a circular reference.                            |
| 507  | Insufficient Storage       | The server is unable to store the representation needed to complete the request.                            |
| 508  | Loop Detected              | The server detected an infinite loop while processing the request.                                          |
| 510  | Not Extended               | Further extensions to the request are required for the server to fulfill.                                   |
