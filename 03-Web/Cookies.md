# Cookies

## Overview

Cookies are small pieces of data stored by a web browser on behalf of a website. Since HTTP is stateless, cookies allow websites to remember users between requests and provide features such as authentication, user preferences, and shopping carts.

## How Cookies Work

A server creates a cookie using the **Set-Cookie** header, which is stored by the browser. On future requests to the same website, the browser automatically sends the cookie back using the **Cookie** header, allowing the server to identify the client.

## Cookie Types

- **Session Cookies** - Exist only while the browser is open.
- **Persistent Cookies** - Remain stored until they expire or are manually deleted.

## Security

Important security attributes include **Secure**, which restricts cookies to HTTPS connections, **HttpOnly**, which prevents JavaScript access, and **SameSite**, which helps mitigate Cross-Site Request Forgery (CSRF) attacks.