# File Systems

## Overview

A file system defines how an operating system stores, organizes, and retrieves data on storage devices. It manages files, directories, metadata, permissions, and the allocation of available storage space.

---

## Common File Systems

### NTFS

NTFS (New Technology File System) is the default file system used by modern Windows systems.

Its main features include:

- Journaling
- Access Control Lists (ACLs)
- File compression
- Encrypting File System (EFS)
- Alternate Data Streams (ADS)
- Support for large files and volumes

### ext4

ext4 is the most widely used file system on Linux distributions.

Its features include:

- Journaling
- High performance
- Reliability
- Large file and volume support
- Efficient storage allocation

---

## Directories

File systems organize data using a hierarchical directory structure that allows users and applications to efficiently locate and manage files.

Directories can contain both files and other directories, forming a tree-like hierarchy.

---

## Metadata

Every file stores metadata describing its properties rather than its contents.

Common metadata includes:

- Filename
- File size
- Owner
- Permissions
- Creation time
- Modification time
- Last access time

---

## Permissions

File systems implement permission models to control who can read, write, modify, or execute files and directories.

Permissions help protect sensitive data and enforce access control between users and applications.

---

## Journaling

Many modern file systems use journaling to record pending changes before they are written to disk.

If the system crashes unexpectedly, the journal helps recover the file system and reduces the risk of corruption.

---

## Linux Directory Structure

Linux organizes files under a single directory hierarchy rooted at `/`.

Common directories include:

| Directory | Purpose |
|-----------|---------|
| `/home` | User home directories |
| `/etc` | System configuration files |
| `/usr` | User applications and libraries |
| `/var` | Variable data such as logs and databases |
| `/tmp` | Temporary files |
| `/boot` | Bootloader and kernel files |
| `/dev` | Device files |
| `/proc` | Virtual process and kernel information |
| `/sys` | Kernel and hardware information |

---

## Windows Directory Structure

Windows stores system files on a drive identified by a drive letter, typically `C:\`.

Common directories include:

| Directory | Purpose |
|-----------|---------|
| `C:\Windows` | Operating system files |
| `C:\Windows\System32` | Core system components and utilities |
| `C:\Program Files` | 64-bit applications |
| `C:\Program Files (x86)` | 32-bit applications |
| `C:\Users` | User profiles |
| `C:\ProgramData` | Shared application data |

---

## Summary

A file system is responsible for organizing, protecting, and managing data stored on a device. Understanding different file systems and directory structures is essential for system administration, troubleshooting, digital forensics, and cybersecurity.