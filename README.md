# DNS and ICMP Network Traffic Analysis

## Overview
This project documents a cybersecurity incident analysis involving DNS resolution failures and ICMP error messages. The investigation was conducted using the tcpdump network protocol analyzer.

## Incident Summary
Customers reported being unable to access the website www.yummyrecipesforme.com and received a "destination port unreachable" error. Analysis of captured network traffic revealed repeated DNS query failures.

## Protocols Involved
- DNS – Domain name resolution service
- UDP – Transport protocol used for DNS queries
- ICMP – Error reporting protocol

## Key Findings
- DNS queries were sent over UDP to port 53.
- The DNS server responded with ICMP messages stating "udp port 53 unreachable."
- The repeated errors indicate the DNS service was unavailable or blocked.

## Likely Root Cause
The DNS service was not responding due to a misconfiguration, service outage, or firewall rule blocking UDP port 53.

## Skills Demonstrated
- Network traffic analysis
- DNS troubleshooting
- tcpdump usage
- Incident documentation
- Protocol-level reasoning

## Artifact
- **Incident Report:** `Cybersecurity-incident-report-network-traffic-analysis.docx`
