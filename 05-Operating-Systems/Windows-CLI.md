## Overview

Windows provides two command-line environments: Command Prompt (CMD) and PowerShell. Both allow users to perform administrative tasks, automate processes, and manage the operating system without using the graphical interface.

## Command Prompt (CMD)

CMD is the traditional Windows command-line interpreter used for basic system administration and compatibility with older scripts.

## PowerShell

PowerShell is a modern shell that combines command-line functionality with scripting capabilities and object-oriented data processing.

## Common Tasks

- Navigate directories
- Manage files
- Display system information
- Execute administrative commands
- Run scripts

## Command Types

Windows command-line environments support several types of commands.

- **Internal commands** are built directly into the shell.
- **External commands** are executable files stored on disk.
- **PowerShell cmdlets** are .NET commands following the `Verb-Noun` naming convention.

Understanding the difference helps explain why some commands are always available while others depend on installed software or the system's environment variables.

## Navigation and File Management

Both CMD and PowerShell allow administrators to navigate the filesystem and manipulate files without using File Explorer.

Common operations include:

- Navigating directories
- Listing directory contents
- Creating files and folders
- Copying and moving files
- Renaming files
- Removing files and directories

These operations are fundamental during system administration, incident response, and penetration testing.

## System Enumeration

One of the primary uses of the Windows command line is collecting information about the local system.

Administrators and security professionals commonly retrieve information such as:

- Operating system version
- Hostname
- Logged-in users
- Running processes
- Installed services
- Hardware information
- Installed drivers
- Environment variables

System enumeration is often the first step when assessing an unfamiliar machine.

## Network Enumeration

Windows provides numerous built-in commands for inspecting network configuration and connectivity.

These commands allow administrators to obtain:

- IP configuration
- DNS configuration
- Routing information
- Active network connections
- Interface status
- Remote connectivity

Network enumeration is essential for troubleshooting communication issues and understanding how a system interacts with the network.


## Automation

Command-line environments make it possible to automate repetitive administrative tasks.

CMD supports traditional batch scripts (`.bat` and `.cmd`), while PowerShell provides a significantly more powerful scripting language capable of interacting with the operating system, Windows APIs, and the .NET runtime.

Automation reduces manual effort, improves consistency, and enables administrators to manage large numbers of systems efficiently.

## PowerShell Object Pipeline

Unlike traditional command-line interpreters that exchange plain text, PowerShell passes structured .NET objects between commands.

Because objects preserve their properties and methods, PowerShell can filter, sort, format, and manipulate data much more reliably than text-based shells.

This object-oriented pipeline is one of the features that distinguishes PowerShell from Command Prompt and makes it suitable for enterprise administration and large-scale automation.

## Help System

Both CMD and PowerShell include built-in documentation to help users discover commands and understand their available options.

Learning how to use the built-in help system is often more valuable than memorizing command syntax, as it allows administrators to quickly adapt to unfamiliar commands and environments.

## Why Cybersecurity Professionals Use the Command Line

Security professionals frequently rely on command-line interfaces because they provide direct access to operating system functionality with minimal overhead.

Tasks commonly performed through the command line include:

- Host enumeration
- Network diagnostics
- Process inspection
- Service management
- Log analysis
- Script execution
- Remote administration
- Incident response
- Digital forensics

Mastering command-line tools significantly improves efficiency and forms the foundation for advanced Windows administration, malware analysis, privilege escalation, and penetration testing.