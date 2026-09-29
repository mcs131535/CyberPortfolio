# Penetration Testing and Vulnerability Assessment

**Michael Sherman | UMGC Cybersecurity Coursework | Academic Lab Project**

A documented security assessment of the fictional FIC Bank environment, completed in an authorized university lab. This project follows the assessment lifecycle from reconnaissance and service enumeration through vulnerability discovery, a simulated credential-harvesting exercise, and remediation and cleanup planning.

## Project Report

[View the Penetration Testing Plan & Report](MSherman-PenetrationTestingReport.pdf)

## My Work

- Documented reconnaissance activities using public information, DNS lookups, and network discovery.
- Used Nmap to identify responsive hosts and accessible services.
- Examined web application resources and configuration findings with DIRB, Nikto, and WPScan.
- Interpreted OpenVAS results and distinguished a scanner-environment issue from target configuration weaknesses.
- Explored Metasploit modules and payload options within the exercise scope.
- Demonstrated credential capture using a simulated login page and test credentials in the lab.
- Developed remediation recommendations and documented cleanup and recovery considerations.

## Tools and Techniques

| Tool | Purpose |
| --- | --- |
| Kali Linux | Security assessment environment |
| Nmap | Host discovery and port enumeration |
| dig, nslookup, WHOIS | DNS and domain reconnaissance |
| DIRB | Web directory and file discovery |
| Nikto | Web server configuration assessment |
| WPScan | Check for a WordPress installation |
| OpenVAS / Greenbone | Vulnerability assessment |
| Metasploit / MSFvenom | Explore modules and payload options |
| Social-Engineer Toolkit (SET) | Simulated phishing and credential harvesting |

## Key Results

| Observation | Interpretation |
| --- | --- |
| Nine responsive hosts identified in the discovery scan | Established an initial inventory for further assessment |
| Eight hosts exposed ports 80 and 443 | Identified accessible web services; open ports alone do not establish a vulnerability |
| DIRB identified directories and web resources | Expanded the application's observed attack surface |
| Nikto reported missing security headers | Identified configuration items requiring contextual review |
| WPScan did not identify WordPress | Recorded a negative result and avoided claiming WordPress vulnerabilities |
| OpenVAS reported weak TLS cipher suites and SSH MAC algorithms | Identified target cryptographic configuration weaknesses |
| OpenVAS reported an outdated local scan engine/environment | Identified an assessment limitation requiring scanner maintenance and reassessment |
| SET captured submitted test credentials | Demonstrated the impact of a simulated phishing workflow |

## Remediation Focus

The report recommends reviewing exposed services, maintaining segmentation and asset inventories, updating the scanning environment, and strengthening phishing defenses through training, phishing-resistant MFA, and email/web controls. The vulnerability analysis also identifies TLS and SSH configuration hardening as necessary follow-up work.

## Skills Demonstrated

Network reconnaissance, vulnerability triage, security tool interpretation, evidence collection, security reporting, remediation planning, and communication of technical findings.

## Scope and Limitations

This is an academic exercise using a fictional client scenario and university-provided lab systems. Public-information reconnaissance is documented separately from the lab activities. The project does not represent a production client engagement.

Reverse-shell access and privilege escalation were outside the documented scope. Metasploit exploration does not establish a successful system compromise. Remediation and recovery steps are recommendations; the report does not claim completed remediation or verified retesting.

## Lessons Learned

Useful reporting requires more than listing tool output. Findings need context, evidence, and a clear explanation of impact. Scanner health can affect assessment quality, and negative results help define what was actually observed. The simulated phishing exercise also demonstrated why technical controls and user awareness should work together.

---

*Prepared by Michael Sherman using a UMGC course-provided reporting template. Lab activities were performed for educational purposes within the assigned environment.*
