# 🛡️ SOC Analyst Portfolio

**A comprehensive portfolio showcasing hands-on security operations, threat detection, and incident response skills through real-world lab projects.**

![Status](https://img.shields.io/badge/status-open%20to%20work-2FBE9F?style=flat-square)
![SIEM](https://img.shields.io/badge/SIEM-Splunk-DD9A3D?style=flat-square)
![Network](https://img.shields.io/badge/Network-Wireshark-1B9CFC?style=flat-square)
![Lab](https://img.shields.io/badge/Lab-Kali%20Linux-557C94?style=flat-square)
![Honeypot](https://img.shields.io/badge/Threat--Intel-Honeypot-FF6B6B?style=flat-square)

> A self-directed cybersecurity training program focused on the full lifecycle of threat detection and incident response — from SIEM monitoring to network forensics to adversary intelligence.

---

## Table of Contents

- [About](#about)
- [Case Studies](#case-studies)
  - [CASE-001 · SIEM Threat Detection & Dashboards](#case-001--siem-threat-detection--dashboards)
  - [CASE-002 · Incident Triage, Ticketing & Reporting](#case-002--incident-triage-ticketing--reporting)
  - [CASE-003 · Network Traffic & Packet Analysis](#case-003--network-traffic--packet-analysis)
  - [CASE-004 · Honeypot Deployment & Threat Intelligence](#case-004--honeypot-deployment--threat-intelligence)
- [Skills & Tools](#skills--tools)
- [Lab Timeline](#lab-timeline)
- [Repository Structure](#repository-structure)
- [Contact](#contact)

---

## About

I'm building hands-on detection and response skills through a self-directed cybersecurity lab. With a foundation in IT support and networking, I've designed a practical training program that mirrors real SOC workflows:

- **Detection & Monitoring** — Standing up SIEM environments and writing queries to surface threats
- **Network Forensics** — Analyzing packet captures to understand attack patterns
- **Incident Response** — Triaging alerts, creating tickets, and writing incident reports
- **Threat Intelligence** — Deploying honeypots to observe adversary behavior firsthand

Each case below represents a complete project with real tool output, methodology, findings, and reflection.

**Lab Stack:** Splunk Enterprise · BOTSv2 Dataset · Wireshark · Kali Linux · Network Honeypots · Ticketing Workflows

---

## Case Studies

### CASE-001 · SIEM Threat Detection & Dashboards

`Detection & Monitoring` · `Splunk Enterprise` · `BOTSv2 Dataset` · `SPL`

**Objective:** Stand up a working SIEM environment and transform raw security logs into actionable visual monitoring using the industry-standard "Boss of the SOC" v2 dataset.

**What I Did:**
- Ingested and explored the BOTSv2 dataset structure in Splunk (indexes, sourcetypes, field mappings)
- Wrote SPL queries to surface indicators of compromise — suspicious authentication activity, anomalous process execution, unusual DNS patterns
- Designed and built operational dashboards from scratch: geospatial maps, timecharts, and top-talker panels
- Practiced live demos, narrating technical findings for non-technical audiences

**Skills Demonstrated:** SPL query writing · log correlation · dashboard design · technical presenting

📁 **Evidence:** [`/01-siem-threat-detection`](./01-siem-threat-detection) — SPL queries, dashboard screenshots, findings summary

---

### CASE-002 · Incident Triage, Ticketing & Reporting

`Incident Response` · `Alert Management` · `Reporting`

**Objective:** Practice the human side of SOC work — deciding what matters, tracking it, and handing it off professionally.

**What I Did:**
- Created structured incident tickets from dashboard alerts rather than leaving findings as one-off searches
- Practiced triage: assigning priority and severity based on asset criticality and business impact
- Wrote incident reports following standard SOC format — summary, timeline, indicators of compromise, remediation steps
- Treated documentation as a critical deliverable

**Skills Demonstrated:** Alert triage · severity assessment · ticketing workflows · incident report writing · stakeholder communication

📁 **Evidence:** [`/02-incident-response`](./02-incident-response) — incident report templates, sample tickets, triage methodology

---

### CASE-003 · Network Traffic & Packet Analysis

`Network Forensics` · `Wireshark` · `PCAP Analysis`

**Objective:** Build the habit of reading raw network traffic instead of relying on log summaries alone.

**What I Did:**
- Captured and analyzed live network traffic in Wireshark, examining protocol hierarchies before drilling into individual frames
- Applied display filters to isolate specific conversations and detect anomalies — unexpected ports, repeated connection attempts, suspicious patterns
- Followed TCP streams end-to-end to reconstruct session activity and identify data exfiltration attempts
- Compared baseline "normal" traffic against anomalous captures to refine detection patterns

**Skills Demonstrated:** Packet analysis · Wireshark filters · protocol analysis · traffic baselining · anomaly identification

📁 **Evidence:** [`/03-wireshark-analysis`](./03-wireshark-analysis) — capture notes, filter examples, annotated screenshots

---

### CASE-004 · Honeypot Deployment & Threat Intelligence

`Adversary Intelligence` · `Honeypot Deployment` · `Network Segmentation` · `Kali Linux`

**Objective:** Observe real adversary behavior by deploying isolated honeypots and analyzing attack patterns firsthand.

**What I Did:**
- Designed a segmented home lab network to safely expose honeypots without risking production systems
- Deployed honeypot instances (SSH, HTTP, DNS) on Kali Linux to passively log connection attempts and attack commands
- Analyzed honeypot logs to identify common attack patterns — credential spray attempts, scanning tools, follow-on exploitation
- Cross-referenced honeypot activity with Wireshark captures to build attacker behavior profiles

**Skills Demonstrated:** Honeypot configuration · network segmentation · log analysis · attacker TTP identification · threat modeling

📁 **Evidence:** [`/04-honeypot-intelligence`](./04-honeypot-intelligence) — network diagrams, attack logs, TTP analysis

---

## Skills & Tools

| Category | Skills & Tools |
|---|---|
| **Detection & Monitoring** | Splunk Enterprise, SPL queries, log correlation, dashboard design, KPI tracking |
| **Network Forensics** | Wireshark, tcpdump, protocol analysis, PCAP review, TCP stream reconstruction, baseline analysis |
| **Lab & Linux Ops** | Kali Linux, honeypot deployment, network segmentation, Linux CLI, firewall rules |
| **Incident Response** | Alert triage, severity assessment, ticketing workflows, incident reports, stakeholder communication |
| **Threat Intelligence** | Attacker TTP analysis, behavior profiling, indicators of compromise (IoCs), threat modeling |

---

## Lab Timeline

| Phase | Days | Focus |
|---|---|---|
| Foundations | 1–2 | Cybersecurity fundamentals, threat landscape, lab environment setup |
| SIEM Monitoring | 3–6 | Splunk deployment, BOTSv2 ingestion, SPL practice, dashboard design, live demo rehearsal |
| Network Forensics | 7–9 | Wireshark capture/filter practice, baseline vs. anomaly analysis, TCP stream reconstruction |
| Adversary Lab | 10–12 | Kali Linux honeypot setup, network isolation, log collection, attack pattern analysis |
| Incident Response | 13–14 | Ticketing workflow, triage practice, incident report writing, stakeholder handoff |
| Wrap-Up & Demo | 15 | Portfolio documentation, live presentation prep, lessons learned review |

---

## Repository Structure

```
MY-SOC-analyst-PORTFOLIO/
├── README.md                          # Main portfolio overview
├── 01-siem-threat-detection/
│   ├── README.md                      # CASE-001 detailed write-up
│   ├── spl-queries.md                 # Actual SPL queries with explanations
│   ├── findings.md                    # Key findings and indicators
│   └── screenshots/                   # Dashboard panels, visualizations
├── 02-incident-response/
│   ├── README.md                      # CASE-002 detailed write-up
│   ├── incident-report-template.md    # Standard IR report format
│   ├── sample-tickets.md              # Example ticket triage
│   └── triage-methodology.md          # Alert severity framework
├── 03-wireshark-analysis/
│   ├── README.md                      # CASE-003 detailed write-up
│   ├── pcap-findings.md               # Filters used and anomalies identified
│   ├── filter-cookbook.md             # Wireshark filter reference guide
│   └── screenshots/                   # Annotated captures and protocol trees
├── 04-honeypot-intelligence/
│   ├── README.md                      # CASE-004 detailed write-up
│   ├── network-diagram.md             # Lab architecture and segmentation
│   ├── attack-logs-analysis.md        # Honeypot log review and TTP extraction
│   └── artifacts/                     # Sample logs, attack payloads
└── assets/
    └── screenshots/                   # Shared media and visual assets
```

---

## Key Takeaways

This portfolio demonstrates:
- **Hands-on tool expertise** — Real experience with industry-standard SOC tools
- **Methodical approach** — Each case follows a clear objective → method → findings → reflection workflow
- **Communication skills** — Ability to translate technical findings for diverse audiences
- **Initiative & drive** — Self-directed learning and project execution outside formal training
- **Attention to detail** — Well-documented evidence and professional reporting

---

## Contact & Connect

- **GitHub:** [github.com/diliryo](https://github.com/diliryo)
- **LinkedIn:** [Add your LinkedIn profile]
- **Email:** [Add your email]

---

*Built as part of a self-directed SOC analyst training program. Last updated: June 2024.*
