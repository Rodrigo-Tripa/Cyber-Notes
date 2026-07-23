# Linux

## Overview

Linux is an open-source operating system kernel that serves as the foundation for many operating systems known as Linux distributions (distros). It is widely used in servers, cloud environments, embedded systems, Android devices, and cybersecurity due to its stability, flexibility, security, and open-source nature.

Unlike proprietary operating systems, Linux allows anyone to inspect, modify, and distribute its source code. This has led to the creation of many distributions, each designed for different use cases.

Common distributions include:

- Ubuntu
- Debian
- Fedora
- Arch Linux
- Kali Linux
- Parrot OS

## The Linux Kernel

The kernel is the core component of the operating system. It manages hardware resources, memory, processes, devices, and communication between software and hardware through system calls.

Different Linux distributions share the same kernel while providing different software, package managers, and desktop environments.

## Remote Administration

Linux systems are commonly administered remotely using SSH (Secure Shell). SSH provides encrypted communication between devices, allowing administrators to securely execute commands, transfer files, and manage systems over a network.

## Package Management

Software on Linux is typically installed through package managers, which automatically download, install, update, and remove software while managing dependencies.

Common package managers include:

- `apt`
- `dnf`
- `pacman`
- `zypper`

## Logging

Linux records system and application events in log files, most of which are stored under `/var/log`. These logs are essential for troubleshooting, system monitoring, auditing, and security investigations.

## Linux Shells

A shell is a command-line interpreter that acts as the interface between the user and the Linux kernel. It receives commands entered by the user, interprets them, launches programs, and displays their output.

Although graphical desktop environments are available, the shell remains the primary interface for system administration, remote management, automation, and cybersecurity. Most Linux servers operate without a graphical environment, making shell proficiency an essential skill.

Several shells are available, each offering different features and customization options.

Common Linux shells include:

- Bash (Bourne Again Shell)
- Zsh (Z Shell)
- Fish (Friendly Interactive Shell)
- Dash (Debian Almquist Shell)

While their syntax is similar for everyday tasks, they differ in scripting capabilities, performance, configuration, and interactive features.

## Environment Variables

Environment variables store configuration values that influence the behavior of the operating system, the shell, and applications.

They define information such as executable search paths, user directories, language settings, and temporary storage locations.

Common environment variables include:

- `PATH`
- `HOME`
- `USER`
- `SHELL`
- `PWD`
- `LANG`

Proper understanding of environment variables is important for configuring software, troubleshooting command execution, and developing portable scripts.

## The PATH Variable

The `PATH` environment variable contains a list of directories searched when a command is executed.

When a user enters a command without specifying its full path, the shell searches each directory listed in `PATH` until it finds a matching executable.

Maintaining a correctly configured `PATH` improves usability while preventing command execution issues caused by missing or incorrectly ordered directories.