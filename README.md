# Asana Workflow Design Portfolio
### A practical workflow-operations capstone by Blair Page

> **Portfolio purpose:** demonstrate practical workflow design, intake, governance, approvals, automation, reporting, and change adoption using Asana-ready templates. This is an interview portfolio, not an exam answer sheet.

**Author:** Blair Page  
**Repository:** `asana-workflow-design-portfolio`  
**Version:** 1.0.0  
**Status:** Reusable reference implementation; adapt assumptions to the real organization before deployment.

## What this repository demonstrates

This portfolio translates three provided project rubrics into implementation-ready workflow blueprints:

1. **Biometric Boarding and Security Initiative** — project planning, milestones, dependencies, task hygiene, success metrics, and portfolio reporting.
2. **Phoenix Airlines Project Request Workflow** — structured intake, branching form design, custom fields, triage, approvals, rules, and service-level reporting.
3. **Phoenix Airlines Workflow Socialization Strategy** — pilot selection, communication, two-week training, organizational conventions, feedback, and adoption measurement.

The rubrics refer to a spreadsheet and process map that were not included with the supplied files. Accordingly, the task lists, field options, process steps, roles, dates, targets, and example metrics in this repository are **explicit working assumptions**, not claims about missing source documents. Replace them with approved organizational information before real deployment.

## Repository map

```text
asana-workflow-design-portfolio/
├── README.md
├── LICENSE
├── CHANGELOG.md
├── docs/
│   ├── 01-portfolio-overview.md
│   ├── 02-biometric-boarding-security.md
│   ├── 03-project-request-workflow.md
│   ├── 04-socialization-and-change-plan.md
│   ├── 05-governance-and-reporting.md
│   ├── 06-interview-walkthrough.md
│   ├── 07-implementation-checklist.md
│   └── 08-assumptions-and-limitations.md
├── templates/
│   ├── README.md
│   ├── biometric_tasks.csv
│   ├── biometric_custom_fields.csv
│   ├── biometric_dependencies.csv
│   ├── request_workflow_tasks.csv
│   ├── request_custom_fields.csv
│   ├── request_rules.csv
│   ├── request_form_schema.json
│   ├── approval_matrix.csv
│   ├── pilot_members.csv
│   ├── communication_plan.csv
│   ├── two_week_training_plan.csv
│   ├── conventions.md
│   └── metrics_dictionary.csv
└── diagrams/
    ├── biometric-workflow.mmd
    ├── request-intake.mmd
    └── change-adoption.mmd
```

## How to use it

1. Read the project blueprints in `docs/`.
2. Create the projects and portfolio in Asana using the setup instructions.
3. Import the task CSVs through Asana's CSV import workflow; map the columns to task name, description, assignee, due date, section, and custom fields as appropriate. Import behavior and supported field mapping can vary by workspace and plan.
4. Create custom fields, rules, forms, approvals, milestones, and dependencies in Asana using the accompanying configuration templates. CSV import alone does not reliably create every native Asana feature.
5. Replace role-based owners and illustrative dates with actual people and dates.
6. Test in a pilot project, collect feedback, and publish the approved version.

## Portfolio / interview framing

**Problem:** work intake and delivery can become inconsistent when requests, ownership, handoffs, and training are not standardized.

**Approach:** define a measurable goal, model the workflow, establish fields and conventions, automate predictable transitions, use approvals for controlled decisions, and plan adoption before scaling.

**Evidence to show in an interview:** project board/list, sample form and branch logic, rule configuration, dependency chain, milestone view, approval matrix, reporting definitions, communication plan, and two-week training schedule.

## Important implementation notes

- The biometric boarding scenario is a **planning simulation**. It does not include biometric data, passenger records, security procedures, or technical deployment instructions.
- Use privacy-by-design, legal review, accessibility testing, human review, and a documented fallback path for any real biometric program.
- Rule and form capabilities depend on Asana plan and workspace settings. Confirm feature availability before promising a particular automation.
- Do not treat the example targets as measured results. They are proposed acceptance criteria.

## Quick links

- [Portfolio overview](docs/01-portfolio-overview.md)
- [Biometric boarding and security](docs/02-biometric-boarding-security.md)
- [Project request workflow](docs/03-project-request-workflow.md)
- [Socialization and change plan](docs/04-socialization-and-change-plan.md)
- [Governance and reporting](docs/05-governance-and-reporting.md)
- [Interview walkthrough](docs/06-interview-walkthrough.md)
- [Implementation checklist](docs/07-implementation-checklist.md)
- [Assumptions and limitations](docs/08-assumptions-and-limitations.md)
- [Importable templates](templates/README.md)
