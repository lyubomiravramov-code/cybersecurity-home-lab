# Cybersecurity Home Lab

**A student cybersecurity portfolio documenting hands-on learning in Linux, virtualisation, network reconnaissance and security analysis.**

> **Status:** An actively developing learning portfolio. The material here describes exercises I have worked on; it does not represent professional penetration-testing engagements or independently validated vulnerability findings.

## What this project covers

- A controlled lab with **Kali Linux** and deliberately vulnerable **Metasploitable2** virtual machines.
- Virtual network configuration using **VMware NAT and host-only adapters**.
- **Nmap** host discovery, port scanning and service-version identification.
- Analysis of network exposure and safe documentation of technical observations.
- Ethical testing boundaries, evidence handling and remediation-oriented thinking.

## Repository guide

| Folder | Contents |
| --- | --- |
| [`docs/`](docs/) | Lab architecture, methodology, ethics and learning log |
| [`lab-reports/`](lab-reports/) | Case studies and evidence-aware technical reports |
| [`commands/`](commands/) | Educational Nmap commands with explanation |
| [`templates/`](templates/) | Reusable report template for new exercises |
| [`screenshots/`](screenshots/) | Instructions for adding sanitised evidence (no private screenshots included yet) |

## Lab overview

```text
                 VMware virtual networking
                ┌────────────────────────────┐
                │ Kali Linux (testing VM)    │
                │           │                │
                │   isolated lab segment     │
                │           │                │
                │ Metasploitable2 (target VM)│
                └────────────────────────────┘
```

This is a conceptual diagram. For actual configuration details, see [Lab Architecture](docs/lab-architecture.md). No publicly routable target addresses or secrets are provided.

## Featured exercises

### 1. Kali Linux and Metasploitable2 setup
I have worked with Kali Linux and Metasploitable2 virtual machines, including adapting network settings and maintaining a clean lab snapshot. See [Lab Setup](lab-reports/01-virtual-lab-setup.md).

### 2. Reconnaissance with Nmap
I have used Nmap to discover devices, inspect open ports and identify exposed services. My lab work included examining service responses from Metasploitable2. See [Network Reconnaissance](lab-reports/02-network-reconnaissance.md) and [Nmap Command Reference](commands/nmap-reference.md).

### 3. Understanding vulnerabilities
I have inspected exposure information for a deliberately vulnerable host and considered how detected services inform prioritisation and defensive recommendations. See [Vulnerability Assessment Notes](lab-reports/03-vulnerability-assessment.md).

## Key learning

- Fundamentals of TCP/IP, service discovery and network segmentation.
- Running and interpreting basic Nmap scans.
- Operating Linux tools in a virtualised lab.
- Distinguishing **an observed open service** from **a confirmed exploitable vulnerability**.
- Writing reproducible technical documentation and noting evidence limitations.

## Evidence and limitations

This initial version contains structured write-ups but **does not yet include original screenshots, raw scan output or exploit demonstrations**. The reports label the difference between remembered lab observations and newly verified results. Evidence can be added later from an authorised lab after checking for secrets and sensitive data.

## Responsible use

These materials are for education and authorised security work only. Never scan or assess systems without permission. Avoid publishing credentials, personal information, live IP addresses, authentication tokens or unrestricted sensitive scan outputs. See [Responsible Use](docs/responsible-use.md).

## About me

I am a UK computing undergraduate developing practical cybersecurity skills alongside coursework and Google Cybersecurity Professional Certificate coursework completed through Course 5. My interests include security operations, vulnerability assessment, network defence and automation.

**Portfolio maintained by:** [lyubomiravramov-code](https://github.com/lyubomiravramov-code)
