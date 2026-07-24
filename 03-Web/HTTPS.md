# HyperText Transfer Protocol Secure (HTTPS)

## Overview

**HTTPS (HyperText Transfer Protocol Secure)** is the secure version of HTTP. It combines HTTP with **Transport Layer Security (TLS)** to provide encrypted communication between clients and web servers.

HTTPS protects sensitive information from interception, modification, and impersonation attacks, making it the standard protocol for modern websites.

## Transport Layer Security (TLS)

TLS establishes an encrypted connection before HTTP data is exchanged. It provides:

- Confidentiality through encryption.
- Integrity by detecting data modification.
- Authentication using digital certificates.

## Digital Certificates

A **digital certificate** verifies the identity of a website or service. Certificates contain the server's public key and are digitally signed by a trusted **Certificate Authority (CA)**.

Web browsers validate certificates before establishing secure communications, helping prevent impersonation attacks.

## TLS Handshake

Before encrypted communication begins, the client and server perform a **TLS Handshake**, during which they:

1. Negotiate the TLS version and encryption algorithms.
2. Verify the server's certificate.
3. Exchange cryptographic information.
4. Generate a shared session key used for symmetric encryption.

## Public Key Infrastructure (PKI)

HTTPS relies on a **Public Key Infrastructure (PKI)**, which consists of Certificate Authorities, digital certificates, and cryptographic key pairs used to establish trust between communicating parties.

## Benefits

HTTPS provides:

- Encrypted communication.
- Server authentication.
- Data integrity.
- Protection against eavesdropping.
- Protection against man-in-the-middle attacks.

## Goal

HTTPS secures web communication by combining HTTP with TLS, ensuring that data exchanged between clients and servers remains private, authentic, and resistant to tampering.