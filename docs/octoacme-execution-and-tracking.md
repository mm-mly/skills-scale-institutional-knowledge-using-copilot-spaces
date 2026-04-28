# OctoAcme — Execution & Tracking

**Document Owner:** Project Manager  
**Contributors:** Developers, QA Lead, DevOps Engineer, UX Designer, Technical Writer, Product Manager

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies; all delivery roles attend
- Weekly delivery sync — PM facilitates; QA Lead reports quality status; DevOps Engineer shares pipeline/deployment updates
- Demo/Review at the end of each sprint or milestone — UX Designer, Developer, and QA Lead present
- Monthly stakeholder update — PM prepares; PdM and QA Lead contribute content

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Each item in the "Done" column must meet the [Definition of Done](octoacme-project-planning.md#quality-gate--definition-of-done-dod)
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review (DevOps Engineer configures; Developers maintain)
  - Require at least one approval before merging (or team-defined policy)
  - QA Lead reviews PRs for testability and coverage gaps on significant changes

## Quality & Testing
- Unit tests for new logic (Developer)
- Integration tests where applicable (Developer + QA Lead)
- End-to-end smoke tests for critical flows before release (QA Lead)
- Security scanning in CI (DevOps Engineer)
- Manual QA for feature acceptance when needed (QA Lead)
- Usability review for user-facing changes (UX Designer)

## QA Review Procedure
When a feature is ready for QA:
1. Developer moves the item to the **QA** column on the project board
2. QA Lead reviews acceptance criteria and runs the test plan
3. Defects are logged as issues and linked to the feature item
4. Defects are triaged: **Critical/High** → PM and Developer notified immediately; **Medium/Low** → tracked in backlog
5. QA Lead moves the item to **Done** only when all acceptance criteria are verified and no open Critical/High defects remain

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage) — DevOps Engineer owns dashboard setup
- QA Lead provides weekly defect trend and test coverage metrics

## Blocker Escalation
- **Level 1:** Team-level triage in daily standup (all delivery roles)
- **Level 2:** PM escalates to Product Lead and dependent teams within 1 business day
- **Level 3:** Sponsor-level escalation for business-impacting issues — PM prepares escalation summary within 4 hours
- **Security incidents:** Follow the security incident runbook (DevOps Engineer leads triage) and notify Security on-call immediately

## Execution Checklist
- [ ] Branching and PR conventions documented in repo (Technical Writer)
- [ ] CI configured for tests, lint, and security scanning (DevOps Engineer)
- [ ] QA Review Procedure communicated to all team members (QA Lead)
- [ ] Regular demos scheduled and UX Designer invited (PM)
- [ ] Risk register updated weekly (PM + risk owners)
- [ ] Escalation path reviewed with all team members at kickoff (PM)
