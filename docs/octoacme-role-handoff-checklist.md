# OctoAcme — Role Handoff Checklist

Use this checklist whenever work is transitioning between roles or phases to ensure nothing is lost and the next owner has what they need to proceed without delay.

---

## Planning → Execution Handoff

**Handoff from:** Product Manager + Project Manager  
**Handoff to:** Developers, Tech Lead / Staff Engineer, UX Designer / Researcher

- [ ] Acceptance criteria written and reviewed for all sprint items
- [ ] Each backlog item has a named owner from the delivery team
- [ ] Dependencies identified and communicated to affected owners
- [ ] Design assets or specs linked from relevant tickets (if applicable)
- [ ] Definition of Done confirmed and visible to the team
- [ ] Blockers from the previous sprint are resolved or have a mitigation plan
- [ ] Technical risk items are logged and assigned to Tech Lead for review

---

## Design → Development Handoff

**Handoff from:** UX Designer / Researcher  
**Handoff to:** Developers

- [ ] Annotated mockups or prototypes are finalized and linked from the ticket
- [ ] UX acceptance criteria documented (including edge cases and error states)
- [ ] Accessibility requirements noted (contrast, keyboard navigation, ARIA)
- [ ] Open design questions or assumptions documented and decisions recorded
- [ ] Shared with Developers in a walkthrough session or async review
- [ ] QA / Testers have reviewed UX acceptance criteria before implementation starts

---

## Development → QA Handoff

**Handoff from:** Developers  
**Handoff to:** QA / Testers

- [ ] Feature is deployed to the agreed test environment
- [ ] PR is merged and CI is passing (no known build failures)
- [ ] Test notes included in the PR description or ticket comment (test steps, known edge cases, areas of risk)
- [ ] Any new environment configuration or feature flags documented
- [ ] Known limitations or deferred items noted and linked to follow-up tickets
- [ ] Developer is available to answer questions during the QA window

---

## QA → Release Handoff

**Handoff from:** QA / Testers  
**Handoff to:** Project Manager + DevOps / SRE

- [ ] All acceptance criteria verified and documented as passed
- [ ] Regression tests completed (automated and/or manual as required)
- [ ] Defects resolved or deferred — deferred items have follow-up tickets with priority set
- [ ] Known issues list drafted and shared with Customer Support / Success Rep
- [ ] Release sign-off provided in the project board or release tracking document
- [ ] Smoke test script reviewed and ready for post-deployment verification

---

## Release → Post-Release Handoff

**Handoff from:** Project Manager + DevOps / SRE  
**Handoff to:** Customer Support / Success Rep + All roles

- [ ] Release deployed and post-deploy verifications completed
- [ ] Release notes published and linked from the project board
- [ ] Customer-facing communication sent (if applicable)
- [ ] Known issues communicated to Customer Support / Success Rep
- [ ] Monitoring dashboards and alerts confirmed active for the new release
- [ ] On-call responsibilities confirmed and escalation contacts updated
- [ ] Retrospective scheduled with all contributing roles

---

## Escalation Handoff

**Use this when escalating a blocker or risk to the next level.**

- [ ] Blocker or risk clearly described in writing (ticket, doc, or message)
- [ ] Impact and urgency stated (who is affected, by when does it need resolution)
- [ ] Steps already taken to resolve at the current level documented
- [ ] Escalation recipient explicitly notified (not just tagged in a comment)
- [ ] Expected response timeline agreed upon (see escalation path in `octoacme-cross-role-interaction-map.md`)
- [ ] Outcome of the escalation documented and communicated back to the team

---

## Notes
- Handoffs do not replace communication — a completed checklist is a minimum, not a substitute for conversation when work is complex or ambiguous.
- If a checklist item cannot be completed, document the reason and get explicit sign-off from the receiving role before proceeding.
- These checklists should be referenced in the project board or sprint tracking tool at each phase transition.
