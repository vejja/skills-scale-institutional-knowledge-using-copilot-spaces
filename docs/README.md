# OctoAcme Project Management Docs

This directory contains OctoAcme's project management process documentation. The files here capture how we initiate, plan, execute, release, and improve projects so teams can onboard quickly, run work consistently, and preserve institutional knowledge.

OctoAcme runs work through a lightweight lifecycle: Initiation (a Project One‑pager to capture problem, success metrics, stakeholders), Planning (kickoff, prioritized backlog with acceptance criteria, Definition of Done, and a release/milestone map), Execution (project board-driven workflow and PR-driven delivery), Release (checklists, smoke tests, rollback/incident playbook), and Retrospective (capture learnings and create action items). The canonical project board flow is Backlog → Ready → In Progress → In Review → QA → Done, and PRs should be small, link the related issue, include acceptance criteria, and pass CI checks and required approvals before merging.

Roles and responsibilities are explicit to ensure clear ownership: Product Managers (PdM) define outcomes and prioritize the backlog; Project Managers (PM) coordinate schedules, manage risks and dependencies, and drive communications; Developers implement and test changes; QA validates acceptance criteria and performs manual or automated checks; Stakeholders provide input and approvals. These persona definitions help with handoffs, escalation, and assigning retrospective action items.

Communication is structured with a predictable cadence: daily standups for team progress and blockers, weekly delivery/PM↔PdM syncs to surface status and risks, demos/reviews at the end of sprints or major milestones, and monthly stakeholder updates. Quality assurance is enforced through unit and integration tests, end-to-end smoke tests for critical flows, CI-run linting and security scans, and a deployment checklist with post-deploy verifications and rollback procedures. Retrospectives capture action items that are tracked back into the backlog with owners and due dates to close the improvement loop.

## Docs in this directory
- [Project Management Overview](./octoacme-project-management-overview.md)
- [Project Initiation Guide](./octoacme-project-initiation.md)
- [Project Planning](./octoacme-project-planning.md)
- [Execution & Tracking](./octoacme-execution-and-tracking.md)
- [Risk Management & Communication](./octoacme-risks-and-communication.md)
- [Release & Deployment Guide](./octoacme-release-and-deployment.md)
- [Retrospective & Continuous Improvement](./octoacme-retrospective-and-continuous-improvement.md)
- [Roles & Personas](./octoacme-roles-and-personas.md)

## How to use these docs
- Keep the Project One‑pager and the project README updated in the project repository as the single source of truth for status, milestones, and owner contact info.
- Add process-specific or team-specific docs into `.copilot/` (or equivalent) if you want Copilot Spaces and similar tools to use them as context.
- When proposing doc updates, use the issue template at `.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml` to ensure consistent review and acceptance.

## Acceptance criteria (from issue #2)
- [ ] Content aligns with existing process docs
- [ ] Update improves clarity or closes a documented gap
- [ ] Proposed content has been reviewed with stakeholders (if needed)
