# Guideline Vulnerability and Patch Management

**Version:** 2.0.1

## Introduction

This guideline describes the processes for remediating information security vulnerabilities and implementing security fixes for services and devices connected to the organization.

## Importance

-   Vulnerability assessments identify system vulnerabilities before malicious actors by thoroughly examining all network components to determine if any weaknesses exist that could be exploited.
-   Regular vulnerability scanning helps maintain regulatory compliance.
-   These assessments are also necessary to obtain and retain security certifications such as ISO 27001.
-   By proactively identifying and addressing vulnerabilities, organizations can prevent costly data breaches and avoid the potential financial consequences of litigation.

## Scope

This policy applies to all information systems and resources of EKiR, whether they are owned or operated by the organization or on its behalf. All individuals associated with EKiR who have access to organization information or to computers and systems managed or maintained on behalf of EKiR must adhere to this policy.

## Responsibilities

-   **Chief Information Officer:** Has the responsibility for enforcing EKiR's software update and patching strategy.
-   **IT Services Manager:** Is responsible for ensuring that all relevant software is kept up-to-date and patched regularly.
-   **System Owners:** Are accountable for making sure all software under their jurisdiction is kept up-to-date and patched regularly.
-   **IT Department:** Is responsible for ensuring that all relevant software is kept up-to-date and patched on a regular basis.

## Software Updates and Patching

-   All IT systems, whether owned by EKiR or managed by third-party vendors, must have proper licensing, vendor support, and updated and patched operating systems and application software.
-   Before using an IT system, third-party vendors must provide evidence of current patching.
-   Patches must be thoroughly reviewed before full implementation, as changes may cause unexpected issues.
-   IT systems that have been disconnected from the network due to missing patches will not be reactivated until it can be confirmed that they have been patched and no longer pose a risk to EKiR.

## Software That Is No Longer Supported (EOL)

-   Operating systems and application programs for which the manufacturer has discontinued support and which can no longer be updated (end-of-life / end-of-support) must be replaced after 90 days at the latest or the corresponding devices must be isolated from the network (at least logically).

## Vulnerability Scanning

-   The organization will use a vulnerability scanner to search for any weaknesses and missing patches on its IT systems.
-   The network of the organization will undergo scanning regularly. Depending on the specific risk, this can be done several times a year or continuously.
-   The vendors of servers, PCs, tablets, printers, switches, routers, and peripherals will be checked for firmware patch availability.
-   Any missing patches discovered through the vulnerability scanning will be promptly installed, and any vulnerabilities found will be promptly addressed.

## Vulnerability Classification

-   To protect the organization's IT systems from known vulnerabilities, security updates must be applied promptly.
-   Patches should be deployed as per the schedule below, unless the organization prohibits it.
-   Vulnerabilities are those that have been identified or classified as such by the BSI (Federal Office for Information Security) or the CVSS (Common Vulnerability Scoring System).

### Very high criticality (CVSS-Score ≥ 9.0)

| Criterion | Remediation Deadline | Escalation | Examples |
|-----------|---|---|---|
| **Internet-Accessible** (DMZ, Cloud, Remote Access) | **3 Days** | Management + Security Team, daily status | Pre-auth RCE, active exploits, CISA-KEV |
| **Internal, but Core Infrastructure** (AD, Email, File-Server, Firewall) | **5 Days** | Management, daily status | Domain Admin takeover, critical data exposure |
| **Internal, Standard System** (Desktop PC, Printer, configurable) | **7 Days** | Team Lead, daily status | Local privilege escalation, DoS |
| **Legacy/EOL Systems** (no patch available) | **3 Days** (Workaround/Mitigation) | CISO decision | Must be isolated or decommissioned |

**Escalation Triggers:** If deadline is missed:
- Day 1 after deadline: Email to system owner + manager
- Day 2: Escalation to department head
- Day 3: CISO involvement + management report
- Day 5: Automatic quarantine/shutdown (with approval)

### High criticality (CVSS-Score 7.0–8.9)

| Criterion | Remediation Deadline | Escalation | Examples |
|-----------|---|---|---|
| **Internet-Accessible** | **14 Days** | Weekly Status Report | RCE with authentication, critical data leak |
| **Internal, Core Infrastructure** | **21 Days** | Bi-weekly Review | Admin account risk, SMB/RDP exploitation |
| **Internal, Standard System** | **30 Days** | Monthly Review | Kernel exploit, malware vector |
| **Legacy/EOL Systems** | **14 Days** (Workaround/Isolation) | CISO decision | Compensating controls required |

**Escalation Triggers:** Similar to CRITICAL (Day 1, 2, 3, 5 after deadline)

### Medium criticality (CVSS-Score 4.0–6.9)

| Criterion | Remediation Deadline | Escalation | Examples |
|-----------|---|---|---|
| **Internet-Accessible** | **60 Days** | Quarterly Report | XSS, SQLi without direct data access |
| **Internal, Core Infrastructure** | **90 Days** | Quarterly Review | Denial of Service, unencrypted services |
| **Internal, Standard System** | **120 Days** | Quarterly Review | Information Disclosure (non-critical) |
| **Legacy/EOL Systems** | **60 Days** (Evaluation for Replacement) | Quarterly Review | Increase priority for EOL planning |

### Low criticality (CVSS-Score 0.1–3.9)

| Criterion | Remediation Deadline | Escalation | Examples |
|-----------|---|---|---|
| **All System Types** | **180 Days** (6 months) | Annual Audit | Best practice deviations, info-disclosure |
| **Legacy/EOL Systems** | **180 Days** (or with EOL planning) | Annual Audit | Not security-critical |
-   Remediation as part of regular patch cycles.

### Handling of Deadline Exceedances

-   In case of exceeding the risk thresholds/deadlines, these must be documented simultaneously and approved by the management board

## References

-   MITRE - CVEs: [https://cve.mitre.org/](https://cve.mitre.org/)
-   NIST - National Vulnerability Database: [https://nvd.nist.gov/](https://nvd.nist.gov/)
-   BSI - Cyber Security Warnings: [https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Cyber-Sicherheitslage/Technische-Sicherheitshinweise-und-Warnungen/Cyber-Sicherheitswarnungen/cyber-sicherheitswarnungen_node.html](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Cyber-Sicherheitslage/Technische-Sicherheitshinweise-und-Warnungen/Cyber-Sicherheitswarnungen/cyber-sicherheitswarnungen_node.html)
