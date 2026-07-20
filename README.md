# 🏠 Home Security Operations Lab

**Built by:** Logan Graham  
**Purpose:** Hands-on security operations practice — detection engineering, log analysis, and incident response simulation  
**Status:** 🔄 Active build — started July 2026

---

## 📋 Overview

This repository documents my home SOC lab environment, built to develop hands-on skills beyond my professional environment. My day job involves SIEM triage and incident response at the analyst level — this lab is where I practice writing detections, simulating attacks, and building the engineering depth I'm working toward.

**The goal:** Move from consuming detections to building them.

---

## 🔧 Lab Architecture

```
┌─────────────────────────────────────────┐
│           Host Machine                  │
│           Windows 11                   │
│                                         │
│  ┌──────────────────┐                  │
│  │   VirtualBox     │                  │
│  │                  │                  │
│  │  ┌────────────┐  │                  │
│  │  │   Wazuh    │  │  ← SIEM/XDR     │
│  │  │   Server   │  │                  │
│  │  │  (Ubuntu)  │  │                  │
│  │  └────────────┘  │                  │
│  └──────────────────┘                  │
│                                         │
│  Wazuh Agent installed on host         │
│  (Windows logs → Wazuh SIEM)           │
└─────────────────────────────────────────┘
```

---

## 🛠️ Tools & Stack

| Tool | Purpose | Status |
|---|---|---|
| VirtualBox | Virtualization platform | ✅ Installed |
| Wazuh SIEM | Security monitoring, detection, alerting | 🔄 Setting up |
| Windows 11 (host) | Endpoint being monitored | ✅ Ready |
| Ubuntu Server (VM) | Wazuh server OS | 🔄 Setting up |

---

## 📁 Repository Structure

```
homelab/
├── README.md               ← You are here
├── setup-docs/             ← Installation notes and configuration
│   └── wazuh-setup.md
├── detection-rules/        ← Custom Wazuh detection rules (XML)
│   └── README.md
├── findings/               ← Documented investigations and exercises
│   └── README.md
└── screenshots/            ← Evidence of lab work
```

---

## 📓 Setup Log

*Documenting progress week by week*

### Week 1 — Environment Setup
**Goal:** Get Wazuh running in VirtualBox  
**Status:** 🔄 In progress  
**Notes:** *Will update as setup progresses*

---

## 🎯 Learning Objectives

- [ ] Deploy and configure Wazuh SIEM from scratch
- [ ] Connect Windows endpoint as monitored agent
- [ ] Understand Wazuh rule syntax and write custom detection rules
- [ ] Simulate common attack techniques (failed logins, new user creation, suspicious processes)
- [ ] Document detection gaps and tune rules to reduce false positives
- [ ] Build incident response runbooks based on simulated scenarios
- [ ] Map detected behaviors to MITRE ATT&CK framework

---

## 🗺️ Roadmap

| Phase | Focus | Status |
|---|---|---|
| Phase 1 | Wazuh setup and agent connection | 🔄 In progress |
| Phase 2 | Log ingestion and baseline understanding | ⏳ Planned |
| Phase 3 | Custom detection rule writing | ⏳ Planned |
| Phase 4 | Attack simulation and detection validation | ⏳ Planned |
| Phase 5 | Threat hunting exercises | ⏳ Planned |

---

## 🔗 Resources I'm Using

- [Wazuh Documentation](https://documentation.wazuh.com)
- [Wazuh OVA Quick Start](https://documentation.wazuh.com/current/deployment-options/virtual-machine/virtual-machine.html)
- [MITRE ATT&CK Framework](https://attack.mitre.org)
- [TryHackMe SOC Level 1 Path](https://tryhackme.com/path/outline/soclevel1)

---

## 📬 Connect

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Logan_Graham-0077B5?style=flat&logo=linkedin)](https://www.linkedin.com/in/logangrahamofficial/)
[![Email](https://img.shields.io/badge/Email-logangraham2002@gmail.com-D14836?style=flat&logo=gmail)](mailto:logangraham2002@gmail.com)

*This lab is actively being built. Check back for updates as detection rules, findings, and documentation are added.*
