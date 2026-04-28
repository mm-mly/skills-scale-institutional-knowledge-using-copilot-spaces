# OctoAcme — Release & Deployment Guide

**Document Owner:** DevOps Engineer  
**Contributors:** Project Manager, QA Lead, Technical Writer, Developers

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- **Patch:** hotfixes addressing critical production issues
- **Minor:** incremental features and improvements
- **Major:** significant functionality or breaking changes

## Pre-release Requirements
- All acceptance criteria met and PRs merged (Developer + QA Lead verify)
- Passing CI and security scans (DevOps Engineer confirms)
- Release notes drafted (Technical Writer)
- Rollback / mitigation plan documented (DevOps Engineer)
- Smoke tests prepared and run in staging (QA Lead)
- UX sign-off for any user-facing changes (UX Designer)

## Quality Gate — Release Readiness

Before any production deployment, the following must be confirmed by the named owner:

- [ ] **QA Lead:** All acceptance criteria verified; no open Critical/High defects
- [ ] **QA Lead:** Smoke tests passed on staging environment
- [ ] **DevOps Engineer:** CI pipeline passing (build, test, security scan)
- [ ] **DevOps Engineer:** Staging deployment verified and mirrors production config
- [ ] **DevOps Engineer:** Rollback plan documented and tested
- [ ] **Technical Writer:** Release notes complete and reviewed
- [ ] **PM:** Deployment window confirmed and stakeholders notified
- [ ] **PdM:** Feature sign-off for any major or breaking changes

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — PM + DevOps Engineer
- [ ] Backup or snapshot (if applicable) — DevOps Engineer
- [ ] Deploy to staging and run smoke tests — DevOps Engineer + QA Lead
- [ ] Release readiness quality gate passed (see above)
- [ ] Deploy to production (automated pipeline preferred) — DevOps Engineer
- [ ] Run post-deploy verifications — DevOps Engineer + QA Lead
- [ ] Announce release to stakeholders and support — PM + Technical Writer

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **DevOps Engineer** triggers incident response and notifies PM and on-call
  - **DevOps Engineer** rolls back to last known-good release if necessary
  - **PM** notifies stakeholders within 30 minutes of a critical incident
  - **QA Lead** assists in triage and validates the rollback state
  - **All:** Triage root cause and capture action items for post-incident retrospective

## Release Notes Template
- **Author:** Technical Writer (with input from Developers and QA Lead)
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
