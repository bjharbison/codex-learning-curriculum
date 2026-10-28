# Defensive Cybersecurity Skills — Hands-On Track

**Objective:** independently explain, demonstrate, and validate a human-supervised AI security workflow. Begin with standard Codex; use Daybreak Blue only when your access is approved and the work is in scope.

**Safe environment:** your own public/open-source application or deliberately vulnerable training app with local fixtures. Keep real secrets, customer data, government systems, and employer data out of this lab.

## The defender lifecycle

| Stage | What to learn | Hands-on deliverable | Evidence to retain |
| --- | --- | --- | --- |
| 1. Threat model | Assets, trust boundaries, attack surface, likely abuse | `security/threat-model.md` | Diagram, assumptions, prioritized risks |
| 2. Discover | Static analysis, dependency alerts, code review | Findings backlog | Tool/version, file/line reference, reproduction notes |
| 3. Validate | Reproduction, impact, false positive detection | Validated finding record | Test evidence and scope limitations |
| 4. Prioritize | Severity versus risk; CVSS and EPSS; exposure and asset importance | Risk-ranked list | Document why priority differs from raw score |
| 5. Remediate | Smallest safe fix; code review; dependency patches | Isolated branch and PR | Diff, rationale, review comments |
| 6. Verify | Regression tests, smoke checks and residual risk | Verification report | Commands/results, negative tests, open risks |
| 7. Detect | Logging, signals, alert definitions, false positives | Example defensive detection | Sample synthetic logs and expected matches |
| 8. Respond and recover | Triage, containment planning, communications, recovery criteria | Tabletop runbook | Human decisions, approvals, recovery tests |

## Rapid sequence: five labs

### Lab 1 — Threat model (45–60 min)
- Select **one** application that you own.
- Ask Codex for a *read-only* architecture tour.
- Map its inputs, outputs, authentication, storage, external APIs, and trust boundaries.
- Identify three credible security risks and possible mitigations.
- **Pass:** You can explain in your own words which threat matters most and why.

### Lab 2 — Triage a findings backlog (60–90 min)
- Run safe repository-local scanning and request an evidence-based code review.
- Categorize findings as confirmed, plausible, false positive, or needs more data.
- For each, record vulnerability type, location, prerequisites, affected assets and uncertainty.
- Learn what CVSS measures and what EPSS estimates; do not treat scores alone as business priority.
- **Pass:** Three findings triaged with defensible explanations.

### Lab 3 — Fix and verify one issue (60–120 min)
- Choose a confirmed problem and create a branch.
- Add a regression test that demonstrates intended safe behavior.
- Request a minimal Codex fix; inspect every change and run relevant tests.
- Draft a PR explaining exploitability in safe terms, root cause, mitigation and residual risk.
- **Pass:** A reviewed fix with passing evidence.

### Lab 4 — Detection and response exercise (60–90 min)
- Generate **synthetic** logs for a defined abuse scenario in a local fixture.
- Define useful indicators and a detection rule or query.
- Test normal behavior and malicious-lookalike events to measure false positives.
- Write an incident triage and recovery checklist.
- **Pass:** Document detection limitations and what decisions a human must make.

### Lab 5 — Teach-back and evidence pack (60–90 min)
- Explain the complete workflow to a non-specialist.
- Assemble screenshots of sample fixtures, sanitised PR links, verification logs, and a brief decision log.
- Rehearse a ten-minute walkthrough using the [demo playbook](DEMO-PLAYBOOK.md).
- **Pass:** A listener can state the risk, mitigation, remaining uncertainty and human approval point.

## Recommended defensive frameworks to learn

- [CIS Critical Security Controls](https://www.cisecurity.org/controls): start with Implementation Group 1.
- [CVSS](https://www.first.org/cvss/): vulnerability severity scoring.
- [EPSS](https://www.first.org/epss/): likelihood-of-exploitation estimate, not a severity score.
- [MITRE ATT&CK](https://attack.mitre.org/): adversary behaviors useful for detection mapping.
- [NIST Cybersecurity Framework](https://www.nist.gov/cyberframework): govern, identify, protect, detect, respond, recover.

## Evaluation rubric (score each 0–2; total /12)

1. Clear threat model and scope.
2. Verified finding evidence with false-positive handling.
3. Defensible risk ranking.
4. Minimal patch with passing regression test.
5. Detection or response limitations acknowledged.
6. Human decision points articulated.

**Rule:** The model's confidence is not evidence. All factual security claims must be supported by code, validated tests, appropriate documentation or logs.
