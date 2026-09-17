# Customer-message handoff workflow verification

The workflow in this folder was imported into a fresh isolated data folder and executed locally with n8n `2.39.6` on 16 September 2026.

## Test boundary

- Local, isolated n8n data folder
- Manual trigger
- Built-in n8n nodes only
- Two fictional customer messages
- No credentials
- No AI-model call
- No external API calls
- No reply, notification, CRM, inbox, or customer-system change
- One non-executing sticky note explaining the sample boundary

## Result

The n8n CLI completed the workflow with `status: success` and `finished: true`.

| Sample | Detected signals | Final review state |
| --- | --- | --- |
| `sample-routine-001` | No human-request, review-topic, sensitive-data, open-case, or empty-message signal | `safe_for_assistant_draft` |
| `sample-human-002` | Explicit request for a person; existing open case; review terms `urgent` and `charge` | `human_review_required` |

The If node sent one item to each intended branch. The routine state grants permission to draft only; it does not approve or send a reply.

## Reproduce the check

After importing the workflow, use its included ID:

```text
n8n execute --id=AFBMessageHandoff01 --rawOutput
```

Confirm that the output reports a successful finished execution and contains both final `reviewState` values shown above. All people, channels, messages, states, and results are fictional.
