# OctoAcme Project Management Docs

This folder contains OctoAcme's program- and project-management process documents. The goal is to centralize guidance so new team members and contributors can quickly find how we initiate, plan, execute, release, and continuously improve work.

## Brief project management processes summary

OctoAcme runs projects with a lightweight, outcome-focused lifecycle that moves from a clear initiation step into planning, execution, release, and continuous improvement. At initiation the team uses a Project One‑pager to capture the problem statement, measurable objectives, primary stakeholders, success metrics, and a high‑level timeline; a simple decision gate (clear metrics, stakeholder alignment, team availability) moves work into planning.

Planning breaks approved initiatives into a prioritized backlog with acceptance criteria, estimates, a Definition of Done, and an initial risk register so work can be pulled into timeboxed sprints or iterations with agreed capacity and release milestones. Day‑to‑day execution is organized around a predictable team rhythm (short daily standups, weekly delivery syncs, sprint demos) and a project board workflow that tracks items from Backlog → Ready → In Progress → In Review → QA → Done.

Roles and responsibilities are clearly defined so people know ownership and communication expectations: Product Managers set outcomes and prioritize the backlog; Project Managers coordinate schedules, risks, and stakeholder communication; Developers implement with tests and documentation; QA validates acceptance criteria and feature quality. Communication cadence includes weekly PM/PdM syncs, regular team standups, and monthly stakeholder updates, with templates for status and incident communications to keep stakeholders aligned.

Quality assurance and release practices are integrated with the workflow: unit, integration, and smoke tests (plus security scanning) run in CI; manual QA is used for acceptance when needed; and releases follow a checklist (pre-release checks, staging verification, rollback plan, post-deploy checks). Retrospectives and tracked action items close the loop on continuous improvement.

## Links to process docs

- [Project Management Overview](docs/octoacme-project-management-overview.md)
- [Project Initiation](docs/octoacme-project-initiation.md)
- [Project Planning](docs/octoacme-project-planning.md)
- [Execution and Tracking](docs/octoacme-execution-and-tracking.md)
- [Risks and Communication](docs/octoacme-risks-and-communication.md)
- [Release and Deployment](docs/octoacme-release-and-deployment.md)
- [Retrospective and Continuous Improvement](docs/octoacme-retrospective-and-continuous-improvement.md)
- [Roles and Personas](docs/octoacme-roles-and-personas.md)

## How to contribute

To add or update a process doc, open an issue using the "Add Content to Project Management Process Docs" template (in .github/ISSUE_TEMPLATE/) and reference the document to update. Once the change is proposed, follow the repo's PR and review process so changes are reviewed and merged.

## Acceptance criteria (example)

- [ ] Content aligns with existing process docs
- [ ] Update improves clarity or closes a documented gap
- [ ] Proposed content has been reviewed with stakeholders (if needed)
