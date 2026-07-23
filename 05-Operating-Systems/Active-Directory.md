# Active Directory

## Overview

Active Directory (AD) is Microsoft's directory service used to centrally manage users, computers, groups, and other network resources within Windows domains. It provides authentication, authorization, and centralized administration, making it a core component of most enterprise Windows environments.

---

## Domain

A **domain** is a logical administrative and security boundary that contains users, computers, groups, and other Active Directory objects.

All objects within a domain share a common directory database and can be managed centrally.

---

## Domain Controller (DC)

A **Domain Controller (DC)** is a Windows Server that hosts Active Directory Domain Services (AD DS).

Its primary responsibilities include:

- Authenticating users and computers
- Authorizing access to resources
- Storing the Active Directory database
- Applying Group Policies
- Replicating directory information with other Domain Controllers

Organizations typically deploy multiple Domain Controllers to improve availability and fault tolerance.

---

## Active Directory Objects

Active Directory stores information as objects.

Common object types include:

- Users
- Computers
- Groups
- Organizational Units (OUs)
- Printers
- Shared folders

Each object contains attributes that describe its properties.

---

## Organizational Units (OUs)

Organizational Units (OUs) are containers used to organize Active Directory objects.

They allow administrators to:

- Group related users and computers
- Delegate administrative control
- Apply Group Policies to specific parts of the domain

Unlike domains, OUs are organizational structures rather than security boundaries.

---

## Groups

Groups simplify permission management by assigning access rights to multiple users simultaneously.

Common group scopes include:

- Domain Local
- Global
- Universal

Instead of assigning permissions to individual users, administrators typically assign permissions to groups.

---

## Authentication

Authentication is the process of verifying the identity of a user or computer before access is granted.

Active Directory primarily uses **Kerberos** as its default authentication protocol.

### Kerberos

Kerberos is a ticket-based authentication protocol that allows users to securely access network resources without repeatedly sending passwords across the network.

It is the preferred authentication protocol in modern Active Directory environments.

### NTLM

NTLM (NT LAN Manager) is an older authentication protocol retained for compatibility with legacy systems.

Although still supported, it is generally less secure than Kerberos and should be avoided whenever possible.

---

## Authorization

After authentication, Active Directory determines which resources a user or computer is allowed to access.

Authorization decisions are based on:

- User permissions
- Group memberships
- Access Control Lists (ACLs)

---

## Group Policy (GPO)

A Group Policy Object (GPO) is a collection of settings that allows administrators to centrally configure Windows systems.

Common uses include:

- Password policies
- Security settings
- Software deployment
- Desktop configuration
- Login and startup scripts
- Windows Update settings

GPOs can be linked to domains, Organizational Units, or sites.

---

## Forests and Trees

Large organizations may consist of multiple domains.

### Tree

A tree is a collection of domains that share a contiguous namespace and trust each other.

### Forest

A forest is the highest-level Active Directory structure.

It consists of one or more trees that share:

- A common schema
- A common global catalog
- Trust relationships

A forest represents the overall security boundary of an Active Directory environment.

---

## Trust Relationships

Trust relationships allow users in one domain or forest to access resources located in another.

Trusts can be:

- One-way
- Two-way
- Transitive
- Non-transitive

These relationships enable resource sharing across different Active Directory environments.

---

## Summary

Active Directory provides centralized identity management, authentication, authorization, and policy enforcement for Windows enterprise environments. By organizing resources into domains, Organizational Units, groups, and forests, administrators can efficiently manage large networks while maintaining security and scalability.