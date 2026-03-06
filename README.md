# active-directory-domain-lab

Windows Server 2022 Active Directory lab demonstrating domain controller deployment, DNS configuration, domain join, and domain authentication using a Windows 10 client.

## Overview

This lab demonstrates how to deploy an Active Directory environment from scratch using Windows Server 2022. A domain controller was configured with DNS services and a new forest was created. A Windows 10 client was then joined to the domain and authenticated using domain user credentials.

The objective was to simulate a small enterprise network where centralized identity management is used to authenticate users across multiple systems.

## Technologies Used

- Windows Server 2022
- Active Directory Domain Services (AD DS)
- DNS Server
- Windows 10
- Oracle VirtualBox

## Lab Environment

Host Machine  
Windows 11

Virtual Machines

Domain Controller
- Windows Server 2022
- 6GB RAM
- 2 CPU cores
- Static IP: 10.0.0.10

Client Machine
- Windows 10
- 4GB RAM
- 2 CPU cores
- Domain Joined

Network Configuration
Internal VirtualBox network used to simulate an enterprise LAN.

## Domain Configuration

Domain Name

company.local

Active Directory Roles Installed

- Active Directory Domain Services
- DNS Server
- Group Policy Management

## Organizational Structure

Organizational Units

Company
- HR
- Finance
- IT

Domain Users

Derek Jeter – HR  
Alex Rodriguez – Finance  
Babe Ruth – IT  

## Domain Join Process

The Windows 10 client machine was configured with the domain controller as its DNS server and joined to the `company.local` domain.

After joining the domain, users were able to authenticate using domain credentials.

Example login:

company\djeter

This confirms successful domain authentication between the client workstation and domain controller.

## Skills Demonstrated

- Active Directory deployment
- Domain controller configuration
- DNS configuration
- Organizational Unit management
- Domain user creation
- Windows client domain join
- Domain authentication troubleshooting
- Virtual network configuration

## Screenshots

Screenshots demonstrating the configuration process are available in the screenshots folder.

Examples include:

- Domain controller deployment
- Active Directory Users and Computers configuration
- Domain join process
- Successful domain login

## Key Takeaways

This lab demonstrates how centralized identity management works in enterprise IT environments.

Active Directory authentication concepts used in this lab are directly applicable to:

- Enterprise Windows environments
- AWS Directory Services
- Azure Active Directory
- Hybrid cloud identity management
