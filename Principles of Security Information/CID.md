# CIA / CID – Additional Security Concepts

## Overview
The CIA Triad (Confidentiality, Integrity, and Availability), also referred to as CID depending on the language, represents the fundamental security objectives for data, information, and computing services. Although the acronyms differ in order, they describe the same core principles that underpin Information Security.

These principles define the minimum requirements that must be preserved to ensure the protection, reliability, and operational continuity of information systems.

---

## Confidentiality
Confidentiality ensures that sensitive or private information is not disclosed or made available to unauthorized individuals. It guarantees that only authorized entities are able to access protected data.

Privacy is closely related to confidentiality and ensures that individuals can control or influence which information about them is collected, stored, and disclosed, as well as to whom such information may be revealed.

A breach of confidentiality may result in information leakage, unauthorized exposure of data, or incorrect system behavior. For example, improperly modified or exposed data values may cause systems to operate incorrectly or produce inaccurate results.

---

## Integrity
Integrity ensures that data and systems are accurate, complete, and trustworthy.

- **Data Integrity** guarantees that information and programs are modified only in authorized and approved ways, preventing unauthorized alteration or corruption.
- **System Integrity** ensures that a system performs its intended functions without unauthorized manipulation, whether intentional or accidental.

A failure of integrity may lead to data tampering, fraud, incorrect processing, or loss of trust in systems and services.

---

## Availability
Availability ensures that systems and services remain accessible and functional for authorized users when needed. This includes protection against service disruptions, performance degradation, and denial-of-service conditions.

A vulnerability affecting availability may cause systems or network resources to become unavailable or excessively slow, making their use impossible or impractical for legitimate users.

---

## Importance of the CIA / CID Triad
The CIA/CID Triad is the foundation of all information security decisions. Every security control, policy, or tool exists to preserve one or more of these principles.

- If **Confidentiality** fails, data breaches and information leakage occur.
- If **Integrity** fails, data becomes corrupted or manipulated.
- If **Availability** fails, services are disrupted or rendered inaccessible.

For this reason, security professionals must understand and apply the CIA/CID Triad as a central reference when designing, implementing, and operating secure systems, networks, and services.

---

## Additional Security Concepts
While the CIA/CID Triad is well established, some security models extend it with additional principles to provide a more comprehensive view of security.

---

## Authenticity
Authenticity refers to the assurance that an entity, message, or data source is genuine, verifiable, and trustworthy. It provides confidence in the validity of communications, messages, and their origin.

In practice, authenticity ensures that:
- Users are who they claim to be
- Data originates from trusted and verified sources
- Communications have not been forged or impersonated

---

## Accountability
Accountability ensures that the actions of an entity can be traced and uniquely attributed to that entity. This principle supports non-repudiation, deterrence, fault isolation, intrusion detection and prevention, and post-incident recovery and legal actions.

Because perfectly secure systems are not realistically achievable, it must be possible to trace security violations back to the responsible entity. Systems must maintain logs and activity records to enable forensic analysis, allowing organizations to investigate incidents, trace breaches, and resolve disputes related to transactions or system usage.
