# ChatGPT + Codex Learning Curriculum

A practical, GitHub-tracked learning path for a developer coming from Claude Code with limited hands-on coding experience. **Goal:** get productive as fast as possible while learning to supervise agents, verify changes, and ship safe software.

## Choose your track

- **Fastest route:** [10-day accelerated sprint](ACCELERATED-TRACK.md), ~90–120 minutes per day, combining the highest-value lessons in the first two weeks.
- **Sustainable route:** [4-week / 20-lesson course](#four-week-syllabus), ~30–60 minutes per day.
- **Cybersecurity specialization:** [Daybreak Blue and secure SDLC](DAYBREAK-BLUE.md), to study alongside either route. **Daybreak Blue access requires approval**, and is for authorized defensive cybersecurity work—not a general-purpose coding speed upgrade.

**Start:** [PROGRESS.md](PROGRESS.md) is your permanent progress checklist. On GitHub click Edit (pencil), tick boxes by changing `[ ]` to `[x]`, and commit. Use [LEARNING-JOURNAL.md](LEARNING-JOURNAL.md) to record evidence and questions.

## Four-week syllabus

| Week | Focus | Lessons |
| --- | --- | --- |
| [Week 1](weeks/week-1.md) | Foundations: ChatGPT, Codex, Git, repo anatomy | 1–5 |
| [Week 2](weeks/week-2.md) | Prompting, planning, AGENTS.md, debugging, PRs | 6–10 |
| [Week 3](weeks/week-3.md) | Architecture, features, testing, GitHub, deployment | 11–15 |
| [Week 4](weeks/week-4.md) | Delegation, threat modeling, AppSec, comparative evaluation, release | 16–20 |

## Rules for this course

1. Work on safe practice copies/branches. Never ask an agent to merge, deploy, or perform destructive operations without review.
2. Require a plan, a diff summary, and verification evidence; do not assume generated code works.
3. Never share secrets, private access tokens, production data, or credentials in prompts.
4. Security exercises must target your own code, deliberately vulnerable labs, or targets with explicit authorization.
5. Use Daybreak **only after** approval and provisioning, and only within the approved workspace/project and authorized scope.

## Repository contents

- [PROGRESS.md](PROGRESS.md) — checkbox tracker
- [ACCELERATED-TRACK.md](ACCELERATED-TRACK.md) — first 10-day fast path
- [DAYBREAK-BLUE.md](DAYBREAK-BLUE.md) — application and defensive security specialization
- [Week guides](weeks/week-1.md) — all 20 lessons
- [Prompt library](resources/prompt-library.md) — reusable coding and review prompts
- [Safety checklist](resources/safety-checklist.md) — before coding, merging, or deploying
- [Glossary](resources/glossary.md) — beginner-friendly terminology
- [Learning journal](LEARNING-JOURNAL.md) — ongoing notes

## Official sources

- [Codex documentation](https://developers.openai.com/codex/)
- [Codex learning](https://developers.openai.com/learn/codex)
- [Daybreak Trusted Access for Cyber](https://help.openai.com/en/articles/20001258-openai-daybreak-trusted-access-for-cyber-overview)
- [Daybreak Blue getting started](https://learn.chatgpt.com/use-cases/getting-started-with-daybreak-blue)
- [Daybreak troubleshooting](https://help.openai.com/en/articles/20001259-troubleshooting-openai-daybreak)
- [GitHub Skills](https://skills.github.com/)

## Applied defender-skills portfolio

- [Defender lifecycle labs](DEFENDER-SKILLS.md) — five hands-on security labs, from threat modeling through validating and remediating findings.
- [10-minute demonstration playbook](DEMO-PLAYBOOK.md) — a reusable executive-friendly human-plus-AI cyber defense demonstration with explicit human checkpoints.

**Suggested capstone:** Run the labs against an owned repository using synthetic or public test data, then assemble a 10-minute demo with documented evidence. The demo works with standard Codex; Daybreak Blue is optional and subject to approval.
