# OctoAcme Project Management Docs

This folder contains the official documentation for OctoAcme's project management processes. These documents define how teams initiate, plan, execute, release, and continuously improve projects while maintaining consistent quality and communication standards across the organization.

## Summary of OctoAcme Project Management Processes

OctoAcme follows a structured project lifecycle: **Initiation → Planning → Execution → Release → Retrospective**. Projects begin with a One-pager that defines the problem statement, success metrics, and stakeholders. Once approved, the team kicks off planning to create a prioritized backlog with acceptance criteria, define the Definition of Done, and establish a release timeline. Execution follows an iterative approach with work tracked on a project board using columns (Backlog, Ready, In Progress, In Review, QA, Done). Pull requests should be small (≤400 lines), include issue links and acceptance criteria, pass CI checks, and require at least one approval before merging.

Key roles drive project success: **Project Managers (PM)** coordinate delivery, schedules, risks, and communications; **Product Managers (PdM)** define outcomes, prioritize the backlog, and measure success; **Developers** implement features, write tests, and participate in code reviews; **QA/Testing** validates quality and acceptance criteria; and **Stakeholders** provide inputs and approvals. Each project has clear ownership with a named PM and Product Lead.

Communication follows a defined cadence: daily standups (15 min) for progress and blockers, weekly delivery syncs for demos and risk updates, weekly PM–PdM alignment, and monthly stakeholder updates. Escalation paths move from team-level triage to PM to Product Lead to Sponsor. For security incidents, teams follow the security incident runbook and notify Security on-call.

Quality assurance is built into the workflow: unit tests for new logic, integration tests where applicable, and end-to-end smoke tests for critical flows before release. CI runs automated tests, linting, and security scanning. Releases require a deployment checklist (staging smoke tests, production deploy, post-deploy verification, rollback plan) and documented release notes. The rollback playbook ensures teams can quickly revert to a known-good state if issues arise.

## Documentation Index

- [Project Management Overview](./octoacme-project-management-overview.md) — Principles, lifecycle, and key artifacts
- [Project Initiation](./octoacme-project-initiation.md) — Validating and authorizing new projects
- [Project Planning](./octoacme-project-planning.md) — Backlog creation, estimation, and release planning
- [Execution & Tracking](./octoacme-execution-and-tracking.md) — Day-to-day workflows and PR conventions
- [Risks & Communication](./octoacme-risks-and-communication.md) — Risk management and stakeholder updates
- [Release & Deployment](./octoacme-release-and-deployment.md) — Release process and rollback playbook
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md) — Learning and iterating
- [Roles & Personas](./octoacme-roles-and-personas.md) — PM, PdM, Developers, QA responsibilities

## How to Use These Docs

- Keep the **Project One-pager** and **project README** updated in your project repository as the single source of truth for status and context.
- Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context for AI-assisted development.
- Reference these docs during onboarding, planning, and retrospectives to ensure consistent practices across teams.

## Acceptance Criteria

- [x] README created at `docs/README.md`
- [x] Short introductory paragraph describing the docs folder purpose
- [x] 3-4 paragraph summary covering workflows, personas, communication, and QA
- [x] Direct relative links to all documentation files
- [x] "How to use these docs" section with guidance on One-pager, README, and `.copilot/`
- [x] Acceptance criteria checklist included
