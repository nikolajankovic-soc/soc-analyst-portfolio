Wireshark-fake-software-c2-analysis
This folder contains the report, screenshots, and IOCs for the Wireshark-fake-software-c2-analysis
# Wireshark Traffic Analysis – Fake Software Download Infection

## Project Overview
This project analyzes a Malware-Traffic-Analysis.net PCAP from 2025-01-22 involving a Windows client that downloaded suspicious content from a fake software site.

## Scenario
A user searched for Google Authenticator and visited a suspicious fake software-related website. Network traffic analysis was performed using Wireshark to identify the infected host, suspicious domains, possible C2 infrastructure, and indicators of compromise.

## Tools Used
- Wireshark
- tcpdump concepts
- Malware-Traffic-Analysis.net PCAP
- VirusTotal for IOC checking
- GitHub for documentation

## Key Findings
- Infected host: 10.1.17.215
- Hostname: DESKTOP-L8C5GSJ
- Username: shutchenson
- Suspicious fake software domain: authenticatoor.org
- Related suspicious domain: google-authenticator.burleson-appliance.net
- Suspicious IP / possible C2: 5.252.153.241

## Skills Demonstrated
- PCAP analysis
- DNS investigation
- HTTP traffic analysis
- TLS/SNI review
- C2/beaconing pattern identification
- IOC extraction
- GitHub documentation
