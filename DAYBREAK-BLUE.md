# Daybreak Blue: Access Readiness and Defensive Security Track

**What it is:** OpenAI's Daybreak Blue is an approved-access tier within Trusted Access for Cyber. It provides reduced unnecessary refusals on supported models for *authorized defensive cybersecurity work*; it does not automatically unlock Daybreak Red or cyber-specialized models. It is **not** a general Codex performance tier or blanket authorization to probe external systems.

## Access checklist (do in parallel with Sprint Days 1–5)

1. Read [Daybreak overview](https://help.openai.com/en/articles/20001258-openai-daybreak-trusted-access-for-cyber-overview) and [getting started](https://learn.chatgpt.com/use-cases/getting-started-with-daybreak-blue).
2. Choose **individual** or **organization** application based on your real usage. Individuals can start at [chatgpt.com/cyber](https://chatgpt.com/cyber). Organizational enrollment and role/project provisioning are distinct.
3. Prepare an accurate intended-use explanation: e.g., *secure code review, dependency triage, regression tests, and remediation for repositories I own or am authorized to maintain*. Do not claim permissions or work you do not have.
4. Follow identity verification and Advanced Account Security requirements (including compatible physical FIDO2 hardware key where required); do not store verification documents or credentials in this public repo.
5. If approved, confirm the approved ChatGPT workspace or API organization/project, authorized product surface/model, and any admin provisioning. Access might remain disabled until enabled by workspace/project owners.
6. In supported Codex clients, use the Daybreak control only when approved. If using CLI, follow current official setup and version instructions; verify current docs rather than guessing from an old tutorial.
7. Read [troubleshooting](https://help.openai.com/en/articles/20001259-troubleshooting-openai-daybreak). **No approval or no toggle = continue with standard Codex**.

## Specialized 5-session defensive lab (safe for standard Codex)

### Blue Lab 1: Threat-model an application
- Use an application you own or an intentionally vulnerable local learning lab.
- Identify assets, data flows, trust boundaries, probable threats, and mitigations.
- **Proof:** `security/threat-model.md` containing a small diagram, assumptions, and priorities.

### Blue Lab 2: Secure code review
- Read code for missing authorization, untrusted input handling, unsafe deserialization, leaked secrets, and error handling.
- Prioritize findings by exploitability and impact; avoid unsupported vulnerability claims.
- **Proof:** finding reports with file/line evidence and remediation recommendations.

### Blue Lab 3: Dependency and secrets hygiene
- Inspect lockfiles, package versions, scanning results, and accidental secret commits on a repository you control.
- Do not copy real secrets into model prompts or logs; rotate exposed secrets via appropriate channels.
- **Proof:** dependency and secrets audit checklist.

### Blue Lab 4: Validate and remediate
- Reproduce an identified bug using safe fixtures and tests in an isolated development environment.
- Fix the root cause, add a regression test, open a reviewable PR.
- **Proof:** PR with test results and rollback instructions.

### Blue Lab 5: Continuous secure development
- Add scoped tests or automated scans to the CI workflow with clear severity thresholds.
- Document false positives, triage decisions, monitoring and ownership.
- **Proof:** security improvements merged with checks passing.

## Practice tasks that develop true proficiency

- Compare what the agent claims with the actual diff and test evidence.
- Ask for evidence supporting each security finding and possible false positives.
- Compare Codex and Claude Code on **the same authorized code**, with identical acceptance criteria and separate branches.
- Maintain a security decisions log; don't equate scanning tools with proof of exploitability.

## Boundaries

- Only test systems, applications, accounts, networks or data you own, operate or have explicit authorization to assess.
- Do not expand work into third-party or production systems absent written permission and a defined scope.
- Daybreak Blue does not grant Daybreak Red, unlimited use, unrestricted refusal removal, or access to all models.
- Access through an approved team workspace or API project is for approved internal use, not unauthorized third-party or customer-facing services.
- Prefer a safe Codex approval/auto-review posture; review high-impact actions before they execute.

## References

- [OpenAI Daybreak overview](https://help.openai.com/en/articles/20001258-openai-daybreak-trusted-access-for-cyber-overview)
- [Team provisioning](https://help.openai.com/en/articles/20001531-openai-daybreak-set-up-access-for-your-team)
- [Getting started with Daybreak Blue](https://learn.chatgpt.com/use-cases/getting-started-with-daybreak-blue)
- [Daybreak troubleshooting](https://help.openai.com/en/articles/20001259-troubleshooting-openai-daybreak)
