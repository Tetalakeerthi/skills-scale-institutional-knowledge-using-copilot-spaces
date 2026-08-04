# Release & Pre-deployment Checklist (template)

Purpose: Lightweight checklist the Release Manager / PM uses to verify readiness.

Release name / number:
Date:
Owner (Release Manager):

Pre-release
- [ ] All PRs merged for this release and linked to issues
- [ ] CI green and required checks passed
- [ ] Security scan results reviewed and critical findings resolved
- [ ] Data instrumentation for success metrics implemented and verified
- [ ] Rollback/mitigation plan documented
- [ ] Release notes drafted and reviewed (include known issues)
- [ ] Stakeholders (support, on-call, product) notified of release window
- [ ] Runbook / post-deploy verification steps documented

Staging Validation
- [ ] Deploy to staging completed
- [ ] Smoke tests executed and passed
- [ ] Key metrics dashboards show expected baseline
- [ ] QA (if required) has signed off

Production Deployment
- [ ] Backup/snapshot taken if applicable
- [ ] Production deploy executed
- [ ] Post-deploy smoke tests run
- [ ] Monitoring/alerts validated
- [ ] Support/on-call notified of successful deployment

Post-release
- [ ] Monitor metrics for X hours/days (as appropriate)
- [ ] Validate success metrics with Data Analyst
- [ ] Capture post-release notes & actions in the project board
