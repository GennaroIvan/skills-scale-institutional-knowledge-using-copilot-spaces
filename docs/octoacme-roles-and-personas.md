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

## QA/Testing Lead

### Role Summary
The QA/Testing Lead owns test strategy, coordinates quality assurance activities, validates acceptance criteria, and champions test automation across projects.

### Responsibilities
- Define and maintain the test strategy, test plans, and acceptance criteria validation
- Design, implement, and maintain automated test suites (unit, integration, end-to-end)
- Coordinate manual QA for feature acceptance and exploratory testing
- Review acceptance criteria with Product Managers before sprint start
- Sign off on release readiness and own the QA column on the project board
- Report defect trends and quality metrics to the Project Manager

### Goals
- Ensure every release meets the agreed Definition of Done quality bar
- Reduce regression risk through comprehensive automated coverage
- Shift quality left by embedding testing earlier in the development cycle

### Typical Communication
- Sprint planning: review acceptance criteria and flag ambiguities with Developers and Product Managers
- Daily standups: surface blocking defects and QA environment issues
- Pre-release sign-off: written QA sign-off document shared with Project Manager and Product Manager
- Defect reports and test result summaries in the project board

### Interactions with Other Roles
- **Developers**: pair on writing unit and integration tests; review PR test coverage; triage defects together
- **Product Managers**: align on acceptance criteria; clarify edge cases and out-of-scope scenarios
- **Project Managers**: report QA status and test progress; flag risks that may affect release readiness
- **DevOps Engineer**: coordinate CI/CD pipeline test stages and test environment provisioning
- **Scrum Master/Agile Facilitator**: raise process impediments that slow QA cycles in retrospectives

### Cross-References
- See `octoacme-execution-and-tracking.md` for the QA column in the project board workflow and quality testing practices
- See `octoacme-project-planning.md` for the initial test plan / QA approach checklist item
- See `octoacme-release-and-deployment.md` for smoke test and release readiness requirements

---

## UX Designer

### Role Summary
The UX Designer leads user research, creates wireframes and prototypes, and validates designs through usability testing to ensure features meet user needs.

### Responsibilities
- Conduct user research (interviews, surveys, usability studies) to inform product decisions
- Produce wireframes, mockups, and interactive prototypes for planned features
- Collaborate with Product Managers to translate requirements into user flows and interface designs
- Run usability tests and synthesize findings for the team
- Maintain and evolve the design system and UX standards
- Provide design review feedback on implemented features before release

### Goals
- Deliver intuitive, accessible, and delightful user experiences
- Reduce rework by validating design decisions early and iteratively
- Align product and engineering on user needs and interaction patterns

### Typical Communication
- Discovery and design reviews with Product Managers and Developers during planning
- Design handoff notes and annotated mockups shared in the project repository or design tool
- Usability test reports distributed to Product Managers and Project Managers
- Participation in sprint demos to assess implemented designs against intent

### Interactions with Other Roles
- **Developers**: provide design specs and assets; clarify interaction details during implementation; review built features against designs
- **Product Managers**: collaborate on user stories and acceptance criteria; inform prioritization with research insights
- **Project Managers**: communicate design timeline dependencies and flag scope risks related to UX work
- **QA/Testing Lead**: provide usability acceptance criteria; support accessibility and UI regression test definitions
- **Business Analyst**: share user research findings to validate business requirements from a user perspective

### Cross-References
- See `octoacme-project-planning.md` for incorporating UX design tasks into the backlog and sprint planning
- See `octoacme-execution-and-tracking.md` for design review as part of the PR and QA workflow

---

## Business Analyst

### Role Summary
The Business Analyst bridges business requirements and technical implementation, conducting requirements gathering, stakeholder liaison, and business case analysis to ensure solutions deliver measurable value.

### Responsibilities
- Elicit, document, and manage business and functional requirements
- Translate stakeholder needs into clear user stories and acceptance criteria
- Conduct gap analysis between current and desired states
- Maintain the requirements traceability matrix linking business goals to deliverables
- Facilitate requirement review sessions and sign-off with stakeholders
- Support change management by assessing the impact of scope changes

### Goals
- Ensure delivered solutions address the underlying business problem
- Reduce ambiguity and rework by producing clear, agreed-upon requirements upfront
- Provide stakeholders with confidence that their needs are captured and prioritized

### Typical Communication
- Requirements workshops with stakeholders, Product Managers, and Developers during initiation and planning
- Written requirements documents, user stories, and process flow diagrams shared in the project repository
- Change request assessments and impact analyses presented to Project Managers
- Regular status updates to business stakeholders on requirements coverage

### Interactions with Other Roles
- **Developers**: clarify functional requirements and answer implementation questions; validate that delivered functionality matches requirements
- **Product Managers**: collaborate on backlog prioritization; provide business context for trade-off decisions
- **Project Managers**: flag scope changes and dependency risks; support risk register with business impact assessments
- **UX Designer**: share stakeholder requirements to inform user research and design direction
- **Scrum Master/Agile Facilitator**: support backlog refinement by ensuring stories meet acceptance criteria standards

### Cross-References
- See `octoacme-project-planning.md` for requirements-gathering activities during planning and backlog creation
- See `octoacme-risks-and-communication.md` for stakeholder communication and escalation paths

---

## DevOps Engineer

### Role Summary
The DevOps Engineer owns the CI/CD pipeline, infrastructure provisioning, deployment automation, and production monitoring to enable fast, reliable, and repeatable releases.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines and build automation
- Provision and manage infrastructure for development, staging, and production environments
- Implement and maintain deployment automation and release tooling
- Set up and monitor observability tooling (logging, metrics, alerting)
- Enforce security scanning and compliance checks in the pipeline
- Support incident response and lead post-incident infrastructure reviews

### Goals
- Enable the team to deploy safely and frequently with minimal manual intervention
- Maintain high availability and performance in production environments
- Reduce mean time to recovery (MTTR) through robust monitoring and rollback capabilities

### Typical Communication
- Sprint planning: surface infrastructure dependencies and pipeline changes needed for upcoming features
- Daily standups: report on environment health, pipeline failures, and deployment status
- Release coordination: confirm deployment readiness with Project Manager and QA/Testing Lead before each release
- Incident reports and post-mortems shared with the full delivery team

### Interactions with Other Roles
- **Developers**: support local development environment setup; review infrastructure-as-code changes; align on build and deployment tooling
- **Project Managers**: communicate infrastructure timelines and deployment window requirements; flag environment risks
- **QA/Testing Lead**: provision and maintain QA and staging environments; integrate automated tests into the CI pipeline
- **Product Managers**: advise on release cadence feasibility and feature flag strategies
- **Scrum Master/Agile Facilitator**: raise pipeline or environment impediments in retrospectives for process improvement

### Cross-References
- See `octoacme-execution-and-tracking.md` for CI standards, PR workflow, and pipeline quality gates
- See `octoacme-release-and-deployment.md` for deployment checklist, rollback playbook, and release types
- See `octoacme-risks-and-communication.md` for incident communication and escalation paths

---

## Scrum Master/Agile Facilitator

### Role Summary
The Scrum Master/Agile Facilitator enables effective agile practices by facilitating ceremonies, removing blockers, coaching the team on process adherence, and fostering a culture of continuous improvement.

### Responsibilities
- Facilitate all agile ceremonies: sprint planning, daily standups, sprint reviews, and retrospectives
- Identify and remove blockers and impediments that slow the team
- Coach the team and organization on agile principles and practices
- Protect the team from unplanned interruptions and scope changes mid-sprint
- Track and communicate team velocity, capacity, and process health
- Support the Project Manager in scheduling and structuring delivery rhythms

### Goals
- Enable the team to deliver predictably and continuously improve
- Create a safe environment for open feedback and experimentation
- Minimize waste and maximize flow through the delivery pipeline

### Typical Communication
- Daily standups: surface blockers and action them promptly
- Sprint retrospectives: facilitate structured improvement discussions and track action items
- Team health check-ins: periodic pulse surveys or one-on-ones to gauge morale and process friction
- Status summaries on team impediments shared with Project Managers as needed

### Interactions with Other Roles
- **Developers**: shield from process overhead; facilitate estimation and planning; help resolve interpersonal or process conflicts
- **Project Managers**: align ceremony schedules with broader project milestones; surface team-level risks and impediments
- **Product Managers**: facilitate backlog refinement; help prioritize stories to ensure sprint goals are achievable
- **QA/Testing Lead**: ensure QA activities are included in sprint capacity and Definition of Done
- **Business Analyst**: support story readiness reviews to confirm acceptance criteria clarity before sprint start

### Cross-References
- See `octoacme-execution-and-tracking.md` for team rhythm, blocker escalation, and project board workflow
- See `octoacme-project-planning.md` for sprint/iteration planning and Definition of Done practices
- See `octoacme-retrospective-and-continuous-improvement.md` for retrospective facilitation and improvement tracking

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

