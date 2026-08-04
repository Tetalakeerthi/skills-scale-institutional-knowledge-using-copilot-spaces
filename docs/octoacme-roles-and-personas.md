# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

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

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

---

## Added Cross-functional & Operational Personas (proposed)

The following personas clarify ownership, handoffs, and escalation points across the project lifecycle. Each includes responsibilities, typical involvement points (initiation/planning/execution/release/incident), and how they interact with core roles.

### Release Manager

Responsibilities:
- Owns release coordination and scheduling.
- Maintains and verifies the pre-release checklist and runbook.
- Confirms rollback/mitigation plans and deployment windows.
- Coordinates CI/CD, staging validation, and on-call notification.

Typical involvement:
- Planning: validate release timeline and dependencies.
- Execution/Release: coordinate deployments, run smoke tests, confirm signoffs.
- Incident: coordinate rollback and post-incident release fixes.

Interactions:
- PM: align on release timing and stakeholder communication.
- Developers: ensure deployment artifacts and feature toggles are ready.
- QA: confirm release acceptance criteria and smoke test results.
- Support/On-call: ensure monitoring and alerting are in place for post-release.

Success signals:
- Smooth automated deployments, minimal rollbacks, clear post-release verification.

---

### Engineering Manager (EM)

Responsibilities:
- Ensure technical capacity and staffing for delivery.
- Resolve cross-team technical dependencies and escalate when required.
- Coordinate architecture and non-functional requirement decisions.
- Support performance and career topics for engineering team members.

Typical involvement:
- Initiation/Planning: validate resource estimates and help prioritize technical work.
- Execution: unblock technical issues and coordinate cross-team efforts.
- Retrospective: ensure learning and improvements are captured and resourced.

Interactions:
- PM/PdM: discuss resourcing trade-offs and priority changes.
- Developers: provide technical guidance and escalations.
- Product Lead: escalate cross-team impacts or strategic technical concerns.

Success signals:
- Reduced cross-team delays, balanced capacity, timely delivery of technical enablers.

---

### Support Lead / Customer Ops Liaison

Responsibilities:
- Owns day-to-day liaison with Customer Support/Operations.
- Triage and prioritize customer-reported issues and bug reports.
- Define SLA expectations and support-to-engineering handoff processes.
- Maintain runbooks for common support flows.

Typical involvement:
- Execution/Incident: provide triage, reproduce issues, and escalate to engineering.
- Release: prepare support notes and known issues lists.
- Post-release: monitor customer reports and coordinate hotfixes.

Interactions:
- PM: escalate high-impact customer issues and receive prioritization decisions.
- Developers: pass prioritized technical tickets and reproduction steps.
- QA: request urgent validation for fixes impacting customers.

Success signals:
- Faster triage-to-fix cycle, improved customer communication, lower SLA breaches.

---

### UX Researcher / Design Lead

Responsibilities:
- Validate product decisions through user research and testing.
- Provide design acceptance criteria and interaction guidance.
- Ensure usability considerations are captured in acceptance criteria.

Typical involvement:
- Initiation/Planning: contribute user insights and define usability goals.
- Execution: review designs and implementation for fidelity to UX intent.
- Release: validate key user flows and acceptance metrics.

Interactions:
- PdM: align on user research plans and product hypotheses.
- Developers: clarify UI/UX implementation details and edge-case behavior.
- QA: advise on usability test cases to include in acceptance checks.

Success signals:
- Increased usability scores, fewer UI regressions, alignment between design and delivery.

---

### Data Analyst / Metrics Owner

Responsibilities:
- Define success metrics and instrumentation requirements.
- Create dashboards and validate telemetry for feature rollouts.
- Analyze post-release impact and validate hypotheses.

Typical involvement:
- Planning: define measurement plan and identify necessary events/metrics.
- Execution: validate telemetry implementation and data quality.
- Post-release: analyze impact and recommend next steps.

Interactions:
- PdM: co-design success metrics and target outcomes.
- Developers: specify event schemas and verify instrumentation.
- PM: report on metric-driven status during weekly syncs.

Success signals:
- Reliable telemetry, clear adoption/impact data, evidence-based product decisions.

---

### Security Liaison

Responsibilities:
- Review security implications during design and planning.
- Coordinate static/dynamic security scans and approvers.
- Track security findings and ensure remediation plans are followed.

Typical involvement:
- Planning: review high-risk features and required threat modeling.
- Execution: confirm scans run and findings are tracked.
- Release/Incident: verify no outstanding critical security issues before release; collaborate on incident response if security incidents occur.

Interactions:
- Developers: provide remediation guidance and validate fixes.
- PM/EM: escalate security risks if they affect release decisions.
- On-call/Security Ops: coordinate during incidents and post-incident reviews.

Success signals:
- No critical unremediated vulnerabilities at release time; timely remediation of findings.

---

## Handoff & Interaction Guidance (summary)

For each key handoff, teams should document:
- What outputs are required (e.g., runbook, telemetry, release notes).
- Who must sign off (e.g., Release Manager, QA, Data Analyst).
- Expected SLAs for response and escalation (e.g., triage within X hours).

Examples:
- Release handoff: Developers -> Release Manager -> QA -> Support Lead (includes deployment artifacts, smoke test results, release notes).
- Incident handoff: Support Lead -> Developers -> Security Liaison -> PM (includes incident summary, impact, next steps).

---

## Templates & Where to Add Them

Add short references/links in this doc to:
- docs/release-checklist.md (pre-release checklist and runbook template)
- docs/metrics-and-instrumentation.md (measurement plan template)
- docs/role-handoffs.md (standardized handoff checklist)

These files should live in docs/ and be kept minimal, practical checklists that teams can copy into project READMEs.
