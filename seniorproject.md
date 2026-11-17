[Back to Portfolio](./)

# HTS Zero Trust Architecture

- **Class:** CSCI 497, CSCI 498, CSCI 499
- **Project:** Zero Trust Security Architecture for a Small Enterprise
- **Focus:** Cybersecurity, Network Security, Identity and Access Management
- **Technologies:** Windows Server 2019, Windows 11 Pro, Ubuntu Server 24.04, Active Directory, Group Policy, PowerShell, Windows Defender Firewall, OpenVPN, Oracle VirtualBox
- **Source Code Repository:** [HTS Zero Trust Capstone](https://github.com/hughesevan/CSCI-497-498-499-Zero-Trust-Capstone)

## Project Description

The HTS Zero Trust Architecture is a senior capstone project developed for CSCI 497, 498, and 499. The project focuses on designing, implementing, and testing a Zero Trust security architecture for a simulated small enterprise environment.

Inside of the fictional organization, Hughes Technology Solutions (HTS), serves as the foundation for the project. The objective is to demonstrate how an organization can strengthen its security posture by applying Zero Trust principles, including identity verification, least-privilege access, role-based access control, and centralized security monitoring.

The environment consists of Windows Server 2019, a Windows 11 Pro domain workstation, and an Ubuntu Server 24.04 system. Oracle VirtualBox provides the virtualized client environment, while OpenVPN supports connectivity to the lab infrastructure.

Rather than relying solely on traditional perimeter security, the project emphasizes controlling access based on user identity, assigned permissions, and security policies.

## System Architecture

The project uses multiple operating systems and security technologies to simulate an enterprise network.

### Windows Server 2019

Windows Server provides the central identity and domain management infrastructure.

Active Directory Domain Services and DNS support domain authentication, user management, and organizational security policies.

The environment includes departmental security groups and separate standard and administrative accounts to support role-based access control and least-privilege access.

### Windows 11 Pro Workstation

The Windows 11 workstation, named `HTS-WKS01`, serves as the domain-connected client.

It is used to test authentication, user permissions, administrative restrictions, and endpoint security policies.

The workstation was deployed using Oracle VirtualBox and configured to interact with the enterprise domain environment.

### Ubuntu Server 24.04

An Ubuntu Server system provides an additional Linux-based resource within the environment.

The server is accessed through SSH over the lab's OpenVPN connection and is used to support cross-platform security and access-control testing.

## Security Features and Implementation

### Identity and Access Management

Active Directory is used to centrally manage user identities and authentication.

Department-specific security groups allow permissions to be assigned according to organizational roles. Separate administrative accounts help reduce unnecessary privileged access.

### Role-Based Access Control

The environment implements access restrictions based on user group membership.

Department-specific file permissions demonstrate how organizations can prevent unauthorized users from accessing resources outside their assigned responsibilities.

### Least-Privilege Security

Users are assigned permissions appropriate to their responsibilities rather than receiving unrestricted administrative access.

This approach reduces the potential impact of compromised accounts and limits unnecessary access to sensitive resources.

### Endpoint and Network Security

Windows security policies and firewall controls are used to restrict access and reduce opportunities for unauthorized communication.

The project includes controls and testing related to SSH access restrictions, default-deny behavior, and limiting lateral movement.

### Centralized Security Logging

Windows security auditing and event logging are used to record authentication activity and administrative events.

The project also incorporates centralized event collection through Windows Event Forwarding to support security monitoring and investigation.

## Testing and Validation

The project includes a structured security testing plan based on its documented functional and performance requirements.

Testing focuses on verifying that security controls behave as intended, including:

- Domain authentication and account access
- Department-based permissions
- Administrative privilege restrictions
- Unauthorized access attempts
- Endpoint communication restrictions
- Security event logging
- System responsiveness and authentication performance

Testing evidence includes screenshots, PowerShell command output, Windows Event Viewer records, access-denied messages, and timing measurements.

The testing approach emphasizes validating the behavior of individual security controls within a controlled laboratory environment.

## Additional Considerations

This project provided practical experience with enterprise cybersecurity technologies and security architecture design.

The capstone also required troubleshooting across Windows and Linux systems, documenting technical decisions, validating security requirements, and evaluating the effectiveness of implemented controls.

[Back to Portfolio](./)
