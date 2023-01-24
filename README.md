# dealing_vulnerabilities

Version: 0.2

## introduction
the ekir vulnerability and patch management policy is defined in this document. This policy describes the procedures for managing information security vulnerabilities and for notifying, testing, and deploying security-related fixes to services and devices connected to the organization.

## importance
vulnerability assessment identifies system vulnerabilities before hackers notice them by examining all network components to see if they have weaknesses that cybercriminals could exploit to attack the organization.
- careful vulnerability scanning can help ensure regulatory compliance.
- vulnerability assessment is also required to obtain and maintain security certifications such as ISO 27001.
- vulnerability scanning prevents data breaches that result in expensive litigation for an organization.

## scope
this policy applies to all the EKiR information systems and resources, whether they are owned or operated by the ekir or on its behalf. this policy must be followed by all ekir-related persons who have access to organization information or computers and systems that are managed or maintained on behalf of the EKiR.

## responsibilities
- The Chief Information Officer oversees enforcing the EKIR software update and patching strategy.
- The IT Services Manager oversees ensuring that in-scope software is kept up to date and patched on a regular basis.
- System owners are responsible for ensuring that all in scope software they manage is kept up to date and patched on a regular basis.
- The IT department oversees ensuring that all in-scope software is kept up to date and patched on a regular basis.

# Software updates, patching
All IT systems, whether owned by EKiR or developed and maintained by third parties, 
- must be appropriately licensed, supported by the vendor, and have current and patched operating systems and application software.
- Prior to commissioning an IT system, third-party vendors must provide proof of a current patch level.
- Patches must be thoroughly reviewed before they are fully implemented, as changes can cause unexpected problems.
- IT- systems that have been disconnected from the network due to missing patches will not be put back into operation until it can be proven that they have been patched and no longer pose a risk to EKiR.

## vulnerability classification
- security updates must be applied in a timely manner to safeguard the organization's it-systems from known vulnerabilities.
- Patches should be deployed according to the schedule below unless the firm prevents it.

### high severity level
- High severity CVEs are those with a documented CVSS severity greater than 7.0
- It is a best practice in standards such as PCI DSS to remediate or patch high severity vulnerabilities within 45 days. 
### medium severity level
- Medium severity CVEs are those with a documented CVSS severity between 4.0 and 6.9
- It is a best practice to remediate or patch medium severity vulnerabilities within 90 days. 
### low severity level
- Low severity CVEs are those with a documented CVSS severity below 4.0
- It is a best practice to remediate or patch low severity vulnerabilities within 120 days. 

## vulnerability scanning
- A vulnerability scanner will be used to scan all items on the organization's it-systems to find flaws in system setup and to see if any systems are missing crucial patches or applications.
- The network of the organization will be inspected at least once a quarter.
- To determine the availability of firmware patches, the websites of vendors of servers, PCs, tablets, printers, switches, routers, and peripherals will be examined.
- Missing fixes discovered during vulnerability scanning will be applied as soon as possible. Any flaws discovered will be addressed.

## references
- MITRE - CVEs (https://cve.mitre.org/)
- NIST - National Vulnerability Database (https://nvd.nist.gov/)
