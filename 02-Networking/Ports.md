# Overview

A **port** identifies a specific service or application running on a device. Ports allow multiple network services to operate simultaneously while sharing the same IP address.

## Port Forwarding

Port forwarding allows incoming traffic from the Internet to be redirected to a specific device and service within a private network.

## Goal

Ports ensure that network traffic reaches the correct application, while port forwarding makes selected internal services accessible from external networks.

## Port Ranges

Port numbers are divided into three standard ranges defined by the Internet Assigned Numbers Authority (IANA).

### Well-Known Ports

**Well-known ports** range from **0 to 1023** and are reserved for common network services.

Examples include:

| Port | Protocol | Service |
|------|----------|---------|
| 20/21 | TCP | FTP |
| 22 | TCP | SSH |
| 25 | TCP | SMTP |
| 53 | TCP/UDP | DNS |
| 67/68 | UDP | DHCP |
| 80 | TCP | HTTP |
| 110 | TCP | POP3 |
| 143 | TCP | IMAP |
| 443 | TCP | HTTPS |

### Registered Ports

**Registered ports** range from **1024 to 49151**.

These ports are assigned to software vendors and applications but can also be used by custom services.

Examples include:

- Microsoft SQL Server (1433)
- PostgreSQL (5432)
- MySQL (3306)
- RDP (3389)

### Dynamic Ports

**Dynamic**, **Private**, or **Ephemeral Ports** range from **49152 to 65535**.

Operating systems temporarily assign these ports to client applications when initiating outbound network connections.

Once the communication session ends, the operating system releases the port for future use.

## TCP vs UDP Ports

Both TCP and UDP use port numbers to identify network services, but they serve different purposes.

**TCP ports** support reliable, connection-oriented communication, making them suitable for applications that require guaranteed delivery, such as web browsing, email, and file transfers.

**UDP ports** provide fast, connectionless communication with minimal overhead. They are commonly used for services such as DNS, VoIP, video streaming, and online gaming, where low latency is more important than guaranteed delivery.

Because TCP and UDP maintain separate port spaces, the same port number can be used simultaneously by both protocols without conflict.

## Ephemeral Ports

An **ephemeral port** is a temporary client-side port automatically assigned by the operating system whenever an application initiates a network connection.

For example, when a web browser connects to an HTTPS server on port **443**, the operating system assigns an available ephemeral port as the source port. This allows multiple simultaneous connections to the same remote service while keeping each communication session uniquely identifiable.