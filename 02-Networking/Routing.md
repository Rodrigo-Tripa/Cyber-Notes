# Overview

Routing is the process of forwarding packets between different networks. This is performed by **routers**, which examine destination IP addresses and determine the best path for data to reach its destination.

## Routers

- Connect different networks.
- Forward packets between networks.
- Maintain routing information.

## Routing Decisions

Routers examine the destination IP address of each packet and use their routing table to decide where it should be forwarded next.

## Goal

Routing allows devices on different networks to communicate, making large-scale networks such as the Internet possible.

## Default Gateway

A **default gateway** is the router that forwards packets destined for networks outside the local subnet.

When a host determines that the destination IP address is not part of its own network, it sends the packet to the default gateway, which then forwards it toward the destination.

Without a correctly configured default gateway, devices can only communicate with hosts on the same local network.

## Static Routing

**Static routing** uses manually configured routes defined by a network administrator.

Static routes are simple, predictable, and consume minimal system resources, making them suitable for small or stable networks. However, they require manual updates whenever the network topology changes.

## Dynamic Routing

**Dynamic routing** allows routers to exchange routing information automatically using routing protocols.

This enables routers to discover new networks, adapt to topology changes, and automatically select the most efficient paths.

Common dynamic routing protocols include:

- RIP
- OSPF
- EIGRP
- BGP

Dynamic routing is widely used in medium and large networks where manual route management would be impractical.

## Routing Table

Every router maintains a **routing table**, which contains information about known networks and the paths used to reach them.

A routing table entry typically includes:

- Destination network
- Subnet mask or prefix
- Next-hop address
- Outgoing interface
- Route metric

Routers consult this table whenever they need to forward a packet.

## Longest Prefix Match

When multiple routes match the destination IP address, routers apply the **Longest Prefix Match** rule.

The route with the most specific network prefix is selected because it represents the closest match to the destination network.

For example, if both `192.168.0.0/16` and `192.168.1.0/24` exist in the routing table, traffic destined for `192.168.1.50` will follow the `/24` route.

## Time To Live (TTL)

The **Time To Live (TTL)** field in the IP header prevents packets from circulating indefinitely due to routing loops.

Each router decreases the TTL value by one before forwarding the packet. When the TTL reaches zero, the packet is discarded and an ICMP error message is typically returned to the sender.

TTL protects networks from infinite forwarding loops and is also used by diagnostic tools such as `traceroute` to discover the path taken by packets across a network.