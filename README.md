# Cybersecurity Homelab Security Lab

## Overview

This project documents my cybersecurity homelab environment built for hands-on learning, security monitoring, detection engineering, network defense, Active Directory administration, and penetration testing.

The lab simulates a small enterprise environment and includes a firewall, Active Directory domain controller, SIEM platform, vulnerable web application, attack workstation, and secure remote access through VPN.

## Objectives

* Build and secure an enterprise-like network environment
* Deploy and manage Active Directory
* Implement centralized log collection and monitoring
* Create custom detection rules and alerts
* Simulate real-world attacks and validate detections
* Practice vulnerability assessment and web application security testing
* Develop incident investigation and threat hunting skills

---

## Lab Architecture

### Network Components

| System                             | IP Address    | Purpose                                   |
| ---------------------------------- | ------------- | ----------------------------------------- |
| pfSense Firewall                   | 192.168.1.200 | Network perimeter security, routing, VPN  |
| Active Directory Domain Controller | 192.168.1.134 | Authentication and centralized management |
| Ubuntu Server                      | 192.168.1.55  | Wazuh SIEM and OWASP Juice Shop hosting   |
| Kali Linux                         | 192.168.1.244 | Attack simulation and security testing    |

### Security Stack

* pfSense Firewall
* Tailscale VPN
* Active Directory
* Wazuh SIEM
* Ubuntu Server
* Kali Linux
* OWASP Juice Shop
* Nmap
* Burp Suite

---

## Network Diagram

![Network Diagram](diagrams/network-diagram.png)

---

## Wazuh Architecture

![Wazuh Architecture](diagrams/wazuh-architecture.png)

---

## Repository Structure

```text
homelab-security-lab/
│
├── README.md
├── diagrams/
│
├── active-directory/
│   ├── setup.md
│   └── hardening.md
│
├── pfsense/
│   ├── firewall-rules.md
│   └── tailscale-vpn.md
│
├── wazuh/
│   ├── installation.md
│   ├── custom-rules.md
│   └── dashboards.md
│
├── detections/
│   ├── nmap-detection.md
│   ├── brute-force-detection.md
│   └── powershell-detection.md
│
├── owasp-juice-shop/
│   ├── deployment.md
│   └── findings.md
│
└── screenshots/
```

---

## Active Directory

The Active Directory environment was deployed to simulate a Windows enterprise network.

### Key Activities

* Domain Controller deployment
* User and Group management
* Organizational Unit configuration
* Group Policy administration
* Security hardening
* Authentication monitoring

Documentation:

* Active Directory Setup
* Active Directory Hardening

---

## pfSense Firewall

pfSense acts as the network gateway and security perimeter.

### Features Implemented

* Stateful firewall rules
* Network segmentation
* Secure remote access
* VPN connectivity through Tailscale
* Traffic monitoring

Documentation:

* Firewall Rules
* Tailscale VPN Configuration

---

## Wazuh SIEM

Wazuh provides centralized logging, monitoring, and threat detection across the lab environment.

### Implemented Capabilities

* Log aggregation
* Security event monitoring
* Threat detection
* Custom detection rules
* Dashboard creation
* Alert investigation

Documentation:

* Wazuh Installation
* Custom Rules
* Dashboards

---

## Detection Engineering

Several detection use cases were developed and validated through attack simulations.

### Detection Use Cases

#### Nmap Scan Detection

Detects network reconnaissance and port scanning activity.

#### Brute Force Detection

Identifies repeated authentication failures and potential credential attacks.

#### PowerShell Monitoring

Detects suspicious PowerShell execution activity on Windows systems.

Documentation:

* Nmap Detection
* Brute Force Detection
* PowerShell Detection

---

## OWASP Juice Shop

OWASP Juice Shop is deployed as a vulnerable web application for security testing and detection validation.

### Activities Performed

* Application deployment
* Vulnerability assessment
* Security testing
* Alert validation through Wazuh monitoring

Documentation:

* Deployment Guide
* Findings and Analysis

---

## Skills Demonstrated

### Blue Team

* Security Monitoring
* SIEM Administration
* Log Analysis
* Detection Engineering
* Incident Investigation
* Threat Hunting

### Infrastructure

* Active Directory Administration
* Windows Server Management
* Linux Administration
* Firewall Management
* VPN Deployment

### Offensive Security

* Vulnerability Assessment
* Web Application Testing
* Network Enumeration
* Attack Simulation

## Screenshots

### Wazuh Dashboard

![Wazuh Dashboard](screenshots/wazuh-dashboard.png)

### pfSense Dashboard

![pfSense Dashboard](screenshots/pfsense-dashboard.png)

### Active Directory

![Active Directory](screenshots/ad-users.png)

### OWASP Juice Shop

![Juice Shop](screenshots/juice-shop.png)


## Future Improvements

* VLAN Segmentation
* Sysmon Integration
* Active Response Automation
* Threat Intelligence Integration
* Security Orchestration Workflows
* Detection Coverage Expansion
* Purple Team Exercises

## Disclaimer

This lab is intended for educational, research, and defensive security purposes only. All attack simulations are performed within an isolated and controlled environment.

## Author

Munashe Maposa

Cybersecurity | SOC Operations | Detection Engineering | Penetration Testing

GitHub: https://github.com/YOUR_USERNAME
LinkedIn: https://linkedin.com/in/YOUR_PROFILE
