# Weekly report workflow verification

The workflow in this folder was imported and executed locally with n8n `2.39.6` on 16 September 2026. On 17 September it was imported and executed again after the in-canvas note was expanded to the complete Creator Hub description.

## Test boundary

- Local, isolated n8n data folder
- Manual trigger
- Built-in n8n nodes only
- Two fictional weekly records
- No credentials
- No external API calls
- No analytics, CRM, email, spreadsheet, database, or customer-system changes
- One non-executing 187-word sticky note covering audience, behavior, setup, requirements, customization and the owner-approval boundary

## Result

The 17 September n8n CLI run completed the updated workflow with `status: success` and `finished: true`.

| Sample | Calculated values | Validation result | Final review state |
| --- | --- | --- | --- |
| `sample-stable-week` | Request rate `5.6%`; completion rate `88.9%` | Named owner; no overdue items or critical exceptions | `ready_for_owner_approval` |
| `sample-review-week` | Request rate `7.9%`; completion rate `54.5%` | Missing owner, one critical exception, two overdue items | `needs_exception_review` |

The If node sent one item to each intended branch. The stable sample still requires the named owner to compare it with the source system before it can be shared.

## Reproduce the check

After importing the workflow, use its included ID:

```text
n8n execute --id=AFBWeeklyReport01 --rawOutput
```

Confirm that the output reports a successful finished execution and contains both final `reviewState` values shown above. The percentages are computed from fictional data and are not customer results.
