# JIRA Help Desk SLA Project — Ticketing System

![Jira Service Management](https://img.shields.io/badge/Jira_Service_Management-0052CC?style=for-the-badge&logo=jira&logoColor=white)
![SLA Tracking](https://img.shields.io/badge/SLA_Tracking-Active-1D9E75?style=for-the-badge)
![Automation](https://img.shields.io/badge/Automation_Rules-3_Active-534AB7?style=for-the-badge)
![Tickets Resolved](https://img.shields.io/badge/Tickets_Resolved-9-0F6E56?style=for-the-badge)

---

## What This Is

I built this lab because the role I was targeting asked specifically for JIRA experience -- SLA tracking, escalation workflows, and a quarterly optimization review. I didn't have that on paper, so I built the environment from scratch to show I understood the work, not just the terminology.

The project runs on Jira Service Management's free tier. I set up a full IT help desk for a fictional company called TechBridge IT Help Desk, configured priority-based SLA rules that match real enterprise targets, wired up three automation rules to handle ticket assignment and escalation without manual steps, then ran 9 tickets through the system from open to resolved.

---

## The Problem I Was Solving

Most help desk failures aren't technical. They happen because nobody noticed a ticket sat unacknowledged for six hours, or because an SLA breach didn't trigger anything until a manager asked. This project builds the infrastructure that catches those problems automatically -- the same infrastructure the job description asked for by name.

---

## What I Built

### SLA Framework

Three SLA rules, priority-based across five levels:

| Priority | First Response | Resolution |
|----------|---------------|------------|
| Highest | 2 hours | 12 hours |
| High | 4 hours | 24 hours |
| Medium | 6 hours | 36 hours |
| Low | 8 hours | 48 hours |
| All remaining | 12 hours | 60 hours (3 business days) |

The 4-hour high-priority response and 3-business-day resolution targets are pulled directly from the job description I was targeting. An employer gets someone who already knows what the SLA targets should be and how to configure them.

---

### Automation Rules

Three rules running without any manual steps:

| Rule | Trigger | Action |
|------|---------|--------|
| Auto-assign | New ticket created | Assigns to agent using balanced workload |
| SLA Warning | 30 minutes before breach | Adds comment notifying assignee to act |
| SLA Escalation | SLA breached | Flips priority to Highest, adds escalation comment |

No one has to remember to check. The system handles it.

---

### Ticket Queue

Nine tickets across real IT support scenarios, each opened, worked, commented, and resolved:

| Key | Summary | Priority | Status |
|-----|---------|----------|--------|
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
- 4-hour first response target matched exactly to enterprise IT support requirements
- 3-business-day resolution target enforced by automation, not manual follow-up

---

## The Quarterly Review Connection

The job description required a Quarterly Ticketing and Version Control Optimization Review -- a formal report on ticket resolution performance and workflow gaps. My [Help Desk Documentation System](https://github.com/agizopacifique-beep/helpdesk-documentation) lab produced exactly that kind of report. This JIRA lab is the live system that feeds it.

---

## Repository Layout

```
JIRA-Help-Desk-SLA-Project-Ticketing-System/
├── README.md
└── screenshots/
    ├── 01-project-overview.png
    ├── 02-sla-config-overview.png
    ├── 03-sla-first-response.png
    ├── 04-sla-resolution.png
    ├── 05-automation-rules-list.png
    ├── 06-automation-auto-assign.png
    ├── 07-automation-sla-warning.png
    ├── 08-automation-escalation.png
    ├── 09-ticket-queue-all.png
    ├── 10-ticket-detail-resolved.png
    ├── 11-sla-report.png
    └── 12-queue-resolved.png
```

---

## Skills This Project Covers

**Ticketing and ITSM**
Jira Service Management · SLA configuration · Escalation procedures · Queue management · Ticket triage · First-contact resolution · ITSM best practices

**Automation**
Jira automation rules · SLA breach workflows · Auto-assignment · Notification triggers · Escalation logic

**Documentation and Reporting**
Ticket resolution documentation · SLA performance reporting · Process improvement analysis · Quarterly review methodology

**IT Support Scenarios**
Account lockouts · Password resets · VPN troubleshooting · Software installation · Hardware setup · Offboarding procedures · Access management

---

## Environment

| Component | Details |
|-----------|---------|
| Platform | Jira Service Management (Free Tier) |
| Project Name | TechBridge IT Help Desk1 |
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
