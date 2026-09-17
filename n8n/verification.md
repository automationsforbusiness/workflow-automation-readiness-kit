# Verification record

The workflow in this folder was imported and executed locally with n8n `2.39.6` on 16 September 2026. It was imported into a fresh isolated data folder and executed again after the in-canvas safety note was added.

## Test boundary

- Local, isolated n8n data folder
- Manual trigger
- Built-in n8n nodes only
- Two fictional enquiries
- No credentials
- No external API calls
- No email, CRM, database, or customer-system changes
- One non-executing sticky note explaining the sample boundary

## Result

The n8n CLI completed the workflow with `status: success` and `finished: true`.

| Sample | Validation result | Final review state |
| --- | --- | --- |
| `sample-complete-001` | Email normalized; no required fields missing | `ready_for_human_approved_pilot` |
| `sample-needs-details-002` | Invalid email plus missing task and owner detected | `needs_clarification` |

The If node sent one item to each intended branch. The complete sample still requires a named person to approve the pilot output before any customer-facing action.

## Reproduce the check

After importing the workflow, use its included ID:

```text
n8n execute --id=AFBLeadReview01 --rawOutput
```

Confirm that the output reports a successful finished execution and contains both final `reviewState` values shown above.
