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

-   Immediate remediation after identification within a maximum of 3 calendar days.

### High criticality (CVSS-Score 7.0–8.9)

-   Remediation within a maximum of 10 calendar days.

### Medium criticality (CVSS-Score 4.0–6.9)

-   Remediation within a maximum of 30 calendar days

### Low criticality (CVSS-Score 0.1–3.9)

-   Remediation as part of regular patch cycles.

### Handling of Deadline Exceedances

-   In case of exceeding the risk thresholds/deadlines, these must be documented simultaneously and approved by the management board

## References

-   MITRE - CVEs: [https://cve.mitre.org/](https://cve.mitre.org/)
-   NIST - National Vulnerability Database: [https://nvd.nist.gov/](https://nvd.nist.gov/)
-   BSI - Cyber Security Warnings: [https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Cyber-Sicherheitslage/Technische-Sicherheitshinweise-und-Warnungen/Cyber-Sicherheitswarnungen/cyber-sicherheitswarnungen_node.html](https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Cyber-Sicherheitslage/Technische-Sicherheitshinweise-und-Warnungen/Cyber-Sicherheitswarnungen/cyber-sicherheitswarnungen_node.html)
