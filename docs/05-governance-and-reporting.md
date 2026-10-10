# Governance and Reporting

## Governance cadence

| Cadence | Meeting / activity | Owner | Output |
|---|---|---|---|
| Weekly during pilot | Workflow review | Workflow owner | Blockers, rule failures, decisions |
| Weekly during pilot | Request queue review | Request coordinator | Aging requests, incomplete intake, triage backlog |
| At milestones | Readiness gate | Sponsor + designated reviewers | Recorded go / no-go decision |
| End of week 1 and week 2 | Pilot feedback review | Change lead | Prioritized improvement backlog |
| Monthly after rollout | Performance review | Process owner | KPI trends, rule maintenance, conventions updates |

## Decision rights

- **Sponsor:** approves scope and resolves priority conflicts.
- **Workflow owner:** maintains process and conventions.
- **Security/privacy/legal reviewers:** decide whether their review requirements are satisfied within their remit.
- **Functional approver:** approves work in their area.
- **Request coordinator:** validates intake and maintains queue quality.
- **Task assignee:** owns task completion and communicates blockers.

A role-based example is not a substitute for the organization's official RACI or delegated authority.

## Metrics dictionary

The CSV template defines metric names, operational definitions, calculation approach, review cadence, and owner. Establish a baseline before setting permanent targets.

Suggested definitions:
- **Intake completeness rate:** complete submissions divided by all submissions in the period.
- **Time to triage:** elapsed business time from submission to first triage decision.
- **Approval cycle time:** elapsed business time from entering Awaiting Approval to a recorded decision.
- **On-time task completion:** tasks completed on or before their due date divided by tasks due in the period.
- **Dependency blockage rate:** active tasks blocked by unmet prerequisites divided by active tasks with dependencies.
- **Training completion:** pilot participants who complete required training divided by participants assigned training.

## Reporting principles

- Show both volume and time; percentages alone can hide low sample sizes.
- Segment by request type and urgency where appropriate.
- Make data definitions visible.
- Review exceptions and qualitative feedback alongside charts.
- Avoid exposing sensitive employee, passenger, or security information in portfolio dashboards.
- Separate target, actual, and forecast values.
