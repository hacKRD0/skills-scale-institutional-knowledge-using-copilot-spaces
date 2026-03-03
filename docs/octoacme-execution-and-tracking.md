# OctoAcme — Execution & Tracking

## Purpose
Guidance for managing day-to-day execution and tracking progress toward project milestones.

## Team Rhythm
- Daily standups (15 min) — focus on progress, blockers, dependencies
- Weekly delivery sync — show progress, updates, and flagged risks
- Demo/Review at the end of each sprint or milestone

## Workflows
- Use the project board (e.g., GitHub Projects) with columns: Backlog, Ready, In Progress, In Review, QA, Done
- Pull Request workflow:
  - Small PRs (<= 400 lines when possible)
  - Include issue link and acceptance criteria in PR description
  - Run automated tests and linting in CI before requesting review
  - Require at least one approval before merging (or team-defined policy)
  - Follow the full **[PR / CI gating checklist](checklists/pr-checklist.md)** before marking a PR ready for review

## Quality & Testing
- Unit tests for new logic
- Integration tests where applicable
- End-to-end smoke tests for critical flows before release
- Security scanning in CI
- Manual QA for feature acceptance when needed

## Reporting & Metrics
- Track velocity and burndown
- Monitor success metrics identified in the Project One-pager
- Use dashboards for key signals (errors, latency, usage)

## Blocker Escalation
- Level 1: Team-level triage in daily standup
- Level 2: PM escalates to Product Lead and dependent teams
- Level 3: Sponsor-level escalation for business-impacting issues

## Execution Checklist
- [ ] Branching and PR conventions documented in repo — **Owner: Developer**
- [ ] CI configured for tests and lint — **Owner: DevOps Engineer**
- [ ] Regular demos scheduled — **Owner: Project Manager**
- [ ] Risk register updated weekly — **Owner: Project Manager**
- [ ] [PR Checklist](checklists/pr-checklist.md) reviewed and adopted by the team — **Owner: Developer / PM**
- [ ] [Release Checklist](checklists/release-checklist.md) reviewed and assigned to release owner — **Owner: DevOps Engineer / PM**

---

## How this improves outcomes
- **Explicit action owners**: Named owners for each checklist item eliminate ambiguity about who drives each activity.
- **Consistent CI/CD gating**: Linking to the PR checklist ensures every contributor follows the same quality bar before requesting review.
- **Reduced onboarding friction**: New team members have a clear, actionable list to follow from day one.
- **Fewer escalations**: Clear ownership and checklists catch issues early, reducing reactive fire-fighting during sprints and releases.
