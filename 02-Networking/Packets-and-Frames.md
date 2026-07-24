# Overview

Data is transmitted across networks by breaking it into smaller units. At different layers of the OSI Model, these units are called **packets** and **frames**, each containing information required for successful communication.

## Packets

- Operate at the **Network Layer (Layer 3)**.
- Contain source and destination IP addresses.
- Routed between different networks.

## Frames

- Operate at the **Data Link Layer (Layer 2)**.
- Contain source and destination MAC addresses.
- Used for communication within a local network.

## Goal

Packets allow data to travel between networks, while frames deliver that data across the local network. Together, they provide reliable communication from source to destination.

## Segments and Datagrams

At the **Transport Layer**, data is divided into smaller units before being transmitted across the network.

When using **TCP**, these units are called **segments**. Each segment includes sequence numbers, acknowledgements, and other control information that allow TCP to provide reliable, ordered communication.

When using **UDP**, the units are called **datagrams**. Unlike TCP segments, UDP datagrams contain minimal control information and are transmitted without guaranteeing delivery, ordering, or error recovery.

Both segments and datagrams are encapsulated into IP packets before being transmitted across the network.

## Packet Structure

A network packet consists of two main components:

- **Header**
- **Payload**

The **header** contains control information required for communication, such as source and destination addresses, protocol information, packet length, and other metadata.

The **payload** contains the actual application data being transmitted between hosts.

As packets move through the network, different protocols add their own headers to provide the information required by each networking layer.

## Frame Structure

At the Data Link Layer, packets are encapsulated inside **frames** before being transmitted across the physical medium.

A frame typically contains:

- Header
- Payload
- Trailer

The frame header contains MAC addresses and other information required for local network communication, while the trailer usually includes an error detection mechanism such as a **Frame Check Sequence (FCS)**.

Frames exist only within a single local network. When a router forwards traffic to another network, the existing frame is removed and a new one is created for the next network segment.

## Maximum Transmission Unit (MTU)

The **Maximum Transmission Unit (MTU)** defines the largest amount of data that can be transmitted within a single frame without fragmentation.

For Ethernet networks, the default MTU is typically **1500 bytes**.

If a packet exceeds the MTU, it may be fragmented into smaller packets or rejected, depending on the network configuration and protocol in use.

Choosing an appropriate MTU improves network efficiency while minimizing fragmentation.

## Encapsulation Example

When a user requests a webpage, the transmitted data moves through multiple protocol layers before reaching the network.

The encapsulation process follows this sequence:

1. The application creates the HTTP request.
2. TCP adds a transport header, creating a **segment**.
3. IP adds a network header, creating a **packet**.
4. Ethernet adds a frame header and trailer, creating a **frame**.
5. The frame is transmitted as a stream of **bits** across the physical medium.

At the destination, each layer removes its corresponding header through **decapsulation** until the original HTTP request is delivered to the web server.