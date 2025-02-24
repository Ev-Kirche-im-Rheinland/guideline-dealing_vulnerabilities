# guideline vulnerability and patch management

Version: 2.0.0

## introduction
This guideline describes the processes for remediating information security vulnerabilities and implementing security fixes for services and devices connected to the organization.

## importance:
- vulnerability assessments identify system vulnerabilities before malicious actors by thoroughly examining all network components to determine if any weaknesses exist that could be exploited.
- regular vulnerability scanning helps maintain regulatory compliance.
- these assessments are also necessary to obtain and retain security certifications such as ISO 27001.
- by proactively identifying and addressing vulnerabilities, organizations can prevent costly data breaches and avoid the potential financial consequences of litigation.

## scope:
- this policy applies to all information systems and resources of EKiR, whether they are owned or operated by the organization or on its behalf. All individuals associated with EKiR who have access to organization information or to computers and systems managed or maintained on behalf of EKiR must adhere to this policy.

## responsibilities:
- the Chief Information Officer has the responsibility for enforcing EKiR's software update and patching strategy.
- the it services manager is responsible for ensuring that all relevant software is kept up-to-date and patched regularly.
- system owners are accountable for making sure all software under their jurisdiction is kept up-to-date and patched regularly.
- the IT department is responsible for ensuring that all relevant software is kept up-to-date and patched on a regular basis.

# software updates and patching:
- all IT systems, whether owned by EKiR or managed by third-party vendors, must have proper licensing, vendor support, and updated and patched operating systems and application software.
- before using an IT system, third-party vendors must provide evidence of current patching.
- patches must be thoroughly reviewed before full implementation, as changes may cause unexpected issues.
- it-systems that have been disconnected from the network due to missing patches will not be reactivated until it can be confirmed that they have been patched and no longer pose a risk to EKiR.

# software that is no longer supported (eol)
- Operating systems and application programs for which the manufacturer has discontinued support and which can no longer be updated (end-of-life / end-of-support) must be replaced after 90 days at the latest or the corresponding devices must be isolated from the network (at least logically).

## vulnerability scanning
- the organization will use a vulnerability scanner to search for any weaknesses and missing patches on its IT systems.
- the network of the organization will undergo scanning regulary. depending on the specific risk, this can be done several times a year or continuously
- the vendors of servers, PCs, tablets, printers, switches, routers, and peripherals will be checked for firmware patch availability.
- any missing patches discovered through the vulnerability scanning will be promptly installed, and any vulnerabilities found will be promptly addressed.

## vulnerability classification:
- to protect the organization's IT systems from known vulnerabilities, security updates must be applied promptly.
- patches should be deployed as per the schedule below, unless the organization prohibits it.
- vulnerabilities are those that have been identified or classified as such by the bsi (federal office for information security) or the cvss (common vulnerability scoring system).

### high severity level
- High severity CVEs are those with a documented CVSS severity greater than 8.0
- High severity vulnerabilities must be eliminated promptly, but no later than 10 working days after the publication of a security update relevant to this vulnerability.
### medium severity level
- Medium severity CVEs are those with a documented CVSS severity between 4.0 and 7.9
- It is a best practice to remediate or patch medium severity vulnerabilities within 60 days. 
### low severity level
- Low severity CVEs are those with a documented CVSS severity below 4.0
- It is a best practice to remediate or patch low severity vulnerabilities within 120 days. 

## references
- MITRE - CVEs (https://cve.mitre.org/)
- NIST - National Vulnerability Database (https://nvd.nist.gov/)
- BSI - Cyber Security Warnings (https://www.bsi.bund.de/EN/Themen/Unternehmen-und-Organisationen/Cyber-Sicherheitslage/Technische-Sicherheitshinweise-und-Warnungen/Cyber-Sicherheitswarnungen/cyber-sicherheitswarnungen_node.html)
