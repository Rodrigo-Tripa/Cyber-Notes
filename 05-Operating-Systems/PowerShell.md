# PowerShell

## Overview

PowerShell is Microsoft's task automation and configuration management framework. It combines a command-line shell with a powerful scripting language built on the .NET platform, enabling administrators to manage Windows systems, automate repetitive tasks, and interact with local and remote resources.

Unlike traditional command-line interpreters, PowerShell processes structured .NET objects instead of plain text. This object-oriented design allows commands to exchange rich information without requiring complex text parsing, making PowerShell significantly more powerful for system administration and automation.

PowerShell is available on Windows by default and, through PowerShell (formerly PowerShell Core), is also supported on Linux and macOS.

## Cmdlets

PowerShell commands are called **cmdlets**.

Cmdlets follow a consistent **Verb-Noun** naming convention, making commands easier to discover and understand.

Examples include:

- `Get-Process`
- `Get-Service`
- `Get-ChildItem`
- `Get-Help`
- `Set-Location`

The standardized naming convention provides a predictable interface across the entire PowerShell ecosystem.

## Object Pipeline

One of PowerShell's defining features is its object pipeline.

Instead of passing plain text between commands, PowerShell passes complete .NET objects that contain properties and methods.

Because commands receive structured objects rather than raw strings, administrators can easily filter, sort, select, group, and manipulate data without relying on complex text processing.

This object-oriented pipeline is one of the primary reasons PowerShell is preferred for enterprise administration and large-scale automation.

## Variables

PowerShell allows data to be stored in variables using the `$` prefix.

Variables can store many types of information, including:

- Strings
- Numbers
- Arrays
- Objects
- Boolean values

Since PowerShell is built on .NET, variables can represent complex objects rather than simple text values.

## Scripting

PowerShell supports scripting through `.ps1` files.

Scripts allow administrators to automate repetitive tasks such as:

- User management
- Software installation
- System configuration
- Service management
- Log collection
- Security auditing

PowerShell scripts can include variables, loops, conditional statements, functions, modules, and error handling, making the language suitable for both simple automation and complex administrative workflows.

## Modules

PowerShell functionality can be extended through modules.

A module is a collection of cmdlets, functions, variables, and scripts focused on a particular technology or administrative task.

Microsoft and third-party vendors provide modules for managing services such as:

- Active Directory
- Azure
- Microsoft 365
- Hyper-V
- Exchange Server
- SQL Server

Modules make PowerShell highly extensible and adaptable to different environments.

## Remote Administration

PowerShell supports remote administration through **PowerShell Remoting**, which allows administrators to execute commands on remote systems without direct physical access.

Remote management enables organizations to administer multiple computers simultaneously, automate deployments, collect information, and perform maintenance across enterprise environments.

## Execution Policy

PowerShell includes an execution policy mechanism that controls whether scripts are allowed to run.

Execution policies help reduce accidental script execution but are **not** considered a security boundary.

Common execution policies include:

- Restricted
- RemoteSigned
- AllSigned
- Unrestricted
- Bypass

Organizations commonly configure execution policies according to their security requirements.

## Security

PowerShell is extensively used by both system administrators and cybersecurity professionals.

Legitimate uses include:

- System administration
- Configuration management
- Automation
- Incident response
- Digital forensics

Because of its powerful capabilities, PowerShell is also frequently abused by attackers for reconnaissance, privilege escalation, persistence, and post-exploitation activities.

Modern versions of Windows include several security mechanisms that improve PowerShell visibility and auditing, including script block logging, transcription logging, and integration with the Antimalware Scan Interface (AMSI).

## Why It Matters

PowerShell has become the standard automation and administration platform for modern Windows environments.

Its object-oriented architecture, extensive scripting capabilities, remote administration support, and deep integration with Windows make it an essential skill for system administrators, cloud engineers, incident responders, blue team analysts, red team operators, and penetration testers.