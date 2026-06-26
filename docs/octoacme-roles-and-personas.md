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

## QA / Testers

### Role Summary
QA / Testers validate that delivered work meets acceptance criteria, quality standards, and user expectations before release.

### Responsibilities
- Review acceptance criteria and define test cases
- Execute functional, regression, and exploratory tests
- Report, triage, and verify bug fixes
- Contribute to the Definition of Done
- Raise quality risks before release gates

### Goals
- Ensure releases are stable and meet agreed acceptance criteria
- Reduce escaped defects and production incidents
- Provide clear, actionable feedback to developers

### Typical Communication
- Sprint reviews and bug triage sessions
- Test summary reports and release sign-off
- Coordination with Developers on fix verification and edge cases

---

## Engineering Manager

### Role Summary
Engineering Managers lead engineering capacity, people management, and delivery health. They are the primary bridge between business commitments and team execution.

### Responsibilities
- Own team capacity planning, staffing trade-offs, and hiring decisions
- Support technical risk management and delivery predictability
- Coach Developers on quality standards, review practices, and growth
- Remove organizational blockers that prevent the team from delivering
- Represent the team in cross-functional planning forums

### Goals
- Sustain a healthy, high-performing team capable of consistent delivery
- Balance short-term delivery pressure with long-term technical quality
- Ensure the team has clarity on priorities and the resources to execute

### Typical Communication
- 1:1s with direct reports and escalation discussions with leadership
- Capacity and risk updates with Project Manager during planning
- Scope trade-off discussions with Product Manager when constraints change

#### Interaction with Existing Roles
- **Project Manager:** Partners on timeline feasibility, risk escalation, and resource constraints. The PM drives schedule; the Engineering Manager ensures the schedule reflects realistic capacity.
- **Product Manager:** Collaborates on scope trade-offs when capacity or technical risk changes priorities.
- **Developers:** Provides coaching, removes blockers, and ensures clear ownership of work items.
- **Tech Lead / Staff Engineer:** Delegates technical decision authority while retaining accountability for team health and delivery outcomes.

---

## Tech Lead / Staff Engineer

### Role Summary
Tech Leads and Staff Engineers provide technical direction and architecture guidance across initiatives. They translate product goals into sound technical approaches and ensure non-functional requirements are addressed.

### Responsibilities
- Define technical approach, architecture constraints, and integration strategy
- Drive technical decomposition and sequencing for the backlog
- Ensure non-functional requirements (reliability, security, performance) are addressed
- Lead design reviews and enforce coding standards
- Identify technical dependencies and surface them to the Project Manager

### Goals
- Deliver technically sound, maintainable solutions aligned with product goals
- Reduce rework by resolving architecture ambiguity before implementation
- Mentor Developers and raise the overall technical capability of the team

### Typical Communication
- Technical design docs and architecture decision records (ADRs)
- Design review sessions and async feedback on PRs
- Dependency and risk discussions with the Project Manager

#### Interaction with Existing Roles
- **Product Manager:** Translates desired outcomes into technical plans; flags when proposed scope carries hidden complexity or risk.
- **Project Manager:** Surfaces technical dependencies, integration risks, and milestone threats early so the PM can adjust plans proactively.
- **Developers:** Mentors on design patterns, reviews architectural decisions, and unblocks implementation challenges.
- **QA / Testers:** Partners on test strategy, especially for integration and non-functional testing.
- **DevOps / SRE:** Aligns on operability requirements, deployment strategy, and observability needs during design.

---

## UX Designer / Researcher

### Role Summary
UX Designers and Researchers ensure solutions are usable, validated, and aligned to user needs before and during implementation.

### Responsibilities
- Conduct lightweight discovery and usability validation
- Produce designs and specifications to reduce implementation ambiguity
- Define UX acceptance criteria collaboratively with product and engineering
- Maintain a shared design system or component library where applicable
- Advocate for accessibility and inclusive design standards

### Goals
- Reduce implementation rework caused by unclear or unvalidated design decisions
- Ensure delivered features meet user expectations and accessibility standards
- Create consistent, well-documented design handoffs

### Typical Communication
- Design reviews and prototype walkthroughs with the team
- Design specifications and annotated mockups shared with Developers
- Usability findings summaries shared with Product Manager

#### Interaction with Existing Roles
- **Product Manager:** Partners on problem framing and user validation; provides design evidence to inform prioritization decisions.
- **Developers:** Coordinates implementation-ready handoffs, clarifies design intent during build, and reviews delivered UI for fidelity.
- **QA / Testers:** Collaborates on usability acceptance checks and accessibility validation criteria.
- **Project Manager:** Flags design dependencies or discovery activities that may affect milestone timelines.

---

## DevOps / SRE

### Role Summary
DevOps Engineers and Site Reliability Engineers own deployment reliability, observability, and operational readiness. They ensure teams can ship safely and recover quickly from incidents.

### Responsibilities
- Maintain CI/CD health, deployment safety checks, and rollback readiness
- Define and monitor operational SLOs, alerts, and dashboards
- Support incident response, post-incident reviews, and improvement actions
- Enforce infrastructure security and compliance requirements
- Contribute to the release readiness checklist and go/no-go decisions

### Goals
- Enable frequent, low-risk deployments to production
- Minimize mean time to detection (MTTD) and recovery (MTTR)
- Maintain infrastructure reliability and operational visibility

### Typical Communication
- Release readiness reviews and deployment coordination with Project Manager
- Runbooks, deployment guides, and incident postmortems
- On-call rotation updates and SLO status reports shared with stakeholders

#### Interaction with Existing Roles
- **Project Manager:** Coordinates on release readiness checkpoints, deployment windows, and go/no-go criteria.
- **Developers:** Partners on operability requirements (logging, feature flags, graceful degradation) during implementation.
- **Tech Lead / Staff Engineer:** Aligns on infrastructure architecture and non-functional requirements early in design.
- **Stakeholders:** Provides status during incidents and communicates expected resolution timelines.

---

## Customer Support / Success Representative

### Role Summary
Customer Support and Success Representatives bring customer feedback loops into planning and release decisions. They ensure the team understands real-world impact and that releases are supportable.

### Responsibilities
- Surface recurring customer issues and impact signals to the product team
- Validate release readiness from a supportability and documentation perspective
- Contribute to rollout communication and known-issues documentation
- Provide QA and Developers with real-world edge cases and user scenarios
- Monitor support ticket trends post-release and escalate emerging patterns

### Goals
- Reduce customer-facing defects and support escalations caused by poor release communication
- Ensure the team prioritizes issues with the highest customer impact
- Improve product supportability and self-service documentation

### Typical Communication
- Customer issue trend summaries shared with Product Manager and Project Manager
- Participation in release readiness reviews to validate support materials
- Post-release monitoring reports and escalation summaries

#### Interaction with Existing Roles
- **Product Manager:** Feeds prioritized customer pain points and usage patterns into backlog decisions.
- **Project Manager:** Coordinates on stakeholder and customer communication plans for upcoming releases.
- **Developers and QA / Testers:** Provides real-world edge cases, customer-specific configurations, and reproduction scenarios.
- **DevOps / SRE:** Collaborates on incident communication and customer-impact assessments during outages.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

