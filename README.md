# Threat-Modelling
#Threat-Model using Microsoft threat model tools and OSWAP framework

Threat modeling is a structured approach used to identify, evaluate, and mitigate security risks within a system. This process helps developers and security teams understand potential threats early in the design phase and build stronger, more resilient applications. The following summarizes the four core steps of threat modeling using Data Flow Diagrams (DFDs) and the STRIDE framework.

## Using Microsoft Threat Modeling Tool (TMT)

- Microsoft TMT automates DFD creation and maps system components using a drag-and-drop interface.
- The tool automatically assigns STRIDE threats to DFD elements.
- Useful for teams using Microsoft Azure or structured architecture documentation.

## Using OWASP Threat Modeling Framework
OWASP provides a broader approach using four core questions:
- What are we building?
  Define architecture, assets, use cases, and assumptions.

- What can go wrong?
  Identify misuse cases, STRIDE threats, and attacker capabilities.

- What are we going to do about it?
  Plan mitigations and defenses.

- Did we do a good job?
  Validate the model and revisit over time.

OWASP complements STRIDE by focusing on attacker paths, business impact, and secure design principles.

## Identify Threats with STRIDE
Use the STRIDE threat classification model to assess each DFD element:

- Spoofing
- Tampering
- Repudiation
- Information Disclosure
- Denial of Service
- Elevation of Privilege
Analyze how each component and data flow could be targeted under each STRIDE category.

## Mitigate Identified Threats

For each threat, define appropriate countermeasures to reduce risk:
- Authentication → prevents Spoofing
- Integrity checks / hashing → protects against Tampering
- Logging & auditing → mitigates Repudiation
- Encryption → reduces Information Disclosure
- Rate-limiting & redundancy → address Denial of Service
- Least privilege & access controls → prevent Elevation of Privilege

Prioritize mitigations based on impact and likelihood.

