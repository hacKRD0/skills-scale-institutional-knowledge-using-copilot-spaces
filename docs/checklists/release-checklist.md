# OctoAcme — Release Checklist

Use this checklist for every production release. Work through each phase in order. The **Owner** column identifies the default responsible role; adjust per project.

---

## Phase 1 — Pre-Release Requirements

| # | Item | Owner | Done |
|---|------|-------|:----:|
| 1 | All issues in the release milestone are closed or explicitly deferred | PM | [ ] |
| 2 | QA sign-off received for all in-scope features | QA | [ ] |
| 3 | Security review completed; no open high/critical findings | Security Lead | [ ] |
| 4 | Release branch cut and all PRs targeting the release have merged | DevOps Engineer | [ ] |
| 5 | [PR Checklist](pr-checklist.md) passed for all PRs in this release | Developer | [ ] |
| 6 | Release notes / CHANGELOG drafted and reviewed | PM / PdM | [ ] |
| 7 | Database migrations tested in staging | Developer + DevOps Eng. | [ ] |
| 8 | Feature flags configured for staged rollout (if applicable) | DevOps Engineer | [ ] |
| 9 | Rollback plan documented and accessible to on-call team | DevOps Engineer | [ ] |

---

## Phase 2 — Deployment Steps

| # | Item | Owner | Done |
|---|------|-------|:----:|
| 1 | Notify stakeholders of upcoming deployment window | PM | [ ] |
| 2 | Confirm monitoring and alerting dashboards are active | DevOps Engineer | [ ] |
| 3 | Deploy to staging and run smoke tests | DevOps Eng. + QA | [ ] |
| 4 | Obtain final deployment approval (see Required Approvers below) | PM | [ ] |
| 5 | Deploy to production using approved runbook / pipeline | DevOps Engineer | [ ] |
| 6 | Monitor error rates, latency, and key metrics for 30 minutes post-deploy | DevOps Engineer | [ ] |

---

## Phase 3 — Post-Deploy Verification

| # | Item | Owner | Done |
|---|------|-------|:----:|
| 1 | Run end-to-end smoke tests in production | QA / DevOps Eng. | [ ] |
| 2 | Verify key user journeys are functioning correctly | QA | [ ] |
| 3 | Confirm metrics and dashboards reflect expected behavior | Data Analyst | [ ] |
| 4 | Check that no new error or performance alerts have fired | DevOps Engineer | [ ] |

---

## Rollback Criteria

Initiate rollback immediately if any of the following occur:
- Error rate exceeds the pre-defined threshold (e.g., > 1% 5xx rate)
- Critical user journey is broken (checkout, login, core feature)
- Security vulnerability discovered in the release
- Data integrity issue detected

**Rollback owner:** DevOps Engineer (notify PM and Security Lead immediately)

---

## Phase 4 — Communication Steps

| # | Item | Owner | Done |
|---|------|-------|:----:|
| 1 | Publish release notes to internal channels | PM | [ ] |
| 2 | Notify Customer Success Manager of changes affecting customers | PM | [ ] |
| 3 | CSM communicates release highlights / known issues to customers | CSM | [ ] |
| 4 | Update public status page / documentation if applicable | CSM / DevOps Eng. | [ ] |
| 5 | Close the release milestone in the project tracker | PM | [ ] |

---

## Required Approvers for Production Deployment

| Environment | Required Approvers |
|-------------|-------------------|
| Staging     | DevOps Engineer + QA |
| Production  | PM + DevOps Engineer + Security Lead (for security-sensitive releases) |

---

## How this improves outcomes
- **Fewer production incidents**: Structured pre-release checks catch issues before customers are affected.
- **Clear ownership**: Named owners for each phase eliminate confusion during the release window.
- **Faster rollback decisions**: Explicit rollback criteria reduce time-to-decision during incidents.
- **Consistent communication**: Stakeholders and customers receive timely, accurate release information every time.
