# Project Blueprint: Phoenix Airlines Project Request Workflow

## Purpose

Provide a consistent front door for employees to request projects, improvements, and operational work. The workflow captures minimum information, triages requests, routes the appropriate approvals, and gives requesters visible status.

## Asana project configuration

- **Project name:** Phoenix Airlines Project Request
- **Portfolio:** Phoenix Airlines Workflow Portfolio
- **Primary view:** Board for status-based flow; List for detailed review and reporting.
- **Goal:** Route at least 90% of complete requests to an initial triage decision within three business days, and record an approval or decline decision for 100% of requests that reach the approval stage.
- **Proposed operational measures:** intake completeness, time to triage, approval cycle time, aged requests, rework rate, and request volume by category.

Targets are illustrative and should be adjusted after a baseline period.

## Sections / workflow states

1. **New Request**
2. **Needs Information**
3. **Triage**
4. **Awaiting Approval**
5. **Approved — Planned**
6. **In Progress**
7. **Completed**
8. **Declined / Withdrawn**

A section represents the current state. Avoid moving a task to “Approved — Planned” until the required approval decision has been recorded.

## Custom fields

See `templates/request_custom_fields.csv`. Core fields:
- Request type
- Business impact
- Urgency
- Estimated effort
- Risk level
- Funding required
- Approval status
- Intake completeness
- Decision date

Keep fields short, consistently defined, and limited to information that supports routing or reporting.

## Form and branching design

The companion `request_form_schema.json` documents a proposed form. Configure the form in Asana and implement branching using the form editor if the feature is available. The schema file is a reusable specification; it is not guaranteed to import directly as a native Asana form.

Suggested branches:
- **Technology / systems:** ask about affected system, data sensitivity, integrations, and technical owner.
- **Process / operations:** ask which process is affected, frequency, and operational impact.
- **Customer / passenger experience:** ask which journey is affected, accessibility considerations, and service impact.
- **Funding required = Yes:** collect estimated amount, cost center, and funding sponsor.
- **Urgency = Critical:** ask for business impact and escalation contact; do not bypass governance solely because the request is urgent.

## Approval model

See `templates/approval_matrix.csv`. A recommended decision path:
1. Request coordinator validates completeness.
2. Functional owner assesses fit, impact, and capacity.
3. Finance approval is required when funding crosses the organization's defined threshold.
4. Security/privacy review is required for sensitive data, integrations, or elevated risk.
5. Sponsor makes the final prioritization decision for requests competing for capacity.

Replace thresholds and approver roles with approved internal policy. Asana's native approval features and available rule triggers vary by plan and configuration; where a native approval task is unavailable, use a documented approval task with a required decision field and evidence link.

## Rules to configure

See `templates/request_rules.csv`. Examples:
- When a request enters Triage and Intake completeness is Complete, assign the Request Coordinator and notify the triage group.
- When Approval status changes to Approved, move the request to Approved — Planned and notify the requester.
- When Approval status changes to Declined, move it to Declined / Withdrawn and require a reason.
- When Urgency is Critical, notify the workflow owner and flag for rapid review without skipping required approvals.
- When a task becomes overdue, notify the owner and coordinator.

Build and test each rule in the workspace; do not assume a CSV import creates native rules.

## Handoff contract

A handoff is complete only when:
- Required intake fields are present.
- The current owner is clear.
- The next state is accurate.
- Approval requirements are known.
- The next action and due date are visible.
- The requester receives a status update at defined points.
