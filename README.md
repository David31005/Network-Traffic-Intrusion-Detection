Network Traffic Intrusion Detection

Project Overview

This cybersecurity portfolio project demonstrates how Python can be used to analyze simulated network traffic, identify suspicious connection patterns, and generate a security incident report.

The project simulates a basic network intrusion detection workflow commonly associated with Security Operations Center (SOC) investigations.

Project Objectives

* Analyze network traffic using Python.
* Identify source IP addresses and destination ports.
* Detect potential port scanning behavior.
* Generate security alerts based on predefined detection thresholds.
* Document suspicious activity in an incident report.
* Recommend appropriate investigation and response actions.

Tools and Technologies

* Python — Security analysis and detection logic
* Pandas — Network traffic data processing
* Google Colab — Python development and testing
* GitHub — Source code management and project documentation
* Network Protocols — TCP/IP traffic analysis

Detection Methodology

The Python script analyzes a simulated network traffic dataset containing source IP addresses, destination ports, and protocols.

The detection process:

1. Groups network connections by source IP address.
2. Counts the number of unique destination ports accessed.
3. Flags IP addresses accessing four or more unique destination ports.
4. Generates alerts for potential port scanning activity.
5. Identifies traffic that does not exceed the detection threshold.

This is a basic threshold-based detection method intended for educational purposes.

Security Investigation Results

The simulated dataset identified the following suspicious activity:

Source IP Address: 10.0.0.5

Unique Destination Ports: 4

Ports Accessed:

* 21 — FTP
* 22 — SSH
* 23 — Telnet
* 3389 — Remote Desktop Protocol (RDP)

Detection Result: Potential port scanning activity

Severity: Medium (Simulated)

Investigation Status: Requires Further Investigation

The source IP triggered the detection rule because it accessed four distinct destination ports.

This pattern may indicate reconnaissance activity, although additional evidence would be required to determine whether the behavior was malicious.

Security Incident Response Recommendations

1. Review firewall and network connection logs.
2. Investigate the source IP address.
3. Examine destination systems for suspicious authentication activity.
4. Review endpoint security alerts.
5. Correlate network events with additional security telemetry.
6. Apply appropriate network restrictions if malicious activity is confirmed.
7. Document findings and remediation actions.

Project Files

Network_Traffic_Analysis.ipynb

Google Colab notebook containing the simulated network traffic dataset, Python analysis, and port scanning detection logic.

incident_report 3.txt

Security incident report documenting the simulated detection results, suspicious IP address, affected ports, and recommended investigation steps.

README.md

Project documentation describing the objectives, tools, detection methodology, and investigation findings.

Skills Demonstrated

* Network Traffic Analysis
* Python Security Automation
* Basic Intrusion Detection
* Port Scanning Identification
* Security Event Analysis
* Incident Documentation
* SOC Investigation Fundamentals
* Threat Detection Logic

Limitations

This project uses simulated network traffic rather than live packet captures.

The detection rule is based on a simple threshold of four unique destination ports. This can generate false positives and does not independently confirm an intrusion.

Future improvements could include timestamp analysis, connection frequency, baseline comparisons, and integration with SIEM tools.

Author

David Jeffries

Cybersecurity Professional Certificate — Google (Completed)

Cybersecurity Portfolio: GitHub

LinkedIn: David Jeffries

⸻

This project was developed to demonstrate foundational cybersecurity monitoring, threat detection, and incident response skills.
