# Nmap network scan report
Network vulnerability scanning with Nmap.

## Objective
This document demonstrates the use of the network scanning application Nmap for executing a detailed network evaluation procedure. The scan's purpose was to discover operational hosts, combined with the identification of active ports and services, as well as the collection of system characteristics. The combination of the following flags: -sC, -sV, -vv, -sL, -sn, and -Pn in Nmap enabled a complete investigation during the network scanning process.

## Tool used and its objective
Nmap is used to perform a detailed network scan, and its objective is to incorporate service detection, script scanning, and host discovery to gather actionable security insights.

## Tool Configuration
### Nmap Configuration: 
The Nmap tool was used with the following command-line flags:
- -sC: Run default scripts for service detection.
- -sV: Probe open ports to determine service/version info.
- -vv: Increase verbosity for detailed output.
- -sL: List targets without scanning (used for initial reconnaissance).
- -sn: Disable port scanning (used for host discovery).
- -Pn: Treat all hosts as online (skip host discovery).
### Target IP: 
The target IP address for the scan was the local: 192.168.0.100, which can be obtained using the command prompt and the syntax “ipconfig” for Windows.

## Key Findings 
The Nmap scan displayed numerous open ports along with services that delivered important security information regarding system flaws. The assessment revealed essential information about particular services along with their version identities that might aid vulnerability assessments.

## Recommendation
### Immediate Remediation Actions
 Conduct an instant assessment of all active services on ports 135, 139, 445, 902, 912, and 8089 to evaluate their necessity.
- Deactivate any non-essential services identified during the review.
- Implement and enhance firewall policies to create restrictive filters for the specified ports.
- Enforce robust password policies for all accounts accessing SMB and disallow guest user access to SMB file shares.
- Utilize SMB signing technology for business-critical operations to safeguard data from unauthorized modifications.
### Long-Term Mitigation
- Network Segmentation
- Principle of Least Privilege
- Regular Vulnerability Scanning
- Security awareness training
- Endpoint Detection and Response (EDR)
- Zero Trust security models

[Full Report on Medium](https://medium.com/@folajayeabdulrahman/how-i-used-nmap-to-scan-my-network-for-hidden-risks-fe50a0728614)













