## Active Directory (AD)

Active Directory (AD) is a directory service and a set of management tools developed by Microsoft and integrated into the Windows Server operating system. It functions as a centralized database that stores and manages information about all resources within a corporate network, such as users, computers, servers, printers, groups, and services.

In essence, Active Directory acts as the “brain” of a Windows-based enterprise network. It controls authentication, authorization, and the enforcement of security policies in a centralized and scalable manner. AD enables administrators to manage identities and access consistently across the entire environment.

Active Directory primarily uses the LDAP (Lightweight Directory Access Protocol) to query and manage directory objects, and Kerberos as its default authentication protocol to provide secure, ticket-based authentication.

---

## Core Functions of Active Directory

### Centralized Authentication
Users authenticate once at logon and can access all authorized resources without re-entering credentials, a concept known as Single Sign-On (SSO).

### Authorization and Access Control
AD determines what resources a user or system can access, based on group membership, permissions, and security policies.

### Policy Enforcement
Through Group Policy Objects (GPOs), administrators can enforce security settings, password policies, software deployment, scripts, and system configurations across all domain-joined machines.

---

## Key Components of Active Directory

### Domain
A logical grouping of objects (users, computers, groups) that share the same directory database and security policies.

### Domain Controller (DC)
A server that hosts the Active Directory database and handles authentication, authorization, and directory services requests.

### Organizational Units (OUs)
Containers used to organize objects and apply Group Policies in a structured and manageable way.

### Forest and Tree
A forest is the highest-level structure in AD, containing one or more domains. Trees represent domain hierarchies with shared namespaces.

### Trust Relationships
Trusts allow users in one domain to access resources in another, enabling collaboration across domains or forests.

---

## Practical Examples

### Corporate User Management
An employee account is created once in AD and automatically gains access to email, file servers, VPN, and internal applications based on group membership.

### Group Policy Enforcement
Security policies such as password complexity, screen lock timeouts, firewall rules, and software installation are centrally enforced using GPOs.

### Access Control
Only members of a specific AD group are allowed to access a sensitive file server or administrative interface.

---

## Why Active Directory Is a Primary Target

Because Active Directory controls identity and access across the entire network, compromising AD often means compromising the organization itself.

If an attacker gains control over Active Directory, they can:
- Create or modify user accounts
- Escalate privileges to domain administrator
- Access or manipulate critical systems
- Disable security controls
- Maintain long-term persistence

For this reason, AD is one of the most targeted components in enterprise cyber attacks.

---

## Security Risks and Common Attack Vectors

- Credential theft (e.g., pass-the-hash, pass-the-ticket)
- Kerberoasting
- Abuse of misconfigured permissions or delegation
- Exploitation of weak service accounts
- Lateral movement via domain trusts
- Persistence through GPO or hidden accounts

---

## Detection and Defense Considerations

### Defensive Measures
- Enforce least privilege and role separation
- Harden Domain Controllers
- Monitor privileged account activity
- Implement tiered administration models
- Use strong authentication and MFA for admins

### Monitoring and Detection
- Log authentication anomalies
- Detect privilege escalation attempts
- Monitor changes to GPOs and group memberships
- Correlate AD logs with SIEM and EDR tools

---

## Why Active Directory Exists
Active Directory was created to simplify, centralize, and secure identity and access management in large-scale Windows environments. Without AD, managing users, permissions, and security policies across thousands of systems would be operationally unfeasible.

Understanding Active Directory is fundamental for both offensive and defensive security professionals, as it represents the core identity infrastructure of most enterprise networks—and a critical point of failure if not properly secured.
