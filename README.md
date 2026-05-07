# AI in Cybersecurity

Hands-on two-day course for SOC analysts and detection engineers. Students build a complete security detection and investigation pipeline on AWS — from a bare EC2 instance through live automated AI-assisted investigations.

**Platform:** AWS (Amazon Linux 2023 EC2, CloudWatch, Security Hub, GuardDuty)  
**AI Tooling:** CloudWatch AI Operations; AI coding assistants (Amazon Q, GitHub Copilot, or equivalent)  
**Language:** Python 3.x and Bash

See [outline.md](outline.md) for full module descriptions, learning objectives, and course overview.


---

## Prerequisites

- Basic Python (reading files, writing functions, running scripts from the command line)
- Familiarity with common security concepts (authentication, SSH, privilege escalation, alerts)
- An AWS account with permissions to launch EC2 instances and enable Security Hub and GuardDuty
- No prior AWS experience required — cloud concepts are introduced in Lab 1.1

---

## Labs

Labs are completed in order. Each lab builds on artifacts from the previous one. Later labs on each day are supplemental — if time runs short the class finishes any started lab before moving on.

### Day 1 — Cloud Environment Setup, Log Evidence, AI-Assisted Scripting, and Security Posture

| # | Lab | Topics |
|---|---|---|
| 1.1 | [Instance Setup](labs/1.1-Instance-Setup.md) | EC2 launch, SSH, VS Code Remote SSH, Linux file permissions, SetUID binaries, security group hardening |
| 1.2 | [Suspicious Activity Simulation and Risk Scoring](labs/1.2-Suspicious-Activity-Simulation-and-Risk-Scoring.md) | Attack simulation (brute force, privilege escalation, account enumeration), auditd, journald, Python risk scorer |
| 1.3 | [AI-Assisted Security Scripting and IAM Review](labs/1.3-AI-Assisted-Security-Scripting-and-IAM-Review.md.md) | Prompt engineering, AI code review checklist, IAM least-privilege policy generation, Lambda execution roles |
| 1.4 | [AWS Security Posture Baseline](labs/1.4-AWS-Security-Posture-Baseline.md) | AWS CLI posture checks, Security Hub findings, GuardDuty, CloudTrail, controlled remediation |
| 1.5 | [Endpoint Telemetry and Alert Pipeline](labs/2.1-Endpoint-security-Integration.md) | CloudWatch agent, auditd → `/soc-lab/secure` log group, GuardDuty Runtime Monitoring, Python normalizer → `soc-alerts-normalized.jsonl` |

### Day 2 — AI-Powered Investigation, Detection Engineering, and SOC Automation

| # | Lab | Topics |
|---|---|---|
| 2.2 | [CloudWatch AI Operations](labs/2.2-CloudWatch-AI-Operations.md) | Logs Insights natural language queries, AI Operations configuration, AI investigation hypothesis evaluation |
| 2.3 | [Security Monitoring Dashboard and Automated Detection](labs/2.3-Security-Monitoring-Dashboard-and-Automated-Detection.md) | Metric filters (auditd syntax), CloudWatch alarms, SOC dashboard, alarm-triggered AI investigations |
| 2.4 | [Attack and Detect Capstone](labs/2.4-Attack-and-Detect-Capstone.md) | Independent detection pipeline build, attack simulation with `testattacker`, AI investigation evaluation, incident report |

## Reference

- [glossary.md](labs/glossary.md) — Key terms and AWS service definitions used throughout the course
