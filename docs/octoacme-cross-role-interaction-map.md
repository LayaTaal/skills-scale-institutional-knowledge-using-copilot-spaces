# OctoAcme — Cross-Role Interaction Map

## Purpose
Clarify decision boundaries, handoff expectations, and escalation paths across all OctoAcme roles so teams can collaborate without ambiguity about who owns what.

---

## Decision Boundaries and Ownership

| Decision | Primary Owner | Consulted | Informed |
|---|---|---|---|
| Business priority and backlog order | Product Manager | Stakeholders, Project Manager | Engineering Manager, Developers |
| Schedule, milestones, and delivery commitments | Project Manager | Engineering Manager, Tech Lead | Product Manager, Stakeholders |
| Technical approach and architecture | Tech Lead / Staff Engineer | Engineering Manager, Developers | Product Manager, Project Manager |
| Team capacity and staffing | Engineering Manager | Project Manager, Tech Lead | Product Manager |
| Design direction and UX acceptance | UX Designer / Researcher | Product Manager, Developers | QA / Testers |
| Deployment timing and release go/no-go | Project Manager + DevOps / SRE | Tech Lead, QA / Testers | All roles |
| Incident response and escalation | DevOps / SRE | Engineering Manager, Tech Lead | Project Manager, Stakeholders |
| Customer-impact prioritization | Product Manager | Customer Support / Success Rep | Project Manager |
| Quality and release sign-off | QA / Testers | Developers, DevOps / SRE | Project Manager, Product Manager |

> **Note:** "Primary Owner" means the role is accountable for the decision and documents the outcome. "Consulted" roles must be engaged before the decision is finalized. "Informed" roles receive the outcome but are not required to approve.

---

## Typical Handoffs by Lifecycle Phase

### 1. Initiation
| From | To | Handoff artifact |
|---|---|---|
| Product Manager | Project Manager | Approved problem statement and success metrics |
| Customer Support / Success Rep | Product Manager | Customer pain point summary and priority signals |
| Stakeholders | Product Manager | Business goals and constraints |

**Gate:** Project Manager confirms team availability and stakeholder alignment before moving to planning.

---

### 2. Planning
| From | To | Handoff artifact |
|---|---|---|
| Product Manager | Tech Lead / Staff Engineer | Outcome brief and prioritized feature list |
| Tech Lead / Staff Engineer | Project Manager | Technical dependency map and milestone risk log |
| UX Designer / Researcher | Product Manager + Developers | Discovery findings and design direction brief |
| Engineering Manager | Project Manager | Confirmed capacity and resource constraints |
| Project Manager | All | Sprint plan with acceptance criteria, owners, and milestones |

**Gate:** Project Manager confirms backlog is estimated, acceptance criteria exist, and dependencies are mapped.

---

### 3. Execution
| From | To | Handoff artifact |
|---|---|---|
| UX Designer / Researcher | Developers | Design specifications and annotated mockups |
| Developers | QA / Testers | Feature branch ready for testing with test notes |
| Tech Lead / Staff Engineer | Developers | Architecture guidance and PR review feedback |
| Developers | DevOps / SRE | Infrastructure and operability requirements |
| QA / Testers | Developers | Bug reports with reproduction steps and priority |

**Gate:** QA / Testers confirm all acceptance criteria are passing before a feature is marked Done.

---

### 4. Release
| From | To | Handoff artifact |
|---|---|---|
| QA / Testers | Project Manager | Release sign-off and known issues list |
| DevOps / SRE | Project Manager | Deployment readiness confirmation and rollback plan |
| Customer Support / Success Rep | Project Manager | Support readiness checklist and communication plan |
| Project Manager | All | Release announcement and deployment schedule |

**Gate:** Project Manager + DevOps / SRE confirm all pre-release requirements are met before production deployment.

---

### 5. Retrospective
| From | To | Handoff artifact |
|---|---|---|
| All roles | Project Manager | Retrospective input (what worked, what didn't, action items) |
| Customer Support / Success Rep | Product Manager | Post-release support ticket trends and customer feedback |
| DevOps / SRE | Tech Lead | Post-incident review findings and infrastructure improvements |
| Project Manager | All | Action item log with owners and due dates |

**Gate:** Action items are assigned before the retrospective closes.

---

## Escalation Path Summary

This escalation path aligns with the risk management guidance in `octoacme-risks-and-communication.md`.

| Level | Trigger | Who acts | Expected response |
|---|---|---|---|
| **1 — Team triage** | Blocker or risk identified in standup or PR review | Developer, QA, or Tech Lead raises in daily sync | Same day: acknowledge and assign owner |
| **2 — PM / Product escalation** | Blocker unresolved after 1 day, scope conflict, or missed milestone risk | Project Manager or Product Manager escalates | Within 24 h: decision or mitigation plan documented |
| **3 — Engineering Manager escalation** | Resource constraint, cross-team dependency, or team conflict | Engineering Manager engages with Project Manager | Within 48 h: capacity or resourcing decision |
| **4 — Sponsor / leadership escalation** | Business-critical blocker, budget impact, or external dependency | Project Manager escalates with written summary | As needed: sponsor decision or priority override |

> For incident escalations specifically, the DevOps / SRE team owns the incident response flow. Project Manager coordinates stakeholder communication throughout.

---

## Quick Reference: Who to Contact

| Need | Contact |
|---|---|
| Change the priority or scope of work | Product Manager |
| Adjust a timeline or milestone | Project Manager |
| Technical design or architecture question | Tech Lead / Staff Engineer |
| Team capacity or staffing concern | Engineering Manager |
| Design clarification or spec question | UX Designer / Researcher |
| Deployment, rollback, or operational issue | DevOps / SRE |
| Customer feedback or support escalation | Customer Support / Success Rep |
| Quality or acceptance criteria question | QA / Testers |
