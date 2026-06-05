# OctoAcme Project Management Docs

Welcome to the OctoAcme Project Management documentation! This README summarizes the lifecycle, roles, and core processes for how OctoAcme delivers projects. Use the links below to access detailed guidance for each stage of project work.

## Project Management Processes (Summary)

OctoAcme delivers value through **customer-first, iterative, and collaborative practices**. Our approach is grounded in clear ownership, data-informed decisions, and a strong commitment to continuous improvement. Teams work together across five distinct lifecycle phases, with well-defined roles ensuring accountability and transparency at every stage.

### Core Principles
- **Customer-first**: Prioritize customer value and usability in all decisions
- **Iterative delivery**: Deliver small, testable increments rather than monolithic releases
- **Clear ownership**: Each project has a named Project Manager (PM) and Product Lead
- **Data-informed decisions**: Measure impact and iterate based on evidence
- **Psychological safety**: Encourage feedback, learning, and blameless retrospectives

### Key Roles
- **Project Manager**: Coordinates delivery, manages schedules, risks, and communications
- **Product Manager**: Defines outcomes, prioritizes the backlog, and measures success
- **Developers**: Implement features, collaborate on design, and identify technical risks
- **QA/Testing**: Validate quality and ensure acceptance criteria are met
- **Stakeholders**: Provide inputs, approvals, and strategic guidance

### Project Lifecycle

OctoAcme follows a structured five-phase lifecycle to move deliberately from problem validation through continuous improvement:

1. **Initiation**: Validate business need through a lightweight One-pager, identify stakeholders, confirm high-level timeline, and decide go/no-go for planning. Success criteria and measurable outcomes must be clear before moving forward.

2. **Planning**: Break work into shippable increments with prioritized backlogs, acceptance criteria, and effort estimates. Define the Definition of Done, identify cross-team dependencies, and map milestones and release points.

3. **Execution & Tracking**: Deliver using daily standups (15 min), sprint-based iteration, and clear PR workflows. Automated CI tests and linting run before review; code reviews are mandatory; quality gates include unit tests, integration tests, and security scanning.

4. **Release & Deployment**: Standardize release procedures with pre-release requirements (acceptance criteria met, CI passing, release notes drafted, rollback plan documented). Deploy to staging for smoke tests, then to production via automated pipeline when possible. Post-deploy verification ensures stability.

5. **Risk Management & Communication**: Maintain a Risk Register (ID, description, impact, likelihood, owner, mitigation) reviewed weekly. Use a three-level escalation path (team → PM → Product Lead → Sponsor) for blockers. Provide regular stakeholder updates (weekly or milestone-based) and follow blameless incident retrospectives.

6. **Retrospective & Continuous Improvement**: After each sprint, release, or milestone, the team reflects on what went well, what could improve, and commits to 2–3 actionable items with clear owners and timelines. Track improvements and celebrate wins to reinforce a culture of learning.

### Communication Cadence
- **Daily standups**: 15 minutes; focus on progress, blockers, dependencies
- **Weekly PM-PdM sync**: Alignment and priority adjustments
- **Twice-weekly delivery team standups** (or as agreed): Sprint planning and execution updates
- **Monthly stakeholder updates**: High-level progress and risks
- **Ad-hoc escalations**: When blockers require immediate attention

### Quality & Testing Standards
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI pipeline
- Manual QA for feature acceptance when needed
- Small PRs (≤400 lines when possible) with automated checks before review
- At least one approval required before merging (or team-defined policy)

---

## Process Documents

Dive into detailed guidance for each lifecycle phase using the links below:

| Document | Purpose |
|----------|---------|
| [Project Management Overview](octoacme-project-management-overview.md) | Concise introduction to OctoAcme's approach, roles, and key artifacts |
| [Project Initiation Guide](octoacme-project-initiation.md) | Validate business need, align stakeholders, and confirm go/no-go decision |
| [Project Planning](octoacme-project-planning.md) | Break work into increments, estimate scope, and define release milestones |
| [Execution & Tracking](octoacme-execution-and-tracking.md) | Day-to-day delivery workflows, team rhythm, and progress tracking |
| [Risks & Communication](octoacme-risks-and-communication.md) | Risk register, escalation paths, and stakeholder communication templates |
| [Release & Deployment](octoacme-release-and-deployment.md) | Pre-release requirements, deployment checklists, and rollback procedures |
| [Retrospective & Continuous Improvement](octoacme-retrospective-and-continuous-improvement.md) | Running effective retrospectives and tracking action items |
| [Roles & Personas](octoacme-roles-and-personas.md) | Detailed definitions of Developer, Product Manager, and Project Manager roles |

---

## How to Use These Docs

- **New to OctoAcme?** Start with [Project Management Overview](octoacme-project-management-overview.md) for a quick orientation.
- **Starting a new project?** Follow the [Project Initiation Guide](octoacme-project-initiation.md), then move to [Project Planning](octoacme-project-planning.md).
- **In execution mode?** Reference [Execution & Tracking](octoacme-execution-and-tracking.md) and [Risks & Communication](octoacme-risks-and-communication.md).
- **Preparing a release?** Use the [Release & Deployment](octoacme-release-and-deployment.md) guide and checklist.
- **Improving the process?** Open an issue using the [Add Content to Process Docs](../.github/ISSUE_TEMPLATE/add-update-content-to-process-docs.yml) template.

Keep the Project Charter updated in your project repo. Add process-specific docs into `.copilot/` if you want Copilot Spaces to use them as context for your team.
