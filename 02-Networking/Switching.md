# Switching

## Overview

Switching is the process of forwarding Ethernet frames between devices within a local area network (LAN). This function is performed by **network switches**, which use MAC addresses to determine where frames should be delivered.

Unlike hubs, switches send traffic only to the intended destination whenever possible, improving both network performance and security.

## MAC Address Table

A switch maintains a **MAC Address Table** (also called a **CAM Table**) that associates MAC addresses with physical switch ports.

When a frame arrives, the switch:

1. Learns the source MAC address.
2. Updates its MAC table.
3. Forwards the frame to the correct destination port if known.
4. Broadcasts the frame if the destination MAC address is unknown.

## Collision Domains

Each switch port represents its own **collision domain**, allowing devices to communicate simultaneously without interfering with one another. This significantly improves network efficiency compared to older hub-based networks.

## Broadcast Domains

By default, all ports on a switch belong to the same **broadcast domain**. Broadcast traffic is forwarded to every device connected to the switch unless the network is segmented using VLANs.

## Virtual LANs (VLANs)

A **Virtual LAN (VLAN)** logically separates devices into independent networks, even when they are connected to the same physical switch. VLANs improve security, reduce broadcast traffic, and simplify network management.

## Goal

Switching enables efficient communication within local networks by forwarding Ethernet frames based on MAC addresses while minimizing unnecessary network traffic.