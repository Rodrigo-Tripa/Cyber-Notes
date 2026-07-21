## What is Offensive Security?

Offensive Security is the practice of testing the security of systems by simulating real-world attacks. The goal is to find vulnerabilities before malicious attackers do and help organizations fix them.

These tests are always performed with permission from the system owner.

## Offensive Security vs Defensive Security

**Offensive Security** focuses on finding and exploiting vulnerabilities to assess security.

**Defensive Security** focuses on protecting systems, detecting attacks, and responding to security incidents.

Both work together to improve an organization's overall security.

## Directory Enumeration

Directory enumeration is the process of discovering hidden files and directories on a web server.

A common tool for this is **DIRB**.

Example:

```bash
dirb http://<target-ip>
```

DIRB uses a wordlist to check whether common paths exist, such as:

* `/admin`
* `/login`
* `/images`
* `/backup`

Finding hidden directories can reveal pages or functionality that may be useful during a penetration test.

## Basic Pentesting Process

A penetration test generally follows these steps:

1. Reconnaissance
2. Enumeration
3. Exploitation
4. Post-Exploitation
5. Reporting

## Key Points

* Offensive Security aims to identify vulnerabilities before attackers.
* Directory enumeration helps discover hidden web resources.
* DIRB is one of several tools used for directory enumeration.
* Penetration testing follows a structured methodology rather than randomly using tools.
