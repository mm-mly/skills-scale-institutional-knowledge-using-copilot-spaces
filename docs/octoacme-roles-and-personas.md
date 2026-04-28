# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

**Document Owner:** Project Manager  
**Contributors:** Product Manager, Team Leads, All Role Representatives

---

## Roles Overview

| Role | Primary Focus | Key Collaborators |
|---|---|---|
| Developer | Implementation, testing, and delivery | PM, PdM, QA Lead, DevOps Engineer |
| Product Manager (PdM) | Outcome definition, backlog prioritization | PM, Developers, Stakeholders, UX Designer |
| Project Manager (PM) | Delivery coordination, risk, communication | All roles |
| UX Designer | User experience, design, usability | PdM, Developers, QA Lead |
| Technical Writer | Documentation accuracy, onboarding content | All roles |
| QA Lead | Test strategy, quality gates, release readiness | Developers, PM, PdM, DevOps Engineer |
| DevOps Engineer | CI/CD, environments, deployments, monitoring | Developers, PM, QA Lead |

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

### Example Interactions with Other Roles
- **QA Lead:** Collaborate on test coverage, review acceptance criteria, and address defects flagged during QA cycles.
- **DevOps Engineer:** Coordinate on CI/CD pipeline requirements, environment configuration, and deployment readiness.
- **UX Designer:** Implement UI components based on wireframes/mockups; flag implementation constraints early.
- **Technical Writer:** Provide technical details to support documentation; review developer-facing docs for accuracy.

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

### Example Interactions with Other Roles
- **UX Designer:** Define user research goals, review personas and wireframes, validate usability findings against product priorities.
- **QA Lead:** Confirm acceptance criteria are testable and sign off on release readiness.
- **Technical Writer:** Review documentation for accuracy against product intent; provide input on user-facing content.
- **DevOps Engineer:** Coordinate on release timing, environment requirements, and operational readiness for new features.

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

### Example Interactions with Other Roles
- **QA Lead:** Confirm quality gates are met before release; track QA progress against milestones.
- **DevOps Engineer:** Schedule deployment windows, review deployment checklists, and confirm rollback readiness.
- **UX Designer:** Ensure UX deliverables are on track and incorporated into sprint plans.
- **Technical Writer:** Verify documentation deliverables are included in project timelines; ensure release notes are complete.

---

## UX Designer

### Role Summary
UX Designers drive user-centered design across features and products. They translate user research, business requirements, and technical constraints into intuitive, high-quality user experiences. They serve as the bridge between what users need and what teams build.

### Responsibilities
- Lead user research, surveys, and usability studies
- Define user experience goals and success criteria for features
- Deliver wireframes, mockups, and interactive prototypes
- Create and maintain a shared design system or component library
- Run usability tests and synthesize feedback into actionable recommendations
- Advocate for accessibility and inclusive design standards

### Goals
- Improve product usability and user satisfaction
- Reduce rework by surfacing UX requirements early in planning
- Ensure consistent design patterns across the product

### Typical Communication
- Design reviews and critiques with Developers and PdMs
- Usability study reports shared with Stakeholders and PdMs
- Asynchronous feedback via design tools (e.g., Figma) and issue comments

### Example Interactions with Other Roles
- **Product Manager (PdM):** Collaborate on translating product requirements into user stories and design briefs; review research findings together.
- **Developers:** Share detailed design specs and component documentation; participate in implementation reviews to ensure design fidelity.
- **QA Lead:** Define usability acceptance criteria; participate in user acceptance testing (UAT) cycles.
- **Technical Writer:** Provide UI copy, labels, and in-app guidance language for documentation.
- **Project Manager (PM):** Report design milestone status; flag design dependencies that may affect sprint timelines.

---

## Technical Writer

### Role Summary
Technical Writers are responsible for the accuracy, clarity, and completeness of all project and product documentation. They ensure that process docs, developer guides, user guides, and onboarding materials are up-to-date, well-organized, and accessible to their intended audiences.

### Responsibilities
- Author and maintain user-facing and developer-facing documentation
- Create onboarding guides and process walkthroughs for new team members
- Review and validate clarity and completeness of project artifacts (specs, release notes, retrospective summaries)
- Manage documentation versioning and change history
- Establish and enforce documentation standards and templates
- Collaborate with subject-matter experts to ensure technical accuracy

### Goals
- Ensure all stakeholders have access to clear, current, and complete information
- Reduce onboarding time for new team members
- Improve the quality and consistency of documentation across the project

### Typical Communication
- Review cycles and feedback via pull requests or documentation tools
- Collaboration sessions with Developers, QA, and UX to gather technical details
- Documentation status updates in weekly PM syncs

### Example Interactions with Other Roles
- **Developers:** Interview for technical accuracy of developer docs; review implementation notes and PR descriptions.
- **QA Lead:** Document test plans, acceptance criteria, and known issues; ensure release notes reflect QA findings.
- **UX Designer:** Incorporate UX copy and UI guidance into user-facing documentation.
- **Product Manager (PdM):** Align user documentation with product intent; review and update docs after feature changes.
- **Project Manager (PM):** Track documentation deliverables as project milestones; flag doc gaps that could block release readiness.

---

## QA Lead

### Role Summary
The QA Lead coordinates and owns the testing strategy for the project, ensuring that features meet quality standards before release. They define test coverage requirements, manage manual and automated test plans, and serve as the quality gate owner across the delivery lifecycle.

### Responsibilities
- Define and maintain the overall test strategy (unit, integration, end-to-end, exploratory)
- Create, review, and maintain test plans and test case libraries
- Coordinate manual and automated testing activities across sprints
- Track, triage, and report on defects and quality metrics
- Own the Definition of Done (DoD) and release readiness criteria
- Partner with Developers to build a culture of quality and testability
- Sign off on release readiness before each deployment

### Goals
- Prevent defects from reaching production
- Ensure features meet all documented acceptance criteria
- Improve test automation coverage over time
- Provide stakeholders with clear, data-driven quality metrics

### Typical Communication
- QA status reports in weekly delivery syncs
- Defect triage sessions with Developers and PM
- Release readiness sign-off shared with PM, PdM, and Stakeholders

### Example Interactions with Other Roles
- **Developers:** Collaborate on testability, review acceptance criteria, triage defects, and integrate automated tests into CI.
- **Product Manager (PdM):** Confirm acceptance criteria are complete and testable before sprint commitment; validate user acceptance.
- **Project Manager (PM):** Report QA status and release readiness; escalate critical quality risks that may affect timelines.
- **DevOps Engineer:** Integrate test suites into CI/CD pipelines; align on environment configuration needed for test execution.
- **Technical Writer:** Provide input for test case documentation and known issues in release notes.
- **UX Designer:** Participate in usability and accessibility testing; validate UX acceptance criteria.

---

## DevOps Engineer

### Role Summary
DevOps Engineers design, implement, and maintain the CI/CD pipelines, deployment infrastructure, and operational monitoring that enable reliable, repeatable software delivery. They bridge the gap between development and operations, ensuring that code can be delivered safely and efficiently to any environment.

### Responsibilities
- Design and maintain CI/CD pipelines and build automation
- Manage deployment environments (dev, staging, production) and infrastructure-as-code
- Implement monitoring, alerting, and observability tooling
- Own the deployment runbook and rollback procedures
- Enforce security scanning and compliance checks in the pipeline
- Coordinate deployment windows and production readiness reviews
- Conduct post-incident root cause analysis and drive operational improvements

### Goals
- Enable fast, safe, and reliable software delivery
- Reduce mean time to recovery (MTTR) for production incidents
- Increase deployment frequency while decreasing change failure rate
- Maintain operational visibility across all environments

### Typical Communication
- Deployment status updates to PM and Stakeholders
- Incident notifications and post-mortem reports
- Pipeline and infrastructure change communication to Developers and QA

### Example Interactions with Other Roles
- **Developers:** Provide CI/CD tooling and guidance; review code for deployment readiness; support environment onboarding.
- **QA Lead:** Integrate automated test suites into pipelines; ensure staging environments mirror production for reliable test results.
- **Project Manager (PM):** Confirm deployment window scheduling; review deployment checklist and rollback readiness before releases.
- **Product Manager (PdM):** Communicate operational constraints that may affect feature delivery timelines; share monitoring insights on feature usage.
- **Technical Writer:** Provide documentation of pipeline processes, runbooks, and operational procedures.

---

## Stakeholders

### Role Summary
Stakeholders include sponsors, business owners, customer representatives, and other teams with an interest in project outcomes. They provide strategic direction, approve key decisions, and receive regular project communications.

### Responsibilities
- Provide business context and strategic priorities
- Review and approve project gate decisions (initiation, major milestones, release)
- Offer feedback on deliverables and prototypes
- Escalation point for cross-organizational issues

### Goals
- Ensure the project delivers expected business value
- Maintain visibility into project health and risks
- Enable timely decisions to unblock the team

### Typical Communication
- Monthly stakeholder updates or milestone-based briefings
- Decision requests via PM for gate approvals
- Ad hoc escalation as needed

### Example Interactions with Other Roles
- **Project Manager (PM):** Receive status reports; approve gates and key decisions; escalation path for business-critical issues.
- **Product Manager (PdM):** Review roadmap priorities; validate product direction aligns with business goals.
- **QA Lead:** Review release readiness reports and quality metrics before major releases.

---

## RACI Summary

| Activity | PM | PdM | Developer | UX Designer | Tech Writer | QA Lead | DevOps Eng | Stakeholders |
|---|---|---|---|---|---|---|---|---|
| Project initiation & one-pager | **A** | R | I | I | I | I | I | C |
| Backlog prioritization | C | **A** | C | C | I | C | I | C |
| Sprint planning | **A** | R | R | R | I | R | C | I |
| Feature design & UX | I | C | C | **A** | C | C | I | I |
| Implementation | I | I | **A** | C | I | C | C | I |
| Test strategy & execution | C | C | R | C | C | **A** | C | I |
| CI/CD & deployment | C | I | C | I | C | C | **A** | I |
| Documentation | R | C | C | C | **A** | C | C | I |
| Release sign-off | **A** | R | C | I | C | R | R | C |
| Stakeholder communication | **A** | C | I | I | C | I | I | R |
| Retrospective facilitation | **A** | C | R | R | R | R | R | I |

*R = Responsible, A = Accountable, C = Consulted, I = Informed*

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.
- Reference the RACI table when assigning owners to checklist items in other process documents.

