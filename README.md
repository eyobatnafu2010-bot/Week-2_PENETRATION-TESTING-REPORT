# Week-2_PENETRATION-TESTING-REPORT
[11/13/2026 10:36 PM] Mia cara: Cybersecurity & Ethical Hacking – Week 2 Practical Lab

Introduction

This repository documents my practical learning activities during Week 2 of my Cybersecurity & Ethical Hacking internship.

The main focus of this week's exercises was understanding how cybersecurity professionals perform information gathering, investigate web technologies, enumerate DNS records, and identify active devices within a network.

I worked with several reconnaissance and network discovery tools in Kali Linux and Windows to gain practical experience with commonly used cybersecurity techniques.

1. Footprinting and Information Gathering

Footprinting is an important part of the reconnaissance phase of ethical hacking. It involves collecting information about a target's domain, website, and digital infrastructure to better understand its publicly accessible resources.

During this activity, I explored the following tools:

1.1 WhatWeb

Purpose: Web technology fingerprinting.

Command:

whatweb 

WhatWeb helps identify technologies used by websites, including:

- Web servers.
- Content Management Systems.
- Programming frameworks.
- JavaScript libraries.
- Website technologies and components.

1.2 WHOIS

Purpose: Domain registration information gathering.

Command:

whois 

WHOIS provides publicly available information about domain registration, such as:

- Domain registrar.
- Registration and expiration dates.
- Name servers.
- Domain status.
- Available registrant details.

1.3 Nslookup

Purpose: Domain Name System investigation.

Command:

nslookup 

Nslookup allows users to investigate DNS resolution and retrieve information about domain names.

It can help identify:

- IP addresses associated with domain names.
- DNS servers.
- Mail exchange records.
- Other DNS-related information.

1.4 Wafw00f

Purpose: Web Application Firewall detection.

Command:
wafw00f https

Wafw00f helps determine whether a website is protected by a Web Application Firewall.

It can identify:

- Whether a WAF is detected.
- The possible WAF provider.
- Security filtering mechanisms protecting web applications.

1.5 DNSRecon

Purpose: DNS enumeration and infrastructure investigation.

Command:

dnsrecon -d 

DNSRecon performs DNS enumeration to gather information about a domain's infrastructure.

Information that may be discovered includes:

- DNS records.
- Name servers.
- Mail servers.
- Hostname information.
- Other publicly accessible DNS details.

1.6 Curl – HTTP Header Inspection

Purpose: Examining HTTP response headers.

Command:

curl -I 

Curl is a command-line tool used to communicate with web servers and retrieve information.

Using the "-I" option, I inspected HTTP response headers to understand:

- HTTP status codes.
- Server information when disclosed.
- Content type.
- Response metadata.
- Security-related HTTP headers.

2. Network Discovery and Scanning

The second part of the practical exercise focused on network reconnaissance using Nmap and Zenmap.

Nmap is a network exploration and security auditing tool, while Zenmap provides a graphical interface for working with Nmap.

Practical activities

During this exercise, I performed the following tasks:

1. Examined network configuration using Windows Command Prompt.
2. Identified the active Wi-Fi network adapter.
3. Retrieved local IP addressing information.
4. Examined physical (MAC) addresses.
5. Tested network connectivity using ICMP ping requests.
6. Performed host discovery using Nmap.
7. Scanned a local subnet to identify responsive hosts.
8. Used Zenmap to visualize and interpret network scanning results.

Commands and Techniques

A. Network Configuration

ipconfig /all

Used to inspect network adapters, IPv4 addresses, subnet masks, default gateways, and physical addresses.

B. Connectivity Testing

ping 127.0.0.1

Used to test communication with the local loopback interface.

C. Individual Host Discovery

nmap -sn 

Used to determine whether a specific target responds to Nmap's host discovery probes.
[11/13/2026 10:36 PM] Mia cara: D. Subnet Host Discovery

nmap -sn NETWORK_ADDRESS/24

Used to discover responsive hosts within a specified subnet without performing a port scan.

E. Zenmap Graphical Scanning

I used Zenmap to configure scans, execute host discovery, and examine the resulting network information through its graphical interface.

Note: Replace the example domain names, target IPs, and subnet notation with the appropriate authorized lab targets.

3. Understanding the Results

One of the practical outcomes of this exercise was successfully scanning a local subnet containing 256 IP addresses.

Nmap identified three responsive hosts during the scan.

This demonstrated how network scanning can help identify devices that respond to host discovery probes and provide an initial understanding of the devices present within a network.

I also learned that a host may be online without responding to particular discovery probes because of firewall rules, network restrictions, or device isolation.

4. Skills and Knowledge Gained

The practical exercises strengthened my understanding of:

- Footprinting and reconnaissance.
- Domain information gathering.
- DNS resolution and enumeration.
- Website technology identification.
- Web Application Firewall detection.
- HTTP response header analysis.
- IPv4 addressing and subnetting concepts.
- MAC address identification.
- Network connectivity testing.
- Host discovery and network scanning.
- Nmap and Zenmap usage.
- Basic technical troubleshooting and documentation.

5. Conclusion

This week's activities helped me connect theoretical cybersecurity concepts with practical tool usage.

By working with reconnaissance tools and network scanning techniques, I gained a better understanding of how security professionals collect information, examine web infrastructure, and discover active hosts within a network.

The exercises also reinforced the importance of interpreting technical results rather than simply executing commands. Understanding what the output represents is essential when conducting security assessments.

I look forward to building on these foundations and exploring more advanced cybersecurity concepts in the upcoming practical sessions.

Tools and Technologies

Category| Tools
Operating System| Kali Linux
Domain Investigation| WHOIS, Nslookup
Web Fingerprinting| WhatWeb
WAF Detection| Wafw00f
DNS Enumeration| DNSRecon
HTTP Inspection| Curl
Network Scanning| Nmap
Graphical Interface| Zenmap
Network Configuration| Windows Command Prompt

Ethical Considerations

All activities were performed for educational purposes within an authorized cybersecurity learning environment. Reconnaissance and network scanning should only be conducted against systems and networks for which permission has been granted.
