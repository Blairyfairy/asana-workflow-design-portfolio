# Interview Walkthrough (5–7 minutes)

## 1. Start with the business problem

“I'm demonstrating a small workflow portfolio that covers both delivery planning and intake governance. The aim is to make ownership, handoffs, approvals, and progress visible, while making adoption part of the rollout rather than an afterthought.”

## 2. Show the biometric boarding project

Walk through:
- The project goal and measurable readiness criteria.
- Sections representing project phases.
- Action-oriented task titles and clear completion descriptions.
- Milestones for charter approval, requirements sign-off, and readiness go/no-go.
- Dependencies showing the critical path and parallel reviews.
- Custom fields for workstream, priority, risk, readiness, and approval status.
- Privacy, accessibility, human fallback, and governance safeguards.

**Explain the trade-off:** dependencies make sequence visible, but they do not replace communication or a named owner.

## 3. Show the request workflow

Walk through:
- The request form and conditional questions.
- Board columns from New Request to Completed or Declined.
- Custom fields that enable routing and reporting.
- Approval matrix and decision record.
- Rules for complete intake, critical urgency, approval outcomes, and overdue tasks.

**Explain the trade-off:** automation should reduce repetitive coordination but preserve required human decisions and exception handling.

## 4. Show the adoption plan

Walk through:
- Pilot roles and why the cohort is cross-functional.
- Communication plan.
- Two-week training plan.
- Conventions for naming and task quality.
- Feedback and go/no-go measures.

**Explain the trade-off:** a technically configured workflow can still fail if people do not understand it or trust the process.

## 5. Close with evidence and next steps

“I would validate the proposed fields and targets with stakeholders, configure the native Asana features in a sandbox, run test cases for standard and exception paths, baseline the metrics, and only then recommend wider rollout.”

## Likely interview questions

**Why use dependencies?** They clarify prerequisites and reduce premature handoffs; they also expose schedule risk when a predecessor slips.

**Why use custom fields?** They make work sortable and reportable using consistent values rather than inconsistent free-text labels.

**Why use a form?** It standardizes intake at the source and can show only relevant follow-up questions when branching is available.

**What should be automated?** Predictable routing and notifications. Decisions involving risk, funding, privacy, or scope should remain with authorized humans.

**How would you prove improvement?** Capture a baseline, run the pilot, compare time to triage and intake completeness, inspect exceptions, and report sample size and limitations.

**What is missing from this portfolio?** The source rubrics refer to a spreadsheet and process map that were not supplied, and no live Asana workspace export or actual pilot results were provided. I would replace assumptions with approved inputs and verify native configuration before claiming deployment.
