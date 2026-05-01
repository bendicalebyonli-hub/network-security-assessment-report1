 Cybersecurity Network Assessment Report
 Overview
This repository contains a professional cybersecurity assessment report based on internal network traffic analysis.
The assessment was conducted in a controlled lab environment using packet capture techniques to identify suspicious activity, potential vulnerabilities, and security misconfigurations.

Project Details
	Client: Cyber1Defense Lab (Simulated Environment)
	Analyst: Bendi Caleb YONLI
	Assessment Type: Internal Network Security Analysis
	Scope: 192.168.100.0/24

 Objectives
	Analyze network traffic using packet inspection
	Detect abnormal or malicious behavior
	Identify vulnerabilities and misconfigurations
	Provide actionable security recommendations

 Tools & Technologies
	Wireshark – Packet capture and analysis
Protocols Analyzed:
•	ARP (Address Resolution Protocol)
•	SSDP (Service Discovery Protocol)
•	mDNS (Multicast DNS)
•	DNS (Domain Name System)
•	TLS / QUIC (Encrypted Traffic)

Key Findings
High Risk
•	ARP Storming
o	Excessive ARP broadcast traffic from a single host
o	Indicates possible reconnaissance or ARP poisoning attempt
 Medium Risk
•	IoT SSDP Flooding
o	High volume of service discovery traffic from IoT device
•	External TLS/QUIC Connections
o	Encrypted outbound traffic to external services (limited visibility)
 Low Risk
•	mDNS Exposure
o	Internal service information broadcast across the network

Risk Summary
Risk Level	Description
High	Critical issue requiring immediate attention
Medium	Moderate risk with potential security impact
Low	Limited risk but useful for attacker reconnaissance

 Recommendations
•	Enable Dynamic ARP Inspection (DAI)
•	Segment IoT devices using VLANs
•	Deploy IDS/IPS monitoring systems
•	Disable unnecessary services (SSDP, mDNS)
•	Monitor outbound encrypted traffic

 Report
The full detailed report is available in this repository:
Cybersecurity_Assessment_Report.pdf

 Future Improvements
•	Include Wireshark screenshots for evidence
•	Add network traffic visualizations (charts, graphs)
•	Integrate automated threat detection tools

 Author
Bendi Caleb YONLI
Contact : +226 71782892 / 0557230269

 Note
This project demonstrates practical skills in network security analysis, traffic inspection, and SOC-style reporting within a simulated environment.

