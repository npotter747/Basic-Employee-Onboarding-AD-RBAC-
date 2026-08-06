
# Basic Employee Onboarding (AD)(RBAC)

## Problem Statement
Northstar Medical Group relied on a poorly organized Active Directory environment with inconsistent user provisioning and limited organizational structure. User accounts were created manually without standardized Organizational Units (OUs) or Role-Based Access Control (RBAC), increasing administrative overhead and the risk of improper access to sensitive resources. This lack of structure could lead to security issues, inconsistent desktop configurations, and potential HIPAA compliance concerns. The goal of this project was to rebuild the environment using Active Directory best practices and standardized user management.

## Solution Overview
A new Active Directory domain (NMG.com) was deployed and organized using department-based Organizational Units for Finance, Human Resources, IT, and Operations. Department-specific security groups were created to implement a flat Role-Based Access Control (RBAC) model, allowing permissions to be assigned through group membership rather than individual user accounts. Fifteen employee accounts were provisioned using standardized usernames, User Principal Names (UPNs), and organizational attributes. The project concluded with an incident response exercise that required diagnosing and correcting both Organizational Unit placement and security group membership to restore proper user access.

## Video Walkthrough
*Coming Soon*

A complete walkthrough of the Active Directory environment, Organizational Unit structure, RBAC implementation, and incident resolution process will be added here.

## Tools Used
* Windows Server
* Active Directory Domain Services
* VirtualBox
* UTM
* RBAC
* GitHub

## Project Timeline
* Day 1: Domain creation and domain controller promotion
* Day 2: Organizational unit and security group design
* Day 3: User provisioning and RBAC implementation
* Day 4: Incident response and resolution (NMG-0047)
* Day 5: Documentation and case study packaging

## Key Accomplishments

- Built the NMG.com Active Directory domain from scratch.
- Designed a department-based Organizational Unit (OU) structure.
- Implemented Role-Based Access Control (RBAC) using security groups.
- Provisioned 15 employee accounts with standardized naming conventions.
- Diagnosed and resolved an Active Directory access issue involving incorrect OU placement and security group membership.
- Documented the complete deployment and incident response process in GitHub.

- ## Repository Structure

Documentation/
- Domain Config File
- Security Group Doc
- User List Documentation
- RBAC-Structure.md

Incident-Reports/
- NMG-0047-Resolution.md

Screenshots/
- Day 1 infrastructure screenshots
- Day 2 OU and security group screenshots
- Day 3 user provisioning screenshots
- Day 4 incident response screenshots


