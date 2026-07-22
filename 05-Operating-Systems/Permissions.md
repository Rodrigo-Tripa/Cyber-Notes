# Permissions

## Overview

Linux uses a permission system to control who can access files and directories. Every file has an owner, an associated group, and a set of permissions that determine whether users can read, modify, or execute it.

This model helps protect the system from unauthorized access while allowing multiple users to share the same machine securely.

## Permission Types

Linux defines three basic permissions:

- **Read (`r`)** - Allows viewing the contents of a file or listing a directory.
- **Write (`w`)** - Allows modifying a file or creating, deleting, and renaming files within a directory.
- **Execute (`x`)** - Allows running a file as a program or entering a directory.

## Permission Classes

Permissions are assigned separately to three classes of users:

- **Owner** - The user who owns the file.
- **Group** - Users belonging to the file's group.
- **Others** - All remaining users.

## Ownership

Every file and directory belongs to both a user and a group. Ownership and permissions can be modified using common administrative commands such as:

- `chmod` - Change permissions.
- `chown` - Change the file owner.
- `chgrp` - Change the file group.

## Why Permissions Matter

The Linux permission model is a fundamental security feature. It prevents unauthorized access, protects sensitive files from accidental modification, and allows administrators to control what each user or process can do on the system.