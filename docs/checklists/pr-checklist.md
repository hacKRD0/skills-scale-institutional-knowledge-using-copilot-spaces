# OctoAcme — PR Checklist

Use this checklist before requesting a review on any pull request. All items should be checked (or explicitly marked N/A with a note) before the PR is marked ready.

---

## Author Checklist

### Code Quality
- [ ] Code follows the project style guide and passes linting (`CI: lint`)
- [ ] No debug statements, commented-out code, or TODO items left unaddressed
- [ ] PR is small and focused — prefer ≤ 400 lines of change where possible; if larger, add a note explaining why

### Tests
- [ ] Unit tests cover new logic (including edge cases)
- [ ] Integration tests updated or added where applicable
- [ ] All CI checks pass (tests, lint, build)
- [ ] No existing tests have been deleted or weakened without justification

### Documentation
- [ ] Inline code comments added for non-obvious logic
- [ ] Relevant docs (README, ADRs, runbooks) updated if behavior has changed
- [ ] CHANGELOG or release notes entry added if this change is user-facing

### Issue & Acceptance Criteria
- [ ] PR description links to the related issue (e.g., `Closes #<issue>` or `Relates to #<issue>`)
- [ ] Acceptance criteria from the linked issue are met and noted in the PR description
- [ ] Screenshots or recordings attached for UI changes

### Security
- [ ] No secrets, credentials, or PII committed to the repository
- [ ] Input validation and output encoding applied where relevant
- [ ] Security scanning in CI passes with no new high/critical findings
- [ ] Dependency updates reviewed for known vulnerabilities (check advisory database)

### Database / Data Migrations
- [ ] Migration script included if schema changes are required (N/A if not applicable)
- [ ] Migration is reversible / rollback procedure documented

---

## Required Approvers by Change Type

| Change Type                        | Required Approvers                          |
|------------------------------------|---------------------------------------------|
| Feature / Bug fix                  | At least 1 Developer peer reviewer          |
| Infrastructure / CI/CD changes     | DevOps Engineer + 1 Developer               |
| Security-sensitive changes         | Security Lead + 1 Developer                 |
| Public API / contract changes      | PdM + 1 Developer                           |
| Database schema changes            | Developer + DevOps Engineer                 |
| Release / version bump             | PM + DevOps Engineer                        |

---

## Reviewer Checklist

- [ ] Logic is correct and matches the acceptance criteria
- [ ] Tests are adequate and meaningful
- [ ] No obvious security or performance concerns
- [ ] Documentation is sufficient
- [ ] Change fits within the scope described in the issue / PR description

---

## How this improves outcomes
- **Consistent quality gate**: Every PR passes the same bar, reducing production incidents caused by missing tests or undocumented changes.
- **Faster reviews**: Reviewers spend less time flagging common issues; authors self-serve before requesting review.
- **Clearer accountability**: Required approvers table removes ambiguity about who must sign off for each change type.
- **Improved security posture**: Explicit security checks surface issues before merge rather than in production.
