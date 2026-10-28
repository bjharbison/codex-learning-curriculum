# Agent safety checklist

### Before editing
- [ ] Correct repository, branch, and account
- [ ] Authorized security-testing scope (if relevant)
- [ ] Goal and acceptance criteria documented
- [ ] No plaintext credentials/tokens or sensitive data in prompts
- [ ] Plan approved, no broad destructive commands

### Before merging
- [ ] Read the complete diff
- [ ] Check unrelated changes and dependencies
- [ ] Run relevant tests and build; verify manually
- [ ] Identify unverified assumptions and risks
- [ ] Know how to revert

### Before releasing
- [ ] Verify correct deployment environment
- [ ] Confirm secrets/environment configuration
- [ ] Run smoke checks and review logs
- [ ] Record release notes and rollback method

### Additional Daybreak Blue controls
- [ ] Approval and provisioning confirmed
- [ ] Only approved user/workspace/project/surface
- [ ] Work only on owned or explicitly authorized defensive targets
- [ ] Do not assume Blue includes Red or specialized models
