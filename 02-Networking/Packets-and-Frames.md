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