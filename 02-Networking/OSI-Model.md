# OSI Model

#networking #osi #tcp-ip #protocols

## Overview

The **Open Systems Interconnection (OSI) Model** is a conceptual framework that standardizes how networked systems communicate. Developed by the International Organization for Standardization (ISO), it divides network communication into seven logical layers, each responsible for a specific function.

Rather than describing specific protocols, the OSI Model provides a common language for understanding, designing, implementing, and troubleshooting computer networks. Although the Internet primarily uses the [[TCP-IP]] protocol suite, the OSI Model remains one of the most important references in networking and cybersecurity.

## Why the OSI Model Exists

Modern network communication is complex, involving many independent technologies and protocols. The OSI Model separates these responsibilities into layers so that each layer performs a specific task while interacting only with the layers directly above and below it.

This layered architecture provides several advantages:

- Standardizes network communication
- Simplifies troubleshooting
- Encourages interoperability between vendors
- Allows protocols to evolve independently
- Makes network design modular and scalable

## The Seven Layers

| Layer | Name | Primary Responsibility | Examples |
|--------|------|------------------------|----------|
| 7 | Application | Provides network services to applications | HTTP, HTTPS, DNS, SMTP, FTP |
| 6 | Presentation | Data formatting, encryption, compression | TLS, SSL, JPEG, UTF-8 |
| 5 | Session | Establishes and manages communication sessions | NetBIOS, RPC |
| 4 | Transport | Reliable end-to-end communication | TCP, UDP |
| 3 | Network | Logical addressing and routing | IPv4, IPv6, ICMP |
| 2 | Data Link | Local delivery using physical addresses | Ethernet, Wi-Fi, ARP |
| 1 | Physical | Transmission of electrical, optical, or radio signals | Copper, Fiber, Wireless |

## Layer Responsibilities

### Layer 7 – Application

The Application Layer is the closest layer to the user. It provides the network services used directly by applications, allowing software to communicate across the network.

Typical protocols include:

- HTTP / HTTPS
- DNS
- FTP
- SMTP
- IMAP
- POP3
- SSH

---

### Layer 6 – Presentation

The Presentation Layer prepares data for transmission by translating formats between different systems. It is also responsible for encryption, decryption, and data compression.

Common responsibilities include:

- Data encoding
- Encryption and decryption
- Compression
- Character encoding

---

### Layer 5 – Session

The Session Layer establishes, maintains, synchronizes, and terminates communication sessions between applications.

Its responsibilities include:

- Session establishment
- Session synchronization
- Session recovery
- Session termination

---

### Layer 4 – Transport

The Transport Layer provides end-to-end communication between hosts.

Its main responsibilities include:

- Data segmentation
- Flow control
- Error recovery
- Reliable delivery
- Port addressing

The two primary transport protocols are:

- **TCP** for reliable communication.
- **UDP** for fast, connectionless communication.

---

### Layer 3 – Network

The Network Layer enables communication between different networks by using logical addresses and routing.

Responsibilities include:

- IP addressing
- Routing
- Packet forwarding
- Path selection
- Fragmentation

Devices operating here:

- Routers
- Layer 3 Switches

Protocols include:

- IPv4
- IPv6
- ICMP

---

### Layer 2 – Data Link

The Data Link Layer enables communication between devices connected to the same local network.

Its responsibilities include:

- MAC addressing
- Frame creation
- Error detection
- Media access control

Devices operating here:

- Network Switches
- Wireless Access Points
- Network Interface Cards (NICs)

Protocols include:

- Ethernet
- Wi-Fi (802.11)
- ARP

---

### Layer 1 – Physical

The Physical Layer transmits raw bits across the communication medium.

It defines:

- Electrical signals
- Optical signals
- Radio signals
- Connectors
- Cabling
- Transmission speed

Examples include:

- Ethernet cables
- Fiber optic cables
- Wireless radio waves

## Protocol Data Units (PDUs)

Each OSI layer works with a different Protocol Data Unit (PDU).

| Layer | PDU |
|--------|-----|
| Application | Data |
| Presentation | Data |
| Session | Data |
| Transport | Segment (TCP) / Datagram (UDP) |
| Network | Packet |
| Data Link | Frame |
| Physical | Bits |

As data moves down the OSI stack, each layer adds its own header. This process is known as **encapsulation**. When data reaches the destination, each layer removes its corresponding header through **decapsulation**.

## Devices by Layer

| Device | Primary Layer |
|----------|--------------|
| Hub | Physical |
| Repeater | Physical |
| Network Interface Card (NIC) | Data Link |
| Switch | Data Link |
| Wireless Access Point | Data Link |
| Router | Network |
| Firewall | Network / Transport / Application |
| Proxy Server | Application |

Some modern devices, such as next-generation firewalls, operate across multiple layers simultaneously.

## OSI vs TCP/IP

The OSI Model is a theoretical framework, while the [[TCP-IP]] model represents the protocol suite used by the Internet.

| OSI | TCP/IP |
|------|---------|
| Application | Application |
| Presentation | Application |
| Session | Application |
| Transport | Transport |
| Network | Internet |
| Data Link | Link |
| Physical | Link |

Although the layer organization differs, both models describe the same communication process.

## Troubleshooting with the OSI Model

One of the OSI Model's greatest strengths is systematic troubleshooting. Network problems can be isolated by identifying which layer is responsible.

Examples include:

- **Layer 1:** Damaged cables, disconnected devices, faulty wireless signal.
- **Layer 2:** MAC address issues, switch failures, VLAN misconfiguration.
- **Layer 3:** Incorrect IP addresses, routing problems, unreachable networks.
- **Layer 4:** Blocked ports, TCP connection failures, UDP communication issues.
- **Layers 5–7:** Application errors, authentication failures, protocol misconfiguration, certificate problems.

Working layer by layer provides a structured approach to diagnosing network issues efficiently.

## Key Takeaways

- The OSI Model divides network communication into seven layers.
- Each layer has a specific responsibility and communicates with adjacent layers.
- Data is encapsulated as it travels down the stack and decapsulated at the destination.
- Different networking devices operate primarily at specific OSI layers.
- The OSI Model is a conceptual framework used to understand, design, and troubleshoot networks.
- Modern Internet communication is implemented using the [[TCP-IP]] protocol suite, but the OSI Model remains the standard reference for networking education and cybersecurity.