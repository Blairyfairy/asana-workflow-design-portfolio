# Templates and Import Guide

These files are designed to be reused as starter assets. CSVs use UTF-8 text and a header row.

## Task CSVs

- `biometric_tasks.csv` — task and subtask plan for the Biometric Boarding and Security Initiative.
- `request_workflow_tasks.csv` — sample workflow tasks and operational setup tasks for the request project.

### Import suggestions

1. Create the project in Asana.
2. Import the relevant CSV through the project's import option.
3. Map `Task Name` to the task name and `Description` to the description field.
4. Map `Section` to sections if supported; otherwise create sections first and move tasks after import.
5. Map `Due Date` only after replacing sample dates with your project calendar.
6. Map custom-field columns only if the importer recognizes existing fields. Otherwise create the fields first and remap or populate them after import.
7. Review parent/subtask relationships and owner mappings; CSV importer behavior may vary.
8. Add native milestones, dependencies, forms, rules, and approvals manually from the configuration templates.

## Configuration catalogs

- `biometric_custom_fields.csv` and `request_custom_fields.csv` define field types, options, and purpose.
- `biometric_dependencies.csv` lists predecessor → successor relationships.
- `request_rules.csv` provides rule trigger/condition/action designs to configure in Asana.
- `request_form_schema.json` is a readable form specification, not a guaranteed direct import format.
- `approval_matrix.csv` defines decision gates.
- `pilot_members.csv`, `communication_plan.csv`, and `two_week_training_plan.csv` are reusable change-management plans.
- `metrics_dictionary.csv` standardizes proposed metrics.
- `conventions.md` defines operating standards.

## Date convention

Sample task dates use ISO format `YYYY-MM-DD` for clarity. They are illustrative. Replace them with dates appropriate to the actual project before importing.
