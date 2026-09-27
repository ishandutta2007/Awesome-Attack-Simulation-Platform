# Awesome-Attack-Simulation-Platform

## Top Attack Simulation Platform Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Breach & Attack Simulation (BAS), Adversary Emulation & Continuous Security Validation*  

**Last updated: March 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Attack Simulation Platforms**. These tools simulate real-world cyberattacks against an organization's infrastructure to validate security controls, test detection capabilities, and measure defensive posture against known threat actor behaviors.



**Examples** include SafeBreach, AttackIQ, Cymulate, Pentera, Picus Security, XM Cyber, Horizon3.ai, Scythe, Red Canary Atomic Red Team, and ThreatGen (the category leaders).



**Open-source emphasis**: This section is expanded with active projects for self-hosting, custom adversary emulation, and transparent security validation — ideal for purple teams, detection engineers, and security researchers building vendor-independent attack simulation programs. Note that while mature open-source adversary emulation frameworks exist, full BAS platforms with automated remediation guidance remain largely commercial.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms

**Market Size & Sector Overview:** The global Breach and Attack Simulation (BAS) & Continuous Security Validation market is estimated at **$550M–$1.0B in 2025/2026** (projected to reach **$3.6B–$16B by 2033** at a CAGR of ~22–40%). The sector is **moderately fragmented**, featuring specialized category leaders alongside emerging AI-native platforms evolving towards broader exposure management consolidation.

| Platform | Description | Company Size (Valuation / Revenue) | Starting Price | Free Tier / Trial Limit |
| :--- | :--- | :--- | :--- | :--- |
| **[Horizon3.ai](https://horizon3.ai/)** | Autonomous penetration testing platform (NodeZero) discovering exploitable vulnerabilities and validating attack paths with proof-of-exploit. | >$2.0B Valuation ($250M Series E, 120% YoY ARR growth) | ~$99/target for ad-hoc NodeZero pentest runs | 30-day Free Trial (up to 1 free internal/external node run upon credential verification) |
| **[Pentera](https://www.pentera.io/)** | Automated penetration testing platform simulating full attack chains from external and internal perspectives with actionable remediation. | >$1.0B Valuation ($117M ARR, Series D) | ~$35,000/year base annual subscription | No free trial (1-on-1 personalized live environment demo available) |
| **[XM Cyber](https://www.xmcyber.com/)** | Hybrid cloud exposure management platform simulating attack paths to critical assets, identifying and prioritizing remediation. | $700M Acquisition Value ($10M–$20M ARR) | ~$24/unit/year (£18/unit/year) enterprise tier | Custom-scoped 14-day Free Trial available via sales demo consultation |
| **[Cymulate](https://cymulate.com/)** | Extended security posture management platform with BAS, automated red teaming, and attack surface validation across email, web, and endpoint vectors. | $141M Total Funding (~$30M+ ARR) | ~$7,000/year starting modular tier | 14-day Free Trial with access to core validation modules |
| **[Red Canary](https://redcanary.com/atomic-red-team/)** | Managed continuous security validation platform with commercial orchestration built around Atomic Red Team. | $130M Total Funding ($100M+ ARR) | ~$120/endpoint/year starting managed subscription tier | No free trial for hosted SaaS platform (free open-source YAML library available) |
| **[SafeBreach](https://www.safebreach.com/)** | Continuous security validation platform with 20,000+ attack methods simulating known threat actor behaviors across the kill chain. | $106M Total Funding (~$21M ARR) | ~$25,000/year starting subscription tier (4 customizable tiers) | No free trial (guided proof-of-concept / sandbox demo on request) |
| **[Picus Security](https://www.picussecurity.com/)** | Security validation platform combining BAS with threat intelligence, measuring detection and prevention effectiveness across security stack. | $77M Total Funding (~$15M–$20M ARR) | ~$10,000/year starting subscription | 14-day Free Trial for Security Validation Platform |
| **[AttackIQ](https://www.attackiq.com/)** | Breach and attack simulation platform built on MITRE ATT&CK, enabling continuous validation of security controls with automated attack scenarios. | $73M Total Funding (~$15M ARR) | ~$15,000/year starting *Flex* testing package tier | AttackIQ Flex free tier (free access to basic ATT&CK testing packages & research) |
| **[Scythe](https://scythe.io/)** | Adversary emulation platform with threat intelligence-driven attack scenarios, purple team collaboration, and detection validation. | ~$15M Funding (~$5M–$10M ARR) | ~$15,000/year practitioner starting license | No free trial (guided interactive sandbox demo on request) |
| **[ThreatGen](https://www.threatgen.com/)** | Cyber range and attack simulation platform with gamified red team/blue team exercises for training and validation. | Early-Stage / Bootstrapped (~$1M–$3M ARR) | $75/year for Individual Pro; $1,500/year for Business tier | No free trial (free interactive video demo and sample scenarios on request) |



## Open-Source GitHub Projects



- **[MITRE Caldera](https://github.com/mitre/caldera)**  

  The leading open-source automated adversary emulation platform, originally developed by MITRE in 2017 and now transitioning to Apache Software Foundation incubation with 6,000+ GitHub stars under Apache-2.0 license . Uses lightweight agents (Sandcat for Windows/macOS/Linux) paired with a central C2 server that schedules and orchestrates ATT&CK-mapped techniques as "abilities" grouped into "adversaries" (playbooks) . Supports red team operations, purple team exercises, detection engineering, and continuous security validation . Includes TLS/HTTPS transport security and AES encryption for agent-server communications .



- **[OpenBAS](https://github.com/OpenBAS-Platform/openbas)**  

  Open-source breach and attack simulation platform from Filigran (creators of OpenCTI), ISO 22398 compliant . Unique capability to simulate every aspect of an incident — not just technical attacks, but also contextual events like journalist inquiries and CEO calls seeking immediate results . Features AI-powered scenario generation, integration with OpenCTI for threat intelligence-driven simulations, and a rich injector/collector ecosystem . Over 4,000 members in Slack community . Shipped as Docker images for easy self-hosting .



- **[Atomic Red Team](https://github.com/redcanaryco/atomic-red-team)**  

  Library of YAML files mapping to MITRE ATT&CK techniques for validating detection capabilities, created by Red Canary . The most notable agentless implementation with raw materials for every ATT&CK technique category . Requires manual execution of each technique on target systems — not well suited for automated full attack path emulation . Best used as a library of test cases rather than a standalone automated emulation platform.



- **[Infection Monkey](https://github.com/guardicore/monkey)**  

  Open-source, agent-based adversary emulation tool from Guardicore (now Akamai). Designed like a C2 framework with a central web server ("Monkey Island") and agents ("Monkeys") . Actions are predefined before agent generation; agents can self-propagate if configured . Less focused on tasking beacons than Caldera, but useful for lateral movement and network propagation testing .



- **[Splunk Attack Range](https://github.com/splunk/attack_range)**  

  Open-source project for spinning up instrumented cloud environments to simulate adversary behavior and test detections . Deploys Splunk instances, Windows/Linux servers, optional Kali, Zeek, and Active Directory-style layouts using Terraform and Ansible . Integrates with Atomic Red Team for attack simulation, with telemetry forwarded to Splunk for detection development . Available via Docker Compose with web UI, REST API, and CLI .



- **[PurpleSharp](https://github.com/mvelazc0/PurpleSharp)**  

  Adversary simulation tool for Windows Active Directory environments, automating attack simulation against AD remotely . Closest thing to a functioning agentless adversarial emulation tool for AD, though development has not continued in the past two years . Limited scope to Windows AD only, requires administrative credentials and SMB/RPC connectivity .



- **[Stratus Red Team](https://github.com/DataDog/stratus-red-team)**  

  "Atomic Red Team for the cloud" from Datadog — granular attack techniques for AWS, Azure, GCP, and Kubernetes . Does not resolve the shortcomings of Atomic Red Team regarding full attack chain emulation .



- **[DumpsterFire](https://github.com/joewalnes/dumpsterfire)**  

  Open-source agentless adversarial emulation toolset. Unmaintained for 8+ years with limited action set . Included for historical context only.



### Additional Strong Open-Source Options



- **Red Team Automation (RTA)** — Collection of scripts mapped to MITRE ATT&CK TTPs from Endgame, less comprehensive than Atomic Red Team .

- **VECTR** — Open-source purple team tracking and reporting tool for measuring detection coverage across exercises.

- **DeTT&CT** — Tool for mapping detection coverage against ATT&CK and identifying gaps, complementing attack simulation platforms.

- **Prelude Operator** — Open-source adversary emulation platform with cross-platform agents and a visual scenario builder.

- **Sliver** — Open-source C2 framework increasingly used in adversary emulation and red team engagements.



**Frameworks for building custom attack simulation programs**: Combine **MITRE Caldera** as the core adversary emulation engine with agent-based execution and ATT&CK-native playbooks . Integrate **Atomic Red Team** as a library of granular tests for detection validation . Use **OpenBAS** for crisis simulation and non-technical incident aspects, especially when integrated with OpenCTI for threat intelligence-driven scenarios . Deploy **Splunk Attack Range** for cloud-based detection engineering labs with full telemetry pipelines . For cloud-specific emulation, **Stratus Red Team** provides granular techniques for AWS, Azure, GCP, and Kubernetes .



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Attack simulation tools must be used only in authorized environments with proper legal approval. Unauthorized use may violate computer fraud laws.

- Self-hosted open-source solutions require proper infrastructure, security hardening, and ongoing maintenance.

- The open-source ecosystem provides strong adversary emulation frameworks and detection validation libraries, but full BAS platforms with automated remediation guidance remain primarily commercial offerings.



---



**Made for purple teams, detection engineers, red teamers, and security researchers.**  

Let's make attack simulation more open, transparent, and vendor-neutral.
