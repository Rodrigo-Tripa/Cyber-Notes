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