# TCP/IP Protocol Suite

## Overview

The **TCP/IP (Transmission Control Protocol/Internet Protocol)** protocol suite is the standard networking model used by the Internet and modern computer networks. It defines how data is transmitted between devices by dividing communication into multiple layers, each responsible for a specific part of the communication process.

Unlike the OSI Model, which serves primarily as a conceptual framework, the TCP/IP model describes the protocols that are actually implemented in real-world networks.

## TCP/IP Layers

| Layer | Purpose | Example Protocols |
|------|--------------------------|-------------------------|
| Application | Provides network services to applications | HTTP, HTTPS, DNS, FTP, SMTP, SSH |
| Transport | End-to-end communication | TCP, UDP |
| Internet | Logical addressing and routing | IPv4, IPv6, ICMP |
| Link | Local network communication | Ethernet, Wi-Fi, ARP |

## Transport Protocols

### TCP

**Transmission Control Protocol (TCP)** provides reliable, connection-oriented communication. It guarantees that data is delivered completely, in the correct order, and without duplication through acknowledgements, sequencing, and retransmissions.

TCP is commonly used for:

- HTTP / HTTPS
- SSH
- FTP
- SMTP
- IMAP
- POP3

### UDP

**User Datagram Protocol (UDP)** is a connectionless protocol that prioritizes speed over reliability. Packets are transmitted without acknowledgements or retransmissions, making UDP suitable for applications where low latency is more important than guaranteed delivery.

UDP is commonly used for:

- DNS
- DHCP
- VoIP
- Video streaming
- Online gaming

## ICMP

The **Internet Control Message Protocol (ICMP)** is used for diagnostics, error reporting, and network troubleshooting rather than transporting application data. Tools such as `ping` and `traceroute` rely on ICMP messages to verify connectivity and identify routing paths.

## ARP

The **Address Resolution Protocol (ARP)** resolves IPv4 addresses into MAC addresses within a local network, allowing devices to locate one another before transmitting Ethernet frames.

## OSI vs TCP/IP

The TCP/IP model closely maps to the OSI Model:

| TCP/IP | OSI |
|---------|---------------------------|
| Application | Application, Presentation, Session |
| Transport | Transport |
| Internet | Network |
| Link | Data Link, Physical |

## Goal

The TCP/IP protocol suite provides the practical framework that enables devices to communicate across local and global networks. Understanding its layers and protocols is essential for network administration, troubleshooting, packet analysis, and cybersecurity.