# OctoAcme — Release & Deployment Guide

## Purpose
Standardize how OctoAcme releases features to production to reduce risk and improve observability.

## Release Types
- Patch: hotfixes addressing critical production issues
- Minor: incremental features and improvements
- Major: significant functionality or breaking changes

## Pre-release requirements
- All acceptance criteria met and PRs merged
- **QA/Testing Lead** has provided written release sign-off
- Passing CI and security scans (verified by **DevOps Engineer**)
- Release notes drafted
- Rollback / mitigation plan documented
- Smoke tests prepared (owned by **QA/Testing Lead** and **DevOps Engineer**)

## Deployment Checklist
- [ ] Deployment window scheduled (if needed) — confirmed by **Project Manager** and **DevOps Engineer**
- [ ] Backup or snapshot (if applicable) — owned by **DevOps Engineer**
- [ ] Deploy to staging and run smoke tests — executed by **DevOps Engineer**, verified by **QA/Testing Lead**
- [ ] Deploy to production (automated pipeline preferred) — owned by **DevOps Engineer**
- [ ] Run post-deploy verifications — **QA/Testing Lead** confirms critical flows
- [ ] Announce release to stakeholders and support

## Rollback & Incident Playbook
- If a deployment fails or causes a critical issue:
  - **DevOps Engineer** triggers incident response and notifies on-call
  - Rollback to last known-good release if necessary (executed by **DevOps Engineer**)
  - **QA/Testing Lead** validates system stability after rollback
  - Triage root cause and capture action items

## Release Notes Template
- Release name / number:
- Date:
- Summary:
- Notable changes:
- Migration steps (if any):
- Known issues:
