# Dynamic Host Configuration Protocol (DHCP)

## Overview

The **Dynamic Host Configuration Protocol (DHCP)** automatically assigns network configuration to devices when they join a network. Instead of manually configuring IP addresses, subnet masks, gateways, and DNS servers, clients obtain this information from a DHCP server.

DHCP simplifies network administration and reduces configuration errors, making it the standard method for assigning IP addresses in home, enterprise, and cloud environments.

## DORA Process

DHCP assigns addresses using a four-step process known as **DORA**:

1. **Discover** – The client broadcasts a request looking for DHCP servers.
2. **Offer** – A DHCP server offers an available IP address.
3. **Request** – The client requests the offered address.
4. **Acknowledgement (ACK)** – The server confirms the lease and provides the network configuration.

## DHCP Lease

A DHCP assignment is temporary and is known as a **lease**. Before the lease expires, the client attempts to renew it with the DHCP server. If renewal fails, the address eventually becomes available for reassignment.

## DHCP Reservation

Administrators can reserve specific IP addresses for particular devices using their MAC addresses. Reservations provide predictable addressing while still allowing DHCP to manage configuration automatically.

## DHCP Relay

A **DHCP Relay Agent** forwards DHCP messages between clients and DHCP servers located on different networks, allowing a centralized DHCP server to serve multiple subnets.

## Ports

DHCP uses the following UDP ports:

- UDP 67 – DHCP Server
- UDP 68 – DHCP Client

## Goal

DHCP automates IP address allocation and network configuration, allowing devices to join networks quickly while reducing administrative effort and configuration mistakes.