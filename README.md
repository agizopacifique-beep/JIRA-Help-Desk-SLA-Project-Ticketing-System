# JIRA Help Desk SLA Project — Ticketing System

![Jira Service Management](https://img.shields.io/badge/Jira_Service_Management-0052CC?style=for-the-badge&logo=jira&logoColor=white)
![SLA Tracking](https://img.shields.io/badge/SLA_Tracking-Active-1D9E75?style=for-the-badge)
![Automation](https://img.shields.io/badge/Automation_Rules-3_Active-534AB7?style=for-the-badge)
![Tickets Resolved](https://img.shields.io/badge/Tickets_Resolved-9-0F6E56?style=for-the-badge)

---

## What This Is

This project is a fully functional IT help desk environment built in Jira Service Management. The goal was hands-on practice with the tools enterprises actually use -- not just reading about them. I configured the SLA framework, wired up automation rules, and ran real ticket scenarios through the system from open to resolved.

The setup covers what most IT support roles expect on day one: knowing how tickets move, when escalation kicks in, and what a breach looks like before it becomes a problem.

---

## The Problem This Solves

Help desk failures are rarely about missing technical knowledge. They happen because a ticket sat unacknowledged too long, or an SLA breach triggered nothing until someone complained. This project builds the infrastructure that catches those gaps automatically -- SLA rules, escalation logic, and automation that runs without anyone having to remember to check.

---

## What I Built

### SLA Framework

Three SLA rules, priority-based across five levels:

| Priority | First Response | Resolution |
|---|---|---|
| Highest | 2 hours | 12 hours |
| High | 4 hours | 24 hours |
| Medium | 6 hours | 36 hours |
| Low | 8 hours | 48 hours |
| All remaining | 12 hours | 60 hours (3 business days) |

The 4-hour high-priority response and 3-business-day resolution targets reflect real enterprise IT support standards.

---

### Automation Rules

Three rules running without any manual steps:

| Rule | Trigger | Action |
|---|---|---|
| Auto-assign | New ticket created | Assigns to agent using balanced workload |
| SLA Warning | 30 minutes before breach | Adds comment notifying assignee to act |
| SLA Escalation | SLA breached | Flips priority to Highest, adds escalation comment |

No one has to remember to check. The system handles it.

---

### Ticket Queue

Nine tickets across real IT support scenarios, each opened, worked, commented, and resolved:

| Key | Summary | Priority | Status |
|---|---|---|---|
| SUP-1 | User locked out of Microsoft 365 | Highest | Resolved |
| SUP-2 | Password reset request - Finance department | Medium | Resolved |
| SUP-3 | VPN not connecting - remote user | High | Resolved |
| SUP-4 | Software install request - Adobe Acrobat | Low | Resolved |
| SUP-5 | Printer offline - HR department | Medium | Resolved |
| SUP-6 | Email not syncing on mobile device | Medium | Resolved |
| SUP-7 | Microsoft Teams call quality issues | Medium | Resolved |
| SUP-8 | Access request - shared Finance drive | Low | Resolved |
| SUP-9 | Offboarding - disable departing employee account | Highest | Resolved |

---

## Key Results

- 9 tickets created and resolved in a single session
- 3 automation rules eliminating manual escalation steps
- 3 SLA tiers configured across 5 priority levels
- 0 tickets left unresolved
- 4-hour first response target matched to enterprise IT support standards
- 3-business-day resolution target enforced by automation, not manual follow-up

---

## The Quarterly Review Connection

A real IT support role requires periodic reporting on ticket resolution performance, workflow gaps, and process improvement recommendations. My [Help Desk Documentation System](https://github.com/agizopacifique-beep/helpdesk-documentation) lab produced exactly that kind of report. This JIRA lab is the live system that feeds it.

---

## Repository Layout

```
JIRA-Help-Desk-SLA-Project-Ticketing-System/
├── README.md
└── screenshots/
    ├── 01-jira-dashboard.png
    ├── 02-sla-config-overview.png
    ├── 02-sla-first-response.png
    ├── 03-sla-resolution.png
    ├── 04-automation-rules-list.png
    ├── 04-automation-templates.png
    ├── 05-automation-auto-assign.png
    ├── 06-automation-sla-warning.png
    ├── 07-automation-escalation.png
    ├── 08-ticket-queue-all.png
    ├── 09-ticket-detail-SUP1.png
    ├── 10-sla-report.png
    ├── 11-sla-report.png
    └── 12-queue-resolved.png
```

---

## Skills This Project Covers

**Ticketing and ITSM**
Jira Service Management, SLA configuration, escalation procedures, queue management, ticket triage, first-contact resolution, ITSM best practices

**Automation**
Jira automation rules, SLA breach workflows, auto-assignment, notification triggers, escalation logic

**Documentation and Reporting**
Ticket resolution documentation, SLA performance reporting, process improvement analysis, quarterly review methodology

**IT Support Scenarios**
Account lockouts, password resets, VPN troubleshooting, software installation, hardware setup, offboarding procedures, access management

---

## Environment

| Component | Details |
|---|---|
| Platform | Jira Service Management (Free Tier) |
| Project Name | TechBridge IT Help Desk |
| Project Key | SUP |
| SLA Rules | 3 configured |
| Automation Rules | 3 active |
| Tickets Created | 9 |
| Tickets Resolved | 9 |
| Resolution Rate | 100% |

---

## Contact

**Pacifique Agizo**
IT Help Desk Support Engineer | Active Directory & Identity Specialist

[![LinkedIn](https://img.shields.io/badge/LinkedIn-agizopacifique-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/agizopacifique)
[![GitHub](https://img.shields.io/badge/GitHub-agizopacifique--beep-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/agizopacifique-beep)

---

*Every result in this project is real, tested, and reproducible.*
