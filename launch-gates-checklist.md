# Four launch gates for a reliable automation

Use this check immediately before a workflow pilot handles real work. A workflow passes only when every gate has an observable test and a named owner.

## Gate 1: required input

The workflow should not start useful work until every required field is present and valid.

- List the fields that are truly required.
- Reject placeholder values and unsupported formats.
- Route incomplete records to a person or a clearly labelled holding state.
- Never invent missing customer, financial or operational information.

**Pass test:** submit one complete record and one record missing a required field. The complete record continues; the incomplete record stops safely with a useful reason.

## Gate 2: duplicate protection

The same event can arrive more than once because of retries, refreshes, imports or connected tools.

- Choose a stable identifier, such as an enquiry ID, order ID or source record ID.
- Define the time window in which two events count as the same work.
- Decide whether the safe action is ignore, update, merge or request review.
- Record the duplicate decision without creating the downstream action twice.

**Pass test:** send the same sample event twice. Only the intended single downstream result is created.

## Gate 3: visible failure

A failed workflow must leave enough information for someone to find and recover the unfinished work.

- Name the owner who receives the alert.
- Include the failed step, record identifier and time.
- Keep secrets and unnecessary customer data out of alerts and logs.
- Define which failures may retry automatically and how many times.
- Provide a manual recovery path that cannot repeat completed actions.

**Pass test:** deliberately fail one safe sample step. The owner can identify the unfinished record and recover it without guessing or duplicating earlier work.

## Gate 4: human approval

Keep a person between an automated draft and any action with meaningful customer, financial, legal or irreversible impact.

- Name who may approve or reject the action.
- Show the reviewer the source facts, proposed action and important warnings.
- Set a timeout and a safe outcome when nobody responds.
- Record the decision and the version that was approved.
- Make rejection or correction as easy as approval.

**Pass test:** approve one sample, reject one sample and let one sample time out. Each follows the defined path, and none proceeds without the required decision.

## Go/no-go record

| Gate | Owner | Evidence from the test | Result | Fix before launch |
| --- | --- | --- | --- | --- |
| Required input |  |  | Pass / Fail |  |
| Duplicate protection |  |  | Pass / Fail |  |
| Visible failure |  |  | Pass / Fail |  |
| Human approval |  |  | Pass / Fail |  |

## Decision

- **Go:** all four gates pass with evidence, and the pilot can be paused or rolled back.
- **Fix first:** any gate fails, has no owner, or relies only on an assumption.
- **Reduce scope:** the workflow is too broad to test safely as one pilot.

Passing these gates does not prove that a workflow will never fail. It proves that the team has tested the most common ways an automation creates silent or repeated work and has a practical response when something goes wrong.
