# Reusable prompts

## Read-only repo onboarding
> I am learning Codex. Inspect this repository without editing files. Explain entry points, architecture, setup, commands for building and testing, current risks, and three low-risk first changes. Separate verified facts from assumptions.

## Plan before code
> Investigate [feature/bug], but make no edits yet. Produce current behavior, goal, relevant files, proposed minimal changes, dependencies, risks, acceptance criteria, and test plan.

## Implementation
> Work on a new branch for [feature]. Scope: [files/features]. Constraints: [rules]. Acceptance: [observable tests]. Make the smallest change, run checks, summarize diff and limitations, and do not merge or deploy.

## Code review
> Critically review this diff for correctness, regression risks, unintended modifications, test gaps, dependencies, and security flaws. Prioritize concrete findings with file references. Do not simply agree that it works.

## Authorized security review
> Review only this repository and its local safe test fixtures for defensive AppSec issues. Identify assets and trust boundaries, provide evidence for each potential finding, assess false positives, suggest minimal patches and tests. Do not perform network probing, exploitation or changes outside my authorized scope.

## Explain like a mentor
> Explain the proposed change in plain English, show the execution path, define technical terms, explain what each test proves, and explain how to revert safely.
