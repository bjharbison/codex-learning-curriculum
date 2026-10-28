# 10-Minute Demo Playbook — Human + AI Cyber Defense

**Audience:** security leaders, government executives, and small defender teams.

**Working title:** *Where AI helps government cyber defenders—and where human judgment stays.*

**Goal:** Show a believable workflow for discovering, validating, prioritizing and fixing one security issue, using an owned sample repository and synthetic data. Demonstrate with ordinary Codex until Daybreak Blue approval is confirmed; do not imply you have access before then.

## Narrative and timing

| Time | Story beat | Visual or action | Core message |
| --- | --- | --- | --- |
| 0:00–1:00 | Small team, large backlog | Show synthetic backlog (e.g., 25 fabricated findings) | Limited staff need better triage, not uncritical automation |
| 1:00–2:30 | Establish scope | Show owned repo, explicit authorized scope and threat model | AI operates within boundaries |
| 2:30–4:00 | Triage | Have Codex analyze a sample finding with code references | AI accelerates investigation and makes assumptions visible |
| 4:00–5:30 | Validate and prioritize | Show reproduction evidence, false positive, CVSS/EPSS context | Human analysts distinguish urgency from numerical scores |
| 5:30–7:00 | Fix and test | Review branch diff and regression test result | AI suggests a patch; tests and review determine acceptance |
| 7:00–8:30 | Human checkpoints | Highlight authorization, approval, residual risks and rollback | Human remains accountable |
| 8:30–10:00 | Adoption takeaway | Show a repeatable checklist and next steps | A small team can start with one bounded workflow |

## Prepare the demonstration

1. Choose a non-sensitive repo you own; maintain a known-good commit and a separate demo branch.
2. Generate synthetic findings; mark them as fictional on the slide/screen.
3. Pre-record or screenshot one clean validated walkthrough as fallback to live tool latency or failures.
4. Show *before/after* tests without hiding failed runs or inventing outcomes.
5. Avoid live unapproved network scanning, active exploitation or production changes.
6. If showing Daybreak Blue, confirm approval and product availability. Otherwise label the tool **standard Codex**.
7. Rehearse aloud; aim for 9 minutes of presentation and 1 minute of contingency.

## Audience-specific explanations

- **Authorizing official:** Show the authorization boundary, approved data handling and auditable human approval.
- **CISO:** Show risk ranking, controls alignment, confidence and residual exposure.
- **Operator:** Show file locations, evidence, false positives, detection and regression testing.
- **Developer:** Show exact diff, tests, pull request and rollback plan.
- **Executive:** Show before/after analyst workflow and clearly distinguish example metrics from measured results.

## Assessment rubric

- [ ] Security problem and authorization scope clear in 60 seconds
- [ ] One finding supported by verifiable evidence
- [ ] At least one AI error, assumption or false positive discussed
- [ ] Demonstrates a reviewable patch and validation test
- [ ] Explains why the human made the final decision
- [ ] Uses terminology appropriate to non-specialists
- [ ] Finishes within ten minutes
- [ ] Contains no restricted or workplace material

## Outputs

- `demo/outline.md` — speaking notes
- `demo/fixtures/` — synthetic examples (separate from production)
- `demo/decision-log.md` — human approval and rejected AI suggestions
- `demo/validation.md` — tests, limitations and links to sanitized artifacts

After delivering, note what a beginner, an analyst, and an executive each misunderstood. Update the demo accordingly.
