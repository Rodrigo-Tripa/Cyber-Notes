# Domain Name System (DNS)

## Overview

The **Domain Name System (DNS)** translates human-readable domain names into IP addresses, allowing users to access websites without memorizing numerical addresses. It is one of the Internet's core services and is used before communication with most online services can begin.

## DNS Resolution

When a client requests a domain, a **recursive resolver** performs the lookup by contacting the **Root Servers**, **Top-Level Domain (TLD) Servers**, and finally the **Authoritative Name Server**. Once the correct record is found, the result is returned to the client and cached according to its **Time To Live (TTL)** value.

## Common DNS Records

- **A** - Maps a domain to an IPv4 address.
- **AAAA** - Maps a domain to an IPv6 address.
- **CNAME** - Creates an alias for another hostname.
- **MX** - Specifies mail servers.
- **NS** - Identifies authoritative name servers.
- **TXT** - Stores verification and configuration data.
- **SOA** - Contains administrative information about a DNS zone.

## DNS Tools

The most common DNS troubleshooting tools are **nslookup** and **dig**, which allow administrators and penetration testers to query DNS records, troubleshoot name resolution, and perform reconnaissance against public infrastructure.