# Overview

**Network Address Translation (NAT)** allows multiple devices on a private network to share a single public IP address when accessing the Internet. It is commonly performed by home and enterprise routers.

## Address Types

- **Private IP Address** - Used within local networks.
- **Public IP Address** - Visible and reachable on the Internet.

## Benefits

- Conserves public IPv4 addresses.
- Hides internal network addresses.
- Allows multiple devices to access the Internet simultaneously.

## Goal

NAT translates private addresses into a public address, enabling communication between private networks and the Internet.

## Types of NAT

Network Address Translation can be implemented in several ways depending on the communication requirements.

### Source NAT (SNAT)

**Source NAT (SNAT)** modifies the **source IP address** of outgoing packets before they leave a private network. This is the most common form of NAT and allows multiple internal devices to communicate with external networks using one or more public IP addresses.

SNAT is typically used when devices on a private network access Internet services.

### Destination NAT (DNAT)

**Destination NAT (DNAT)** modifies the **destination IP address** of incoming packets before forwarding them to an internal host.

DNAT is commonly used to expose internal services, such as web servers or mail servers, to external clients while keeping the internal addressing scheme private.

### Port Address Translation (PAT)

**Port Address Translation (PAT)**, also known as **Network Address Port Translation (NAPT)** or **NAT Overload**, allows multiple devices to share a single public IPv4 address.

Instead of translating only IP addresses, PAT also translates transport-layer port numbers, allowing many simultaneous connections to coexist using the same public address.

PAT is the form of NAT most commonly implemented by home and small business routers.

## Why NAT Exists

One of the primary reasons for NAT is the limited number of available **IPv4 addresses**.

Because IPv4 provides approximately 4.3 billion unique addresses, widespread Internet adoption quickly exhausted the available address space. NAT delays IPv4 exhaustion by allowing thousands of private devices to share a much smaller pool of public IP addresses.

Although IPv6 largely removes this limitation through its vastly larger address space, NAT remains widely deployed in IPv4 networks.

## Limitations

While NAT provides address conservation and a degree of network isolation, it also introduces several limitations.

These include:

- Increased complexity when troubleshooting network connectivity.
- Additional processing performed by routers.
- Difficulties for applications that embed IP addresses within their payloads.
- Challenges for peer-to-peer communication and some real-time protocols.
- Port forwarding requirements when hosting internal services.

For these reasons, NAT should not be considered a security mechanism on its own, even though it hides private IP addresses from external networks.