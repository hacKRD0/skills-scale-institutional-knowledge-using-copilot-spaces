# OctoAcme — Risk Register Template

Consistent with the risk management approach defined in [docs/octoacme-risks-and-communication.md](../octoacme-risks-and-communication.md).

## Purpose
Track identified risks, their potential impact, and the actions taken to mitigate them. Review and update this register at every weekly sync.

---

## How to use this template
1. Assign each risk a unique **ID** (e.g., `RISK-001`).
2. Briefly describe the risk in the **Description** column.
3. Rate **Impact** and **Likelihood** as `High`, `Med`, or `Low`.
4. Assign an **Owner** — the person responsible for driving mitigation.
5. Document the **Mitigation** strategy and any contingency plan.
6. Update **Status** as the risk evolves: `Open`, `Mitigated`, `Accepted`, `Closed`.
7. Record the **Last Reviewed** date at each weekly sync.

---

## Risk Register

| ID       | Description | Impact | Likelihood | Owner | Mitigation | Status | Last Reviewed |
|----------|-------------|:------:|:----------:|-------|------------|:------:|:-------------:|
| RISK-001 | _Example: Third-party API deprecation before launch_ | High | Med | Developer | Identify alternative API; build abstraction layer | Open | YYYY-MM-DD |
| RISK-002 | _Example: Key team member unavailable during release window_ | Med | Low | PM | Cross-train backup; document runbook | Open | YYYY-MM-DD |
| RISK-003 | _Add risk here_ | | | | | | |

---

## Field Definitions

| Field | Description |
|-------|-------------|
| **ID** | Unique identifier (e.g., `RISK-001`) |
| **Description** | Concise statement of the risk event and its potential consequence |
| **Impact** | Business or delivery impact if the risk materializes: `High`, `Med`, `Low` |
| **Likelihood** | Probability of occurrence: `High`, `Med`, `Low` |
| **Owner** | Role or person accountable for monitoring and driving mitigation |
| **Mitigation** | Actions taken or planned to reduce impact or likelihood; include contingency if applicable |
| **Status** | `Open` / `Mitigated` / `Accepted` / `Closed` |
| **Last Reviewed** | Date the risk was last reviewed at a weekly sync (ISO format: `YYYY-MM-DD`) |

---

## Risk Lifecycle (summary)

| Stage | Description |
|-------|-------------|
| **Identify** | Surface risks during planning, standups, and execution |
| **Assess** | Rate impact and likelihood; assign owner |
| **Mitigate** | Define and execute mitigation actions |
| **Monitor** | Review at weekly syncs; update status and mitigation notes |
| **Close** | Mark `Closed` when risk is no longer relevant or fully mitigated |

---

## How this improves outcomes
- **Proactive risk management**: A living register ensures risks are visible and never forgotten between meetings.
- **Clearer ownership**: Every risk has a named owner, reducing the chance that risks fall through the cracks.
- **Faster escalation**: High-impact risks are immediately visible to PM and sponsors during weekly reviews.
- **Audit trail**: The Last Reviewed field provides a traceable history of risk monitoring activity.
