# OctoAcme — Risk Management & Communication

**Document Owner:** Project Manager  
**Contributors:** Product Manager, QA Lead, DevOps Engineer, Technical Writer

## Purpose
Explain how to identify, manage, and communicate risks and dependencies.

## Risk Register
Maintain a simple table with:
- ID
- Description
- Impact (High/Med/Low)
- Likelihood (High/Med/Low)
- Owner (assigned role — e.g., PM, DevOps Engineer, QA Lead)
- Mitigation plan
- Status

## Risk Lifecycle
- **Identify:** during planning and ongoing execution; all roles are responsible for surfacing risks in their domain
- **Assess:** estimate impact and likelihood
- **Mitigate:** reduced via actions, contingency plans
- **Monitor:** review at weekly syncs and update status

## Role-Specific Risk Ownership

| Risk Type | Primary Owner | Escalation Path |
|---|---|---|
| Schedule / delivery risk | Project Manager | Product Lead → Sponsor |
| Quality / defect risk | QA Lead | PM → Product Lead |
| Infrastructure / deployment risk | DevOps Engineer | PM → Sponsor |
| UX / usability risk | UX Designer | PM → PdM |
| Documentation completeness | Technical Writer | PM |
| Scope / requirements risk | Product Manager | PM → Sponsor |

## Stakeholder Communication
- Identify stakeholder groups and communication needs (e.g., engineering, sales, support)
- Provide regular updates (weekly or milestone-based)
- Use a single source of truth (project README or release doc) for status
- All communications must have a named author and owner

## Communication Cadence

| Audience | Frequency | Owner | Format |
|---|---|---|---|
| Delivery team | Daily | PM | Standup |
| Delivery team | Weekly | PM | Delivery sync |
| Stakeholders | Weekly or milestone | PM | Written status update |
| Stakeholders | Monthly | PM + PdM | Briefing or report |
| All hands / leadership | Per release | PM | Release announcement |

## Communication Templates

### Weekly Status Template
- **Owner:** Project Manager
- Progress this week:
- Next steps:
- Risks & blockers:
- QA status (owner: QA Lead):
- Deployment / infrastructure notes (owner: DevOps Engineer):
- Ask / decisions needed:

### Incident Communication
- **Owner:** Project Manager (PM) + DevOps Engineer
- Triage summary
- Actions being taken
- Expected timeline
- Post-incident blameless retrospective scheduled
- Stakeholders notified within: [Critical: 30 min | High: 2 hrs | Med: next business day]

## Escalation Paths

| Severity | Initial Owner | Level 1 | Level 2 | Level 3 |
|---|---|---|---|---|
| Delivery blocker | PM | Product Lead | Sponsor | Executive Sponsor |
| Critical quality defect | QA Lead | PM | Product Lead | Sponsor |
| Production incident | DevOps Engineer | PM | Security/Ops on-call | Sponsor |
| Scope change request | PdM | PM | Sponsor | — |

- **Timelines:** Level 1 escalation within 1 business day; Level 2 within 4 hours for critical issues; Level 3 immediately for business-impacting outages
- For security incidents, follow the security incident runbook and notify Security on-call immediately
