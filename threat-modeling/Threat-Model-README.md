**Michael Sherman | UMGC Cybersecurity Coursework | Academic Design Project**

A threat model for TRex Smart Everything (TRex SE), a fictional Azure-hosted SaaS platform supporting home, business, and medical smart devices. The project examines how architecture, identity, dataflows, and operational practices can affect the confidentiality, integrity, and availability of sensitive information.

## Project Report

[View the Threat Model](ShermanM-Project-ThreatModel.pdf)

## Scenario

The supplied scenario describes devices collecting personal, health, payment, and device information. The platform includes application and management planes, Azure networking and services, Active Directory, Okta MFA, and Splunk logging. Customers, administrators, devices, and external services exchange information across the environment.

## My Work

- Used Threat Composer to document the model and relationships between its components.
- Examined the scenario's architecture and dataflows to identify potential attack paths.
- Recorded assumptions about identity controls, network access, updates, logging, and recovery.
- Developed threat statements covering external attackers, internal actors, and operational weaknesses.
- Assigned threat priorities and STRIDE categories.
- Linked threats to affected assets, assumptions, and proposed mitigations.

## Approach

| Element | Role in the Model |
| --- | --- |
| Architecture and dataflows | Establish system context and information movement |
| Assumptions | Make dependencies and expected controls explicit |
| Threat statements | Describe potential conditions, actions, and impacts |
| STRIDE | Organize threats by security concern |
| Assets | Identify the information and capabilities potentially affected |
| Mitigations | Connect identified threats with proposed risk-reduction measures |

STRIDE covers spoofing, tampering, repudiation, information disclosure, denial of service, and elevation of privilege.

## Threat Themes

| Theme | Potential Risk Considered |
| --- | --- |
| Privileged access and MFA | Unauthorized identity configuration changes or bypass of access controls |
| Authentication attempts | Brute-force access where protective controls are insufficient |
| Firewall configuration and routing | Unprotected paths into application infrastructure |
| Phishing and security awareness | Exposure of credentials through social engineering |
| User access reviews | Excess permissions enabling unauthorized actions |
| Monitoring maintenance | Security events missed because monitoring capabilities are not maintained |
| Backup and recovery | Data loss or service disruption without effective recovery arrangements |

## Proposed Controls

The model considers MFA, security awareness training, phishing simulations, firewall rules, vulnerability scanning, software maintenance, and backup recovery planning. These are proposed or assumed controls in the academic model; their inclusion does not demonstrate that they were deployed or tested.

## Skills Demonstrated

Threat modeling, Azure architecture interpretation, identity and access risk analysis, STRIDE categorization, asset identification, control mapping, and structured security documentation.

## Scope and Limitations

This is a design assessment of a fictional system based on a supplied academic scenario. Architecture details describe the scenario rather than infrastructure I deployed. Threats are modeled possibilities, not verified exploits or confirmed production vulnerabilities.

Priorities and control relationships reflect the submitted coursework and should be refined through further review. Control effectiveness and residual risk were not validated through implementation testing.

## Lessons Learned

Threat modeling connects system design with practical security questions: what could go wrong, which assets would be affected, and which controls would reduce the risk? Clear assumptions and specific threat-to-control relationships make a model more useful. A control's presence in a diagram or table is only the starting point; its effectiveness requires validation.

---

*Prepared by Michael Sherman as part of UMGC cybersecurity coursework using Threat Composer and a supplied fictional system scenario.*
