# OctoAcme — Roles & Responsibility Matrix Template

## Purpose
This template provides a reusable RACI matrix for mapping project responsibilities to defined personas. Copy and adapt it for each project or workstream.

**Key:**
- **A** — Accountable (owns the outcome; one per row)
- **R** — Responsible (performs the work)
- **C** — Consulted (provides input before decision/action)
- **I** — Informed (notified of outcomes)

---

## How to fill this template
1. List all key activities or deliverables in the **Responsibility** column.
2. Add a column for each persona/role that participates in your project.
3. Assign exactly **one A** per row. Multiple **R**, **C**, and **I** entries are allowed.
4. Review the matrix with all stakeholders at project kickoff and update it when team composition or scope changes.
5. **Recommended review cadence:** At kickoff, after any major scope change, and at each retrospective.

---

## Example Matrix

| Responsibility              | PM | PdM | Developer | QA | UX Designer | Data Analyst | DevOps Eng. | CSM | Security Lead |
|-----------------------------|:--:|:---:|:---------:|:--:|:-----------:|:------------:|:-----------:|:---:|:-------------:|
| Product decisions           | C  | A/R | C         | I  | C           | C            | I           | C   | C             |
| Technical design            | I  | C   | A/R       | C  | C           | C            | R           | I   | R             |
| UX / Design sign-off        | I  | C   | C         | I  | A/R         | I            | I           | C   | I             |
| QA sign-off / release gate  | I  | I   | R         | A/R| I           | I            | I           | I   | C             |
| Deployment approval         | R  | I   | R         | R  | I           | I            | A/R         | I   | R             |
| Incident response           | R  | I   | R         | C  | I           | C            | A/R         | I   | R             |
| Customer communication      | C  | C   | I         | I  | I           | I            | I           | A/R | C             |
| Risk tracking               | A/R| C   | C         | C  | I           | C            | C           | I   | R             |
| Metrics & reporting         | R  | R   | C         | C  | I           | A/R          | C           | C   | I             |
| Security review             | I  | I   | R         | C  | I           | I            | R           | I   | A/R           |

---

## Blank Template

Copy the table below and replace the placeholder rows with project-specific responsibilities.

| Responsibility              | PM | PdM | Developer | QA | UX Designer | Data Analyst | DevOps Eng. | CSM | Security Lead |
|-----------------------------|:--:|:---:|:---------:|:--:|:-----------:|:------------:|:-----------:|:---:|:-------------:|
| _Add responsibility here_   |    |     |           |    |             |              |             |     |               |
| _Add responsibility here_   |    |     |           |    |             |              |             |     |               |
| _Add responsibility here_   |    |     |           |    |             |              |             |     |               |

---

## How this improves outcomes
- **Clearer accountability**: Each responsibility has an explicit owner, reducing hand-off confusion.
- **Faster onboarding**: New team members immediately understand who to involve for each decision.
- **Fewer escalations**: Eliminating ambiguity up front reduces unnecessary escalations during execution.
- **Improved retrospectives**: The matrix gives teams a concrete artifact to review when accountability gaps surface.
