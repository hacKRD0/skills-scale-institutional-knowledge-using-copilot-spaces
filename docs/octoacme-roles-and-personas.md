# OctoAcme Personas

This document defines typical roles and responsibilities used in OctoAcme project docs and exercises.

---

## Developers

### Role Summary
Developers design, build, test, and deliver software components. They collaborate with product and project leads to implement features that meet acceptance criteria and quality standards.

### Responsibilities
- Implement features and fixes to meet acceptance criteria
- Write and maintain tests and documentation
- Participate in design and code reviews
- Assist in estimating and planning work
- Help identify technical risks and propose mitigations

### Goals
- Deliver reliable, maintainable code
- Reduce cycle time from idea to production
- Maintain high test coverage and observability

### Typical Communication
- Daily standups and sprint planning
- PR descriptions and code review comments
- Technical design docs when needed

---

## Product Managers

### Role Summary
Product Managers define what should be built to deliver customer and business value. They own the product vision, prioritize the backlog, and measure outcomes.

### Responsibilities
- Define problem statements and success metrics
- Prioritize the roadmap and backlog
- Collaborate with stakeholders and engineering on trade-offs
- Validate solutions through user research and metrics

### Goals
- Maximize customer value and impact
- Make clear, data-driven prioritization decisions
- Ensure product-market fit and usability

### Typical Communication
- Weekly alignment with PM and engineering leads
- Roadmap updates and stakeholder briefings
- Acceptance criteria and feature specs

---

## Project Managers

### Role Summary
Project Managers coordinate delivery activities, manage schedules, risks, and communications. They enable the team to deliver on commitments efficiently.

### Responsibilities
- Create and maintain project plans and timelines
- Manage risks, dependencies, and resource constraints
- Facilitate meetings (kickoff, planning, retrospectives)
- Ensure consistent project documentation and status reporting
- Coordinate cross-team and stakeholder communication

### Goals
- Deliver projects on time and within scope
- Minimize unplanned work and escalations
- Maintain transparency and alignment across stakeholders

### Typical Communication
- Weekly status updates and stakeholder reports
- Risk registers and decision logs
- Coordination via project boards and meeting facilitation

---

## QA Engineers

### Role Summary
QA Engineers validate that delivered software meets acceptance criteria and quality standards. They design and execute test plans, surface defects, and gate releases.

### Responsibilities
- Write and execute manual and automated test cases
- Define and maintain test plans and regression suites
- Raise and track defects through resolution
- Provide sign-off for release readiness
- Collaborate with Developers to improve testability

### Goals
- Prevent regressions and quality escapes to production
- Improve test coverage and automation over time
- Enable faster, confident releases

### Typical Communication / Interactions
- Coordinates with Developers during code review and bug triage
- Reports defect status to PM and Project Manager
- Participates in sprint planning to assess testability and scope

---

## UX Designer

### Role Summary
UX Designers own the user experience and interface design, translating product requirements into intuitive, accessible designs that delight users.

### Responsibilities
- Create wireframes, prototypes, and high-fidelity designs
- Conduct usability testing and synthesize findings
- Document user flows, design rationale, and interaction patterns
- Maintain a shared design system and component library
- Advocate for accessibility and inclusive design

### Goals
- Deliver experiences that are intuitive and meet user needs
- Reduce design-to-implementation ambiguity
- Improve usability metrics and reduce support escalations

### Typical Communication / Interactions
- Works closely with Product Managers (PdM) to align designs with feature specifications
- Collaborates with Developers during implementation to ensure design fidelity
- Shares usability findings with PM and PdM to inform prioritization

---

## Data Analyst

### Role Summary
Data Analysts collect, interpret, and communicate project and product metrics that drive evidence-based decisions.

### Responsibilities
- Define, track, and report on success KPIs and OKRs
- Build dashboards and automated reports for the team
- Partner with Developers on data instrumentation and event tracking
- Surface insights and anomalies that affect project outcomes
- Document metric definitions and data dictionaries

### Goals
- Enable data-driven prioritization and decision-making
- Improve visibility into product performance and team velocity
- Reduce time-to-insight for stakeholders

### Typical Communication / Interactions
- Reports metrics and trends to PM and PdM weekly
- Works with Developers to instrument new features
- Provides QA with baseline metrics to detect regressions

---

## DevOps Engineer

### Role Summary
DevOps Engineers build and maintain the CI/CD pipeline, deployment infrastructure, and observability tooling that enable reliable, frequent releases.

### Responsibilities
- Design, implement, and maintain CI/CD pipelines and automated deployments
- Manage infrastructure as code (IaC) and environment configurations
- Monitor system health, define alerts, and drive incident response for infrastructure issues
- Enforce deployment standards, rollback procedures, and change management
- Partner with the Security Lead on hardening and compliance

### Goals
- Enable fast, safe, and repeatable deployments
- Reduce mean time to recovery (MTTR) for production incidents
- Maintain infrastructure reliability and cost efficiency

### Typical Communication / Interactions
- Partners with Developers and QA to define pipeline gates and deployment readiness criteria
- Coordinates with Project Manager on release schedules and deployment windows
- Escalates infrastructure incidents to PM and Security Lead as needed

---

## Customer Success Manager

### Role Summary
Customer Success Managers serve as the primary liaison between users/customers and the product team, ensuring customers achieve their goals and that their feedback shapes the roadmap.

### Responsibilities
- Manage customer relationships and proactively monitor adoption and satisfaction
- Capture, document, and prioritize customer feedback and feature requests
- Support customer onboarding, training, and renewal activities
- Communicate product changes, releases, and known issues to customers
- Act as internal advocate for customer needs during planning cycles

### Goals
- Maximize customer retention and satisfaction
- Close the feedback loop between users and the product team
- Reduce time-to-value for new customers

### Typical Communication / Interactions
- Channels customer feedback to PdM and PM for roadmap input
- Works with Developers to clarify real-user use cases and edge cases
- Coordinates with Project Manager on customer-impacting release communications

---

## Security Lead

### Role Summary
The Security Lead ensures that security best practices are embedded across design, development, and deployment, and leads the organization's response to security incidents.

### Responsibilities
- Conduct threat modeling and security reviews for new features and architecture changes
- Define and maintain security policies, standards, and compliance requirements
- Review PRs and designs for security vulnerabilities
- Own and coordinate the security incident response process
- Track and drive remediation of identified security risks

### Goals
- Prevent security vulnerabilities from reaching production
- Reduce risk exposure and maintain compliance posture
- Foster a security-first culture across all roles

### Typical Communication / Interactions
- Collaborates with all roles as a security advisor throughout the SDLC
- Partners with DevOps Engineer on infrastructure security and hardening
- Escalates critical security findings to PM, Project Manager, and sponsors
- Leads post-incident reviews for security events

---

## Roles & Responsibilities Matrix

The matrix below summarizes primary accountability (A), responsibility (R), consulted (C), and informed (I) for key activities. See the full reusable template at [docs/templates/roles-responsibility-matrix.md](templates/roles-responsibility-matrix.md).

| Responsibility              | PM | PdM | Developer | QA | UX Designer | Data Analyst | DevOps Eng. | CSM | Security Lead |
|-----------------------------|:--:|:---:|:---------:|:--:|:-----------:|:------------:|:-----------:|:---:|:-------------:|
| Product decisions           | C  | A/R | C         | I  | C           | C            | I           | C   | C             |
| Technical design            | I  | C   | A/R       | C  | C           | C            | R           | I   | R             |
| UX / Design sign-off        | I  | C   | C         | I  | A/R         | I            | I           | C   | I             |
| QA sign-off                 | I  | I   | R         | A/R| I           | I            | I           | I   | C             |
| Deployment approval         | R  | I   | R         | R  | I           | I            | A/R         | I   | R             |
| Incident response           | R  | I   | R         | C  | I           | C            | A/R         | I   | R             |
| Customer communication      | C  | C   | I         | I  | I           | I            | I           | A/R | C             |
| Risk tracking               | A/R| C   | C         | C  | I           | C            | C           | I   | R             |
| Metrics & reporting         | R  | R   | C         | C  | I           | A/R          | C           | C   | I             |
| Security review             | I  | I   | R         | C  | I           | I            | R           | I   | A/R           |

---

## How this improves outcomes
Adding these personas and the responsibility matrix brings several concrete benefits:
- **Clearer accountability**: Every key activity has a named owner, reducing confusion during hand-offs.
- **Faster onboarding**: New team members can quickly understand who to consult for each type of decision.
- **Fewer escalations**: Explicit interaction notes reduce ambiguity that often leads to unnecessary escalations.
- **Better cross-functional collaboration**: Interaction expectations are set upfront, improving sprint planning and retrospective quality.

---

## How these personas are used in the exercise
- Use these persona definitions to frame scenarios and sample interactions in the Skills Exercise.
- Each persona can be used as a persona prompt for Copilot Spaces to shape role-specific guidance.

