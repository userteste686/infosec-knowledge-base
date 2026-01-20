## Pivoting

Pivoting is a technique used in Information Security and penetration testing in which a compromised system—typically located inside a target network—is leveraged as an intermediary point to access other systems or subnets that are not directly reachable from the attacker’s original position.

By using the compromised host as a “pivot,” an attacker can redirect traffic, establish tunnels, or create new network routes that allow access to restricted internal networks. This technique exploits trust relationships and network connectivity between systems within segmented environments.

Pivoting is commonly implemented by configuring routing rules or tunnels through the compromised machine, which forwards the attacker’s traffic into internal or protected networks. Tools such as SSH, Metasploit, proxy frameworks, and tunneling utilities are frequently used to enable this redirection.

---

## How Pivoting Works
The pivoting process typically follows these steps:

1. Initial compromise of a system with network access to internal segments  
2. Enumeration of reachable networks and hosts from the compromised system  
3. Establishment of a tunnel, proxy, or route through the pivot host  
4. Access to internal systems as if the attacker were inside the network  

The compromised system effectively becomes an extension of the attacker’s infrastructure within the target environment.

---

## Practical Examples

### SSH Tunneling
An attacker uses SSH port forwarding on a compromised Linux server to access an internal database server that is not exposed externally.

### Metasploit Pivoting
After gaining a Meterpreter session, the attacker adds routes to internal subnets and launches further exploits against internal hosts.

### Proxy-Based Pivoting
A compromised system is configured as a SOCKS proxy, allowing scanning and exploitation of internal assets using tools such as Nmap or web browsers.

---

## Why Pivoting Is Effective
Pivoting is effective because it bypasses network segmentation controls such as:
- Firewalls
- VLANs
- Access Control Lists (ACLs)
- NAT boundaries

These controls often trust internal systems more than external ones, allowing a compromised internal host to communicate freely with other internal assets.

---

## Use Cases

### Penetration Testing
In pentesting, pivoting is essential for simulating advanced attacks and uncovering vulnerabilities that exist only within internal network segments. It allows testers to evaluate the effectiveness of segmentation, monitoring, and lateral movement detection.

### Malicious Attacks
In real-world attacks, pivoting is a core technique for lateral movement within corporate networks. Attackers use it to gradually expand their access, reach critical systems, and maintain stealth by avoiding direct exposure.

---

## Security Impact
Successful pivoting can lead to:
- Lateral movement across the network
- Compromise of critical systems
- Escalation of privileges
- Data exfiltration from internal assets
- Extended attacker persistence

Because pivoting often leverages legitimate internal communication paths, it may bypass traditional perimeter-based defenses.

---

## Detection and Mitigation

### Detection
- Monitoring unusual internal traffic patterns
- Detecting new or unexpected routes
- Analyzing lateral movement behaviors
- Correlating EDR and network telemetry
- Monitoring tunneling or proxy activity

### Mitigation
- Strong network segmentation and zero trust principles
- Restricting lateral communication by default
- Endpoint hardening and least privilege
- Continuous internal traffic monitoring
- Rapid isolation of compromised hosts

---

## Why Pivoting Exists
Pivoting was developed to operate in complex, segmented environments where direct access to all systems is not possible. Without pivoting, many internal network vulnerabilities would remain inaccessible—both to attackers and defenders.

Understanding pivoting is essential for both offensive and defensive security professionals, as it directly relates to lateral movement, network architecture weaknesses, and detection strategy effectiveness.
