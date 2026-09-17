# Example: lead-enquiry handoff

This example shows how a small service business might acknowledge a website enquiry, prepare context for a person, and avoid sending an unreviewed promise.

## Outcome

Every valid enquiry receives a prompt acknowledgement, the team sees a useful summary, and a person approves any pricing or delivery commitment.

## Trigger

A visitor submits the website contact form.

## Normal path

1. Validate that the name, contact method and request are present.
2. Check whether the same contact and message were received recently.
3. Store the enquiry in the chosen system of record.
4. Send a short acknowledgement that states when a person normally responds.
5. Prepare a summary containing the request, current tools and any stated deadline.
6. Notify the assigned person.
7. Pause until the person reviews the enquiry.

## Exceptions

| Situation | Safe response |
| --- | --- |
| Required detail missing | Ask one clear follow-up question; do not create a quote. |
| Duplicate submission | Link it to the existing enquiry and avoid a second acknowledgement. |
| Possible spam | Quarantine it for review and do not follow external links automatically. |
| Customer requests a person | Stop automated sales replies and alert the assigned person. |
| System of record unavailable | Queue the item, alert the owner and retry with an upper limit. |
| No human response by the stated time | Send an honest delay update and offer a direct contact option. |

## Human approval

A person must approve pricing, scope, delivery dates, contracts and any statement that could create a customer commitment.

## Minimum log

Record the event time, workflow version, outcome, error category and human-review state. Avoid copying full private messages into multiple tools when a secure source record can be referenced instead.

## Pilot

Run 20 test cases that include missing details, duplicates, spam and delayed approval. Compare acknowledgement time, missed enquiries, duplicate messages and staff rework with the current process. Pause the pilot if any message is sent to the wrong recipient or a customer commitment is created without approval.
