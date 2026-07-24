# HyperText Transfer Protocol (HTTP)

## Overview

**HTTP (HyperText Transfer Protocol)** is the application-layer protocol used for communication between web clients and web servers. It follows a **request-response** model in which a client requests a resource and the server returns the requested content or an error message.

## HTTP Methods

The most common HTTP methods are:

- **GET** - Retrieves resources.
- **POST** - Sends data to the server.
- **PUT** - Creates or replaces resources.
- **DELETE** - Removes resources.
- **HEAD** - Retrieves only the response headers.

## Status Codes

HTTP responses contain status codes that indicate the result of a request. They are grouped into **1xx (Informational)**, **2xx (Success)**, **3xx (Redirection)**, **4xx (Client Errors)**, and **5xx (Server Errors)**. Common examples include **200 OK**, **301 Moved Permanently**, **404 Not Found**, and **500 Internal Server Error**.

## Stateless Protocol

HTTP is a **stateless protocol**, meaning each request is independent from previous ones. Websites rely on cookies, sessions, and authentication tokens to maintain user state across multiple requests.

## HTTP Message Structure

HTTP communication is based on a request-response model in which clients send requests and servers return responses.

An HTTP message consists of three main components:

- Start line
- Headers
- Message body (optional)

The exact structure depends on whether the message is a request or a response.

## HTTP Request

An HTTP request is sent by a client to request a resource from a web server.

A request contains:

- Request method
- Target resource (URL or path)
- HTTP version
- Request headers
- Optional message body

For example, a browser may send a `GET` request to retrieve a webpage or a `POST` request to submit form data.

## HTTP Response

After processing a request, the server returns an HTTP response.

A response contains:

- HTTP version
- Status code
- Status message
- Response headers
- Optional response body

The response body typically contains HTML, JSON, images, files, or other requested content.

## HTTP Headers

HTTP headers provide additional information about the request or response.

Common request headers include:

- Host
- User-Agent
- Accept
- Authorization
- Cookie

Common response headers include:

- Content-Type
- Content-Length
- Set-Cookie
- Cache-Control
- Server

Headers allow clients and servers to negotiate content, authentication, caching, compression, and many other communication features.

## Persistent Connections

In early versions of HTTP, a new TCP connection was established for every request.

Starting with **HTTP/1.1**, persistent connections became the default behaviour, allowing multiple requests and responses to reuse the same TCP connection.

Persistent connections reduce latency, decrease network overhead, and improve overall web performance.

## HTTP Versions

HTTP has evolved significantly since its introduction.

### HTTP/1.1

HTTP/1.1 introduced persistent connections, improved caching, virtual hosting support, and several performance enhancements. It remains widely supported today.

### HTTP/2

HTTP/2 significantly improves efficiency by allowing multiple requests and responses to be transmitted simultaneously over a single TCP connection through **multiplexing**. It also introduces header compression to reduce bandwidth usage.

### HTTP/3

HTTP/3 replaces TCP with the **QUIC** protocol, which operates over UDP. This reduces connection establishment time, improves performance on unreliable networks, and minimizes delays caused by packet loss while maintaining secure communication through TLS.