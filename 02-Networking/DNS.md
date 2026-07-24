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

## Recursive and Iterative Queries

DNS name resolution can involve two types of queries: **recursive** and **iterative**.

In a **recursive query**, the DNS client asks a resolver to return the final answer. The resolver performs all necessary lookups on behalf of the client by contacting other DNS servers until the requested record is found or the query fails.

In an **iterative query**, each DNS server returns the best information it has available, often referring the requester to another DNS server closer to the final answer. The requester then continues the lookup process by querying the next server.

Recursive queries simplify name resolution for clients, while iterative queries reduce the workload placed on authoritative DNS servers.

## Reverse DNS Lookup

A **reverse DNS lookup** performs the opposite operation of a normal DNS query by resolving an IP address into a domain name.

Reverse lookups use **PTR (Pointer)** records and are commonly used for:

- Email server verification
- Network troubleshooting
- Logging and auditing
- Security investigations

## DNS Cache

To improve performance and reduce network traffic, DNS responses are temporarily stored in a **DNS cache**.

Caching occurs at multiple levels:

- Client operating systems
- Web browsers
- Recursive DNS resolvers

Cached records remain valid until their **Time To Live (TTL)** expires, after which a new query must be performed.

## DNS over HTTPS (DoH)

**DNS over HTTPS (DoH)** encrypts DNS queries using HTTPS, preventing attackers or network operators from viewing or modifying DNS requests in transit.

Because DoH uses standard HTTPS traffic, DNS requests are more difficult to intercept or filter.

## DNS over TLS (DoT)

**DNS over TLS (DoT)** also encrypts DNS traffic, but it establishes a dedicated TLS connection specifically for DNS communication.

Unlike DoH, which operates over HTTPS, DoT typically uses TCP port **853**. Both protocols improve user privacy by protecting DNS queries from eavesdropping and manipulation.