# Welcome to HTTP-Status-Code-Guide

This repository provides a comprehensive list of HTTP status codes along with their categories and descriptions.

# HTTP Status Code Definitions

HTTP status codes are standard response codes given by web servers on the internet. They communicate the status of the HTTP request made by a client, such as a web browser or an API consumer. These status codes are three-digit numbers grouped into different categories, each representing a specific outcome of the request-response cycle. They provide valuable information about whether a request was successful, encountered an error, or requires further action.

# Types of status codes

| Type  | Description                                                    |
|-------|----------------------------------------------------------------|
| 1xx   | Informational: The server has received the request and is continuing the process. |
| 2xx   | Success: The request was received, understood, and accepted by the server. |
| 3xx   | Redirection: Further action needs to be taken to complete the request. |
| 4xx   | Client Error: There was an error on the client side. |
| 5xx   | Server Error: The server encountered an error while processing the request. |


## Informational (1xx)

| Code | Description                                   |
|------|-----------------------------------------------|
| 100  | Continue: The client should continue with its request. |
| 101  | Switching Protocols: The server is changing protocols, for example, switching to WebSocket. |


## Success (2xx)

| Code | Description                                                    |
|------|----------------------------------------------------------------|
| 200  | OK: The request was successful.                               |
| 201  | Created: The request has been fulfilled, and a new resource is created. |
| 202  | Accepted: The request has been accepted for processing, but the processing has not been completed. |
| 203  | Non-Authoritative Information: The server is a transforming proxy that received a 200 OK response from its origin but is returning a modified version of the origin's response. |
| 204  | No Content: The server successfully processed the request but is not returning any content. |
| 205  | Reset Content: The server successfully processed the request, and the user agent should reset the document view which caused the request to be sent. |
| 206  | Partial Content: The server is delivering only part of the resource due to a range header sent by the client. |

