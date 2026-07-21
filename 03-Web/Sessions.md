# Sessions

## Overview

A **session** is a mechanism used by web applications to maintain a user's state across multiple HTTP requests. Since HTTP is a stateless protocol, sessions allow servers to recognize authenticated users and store temporary information throughout their interaction with a website.

## How Sessions Work

When a user successfully authenticates, the server creates a unique **Session ID** and stores session data on the server. The Session ID is sent to the client, usually through a cookie, and is included in subsequent requests so the server can identify the user.

## Security

Sessions should be protected by using unpredictable Session IDs, HTTPS, and secure cookie attributes such as **HttpOnly** and **Secure**. Poor session management can lead to attacks such as **Session Hijacking**, allowing attackers to impersonate legitimate users.