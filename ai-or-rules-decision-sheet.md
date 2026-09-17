# Rules, AI or human review? A workflow decision sheet

Use this worksheet to decide how each step in a business workflow should run. The aim is not to add AI everywhere. It is to make clear decisions predictable, use AI only where interpretation helps, and keep a person responsible when an action has meaningful consequences.

This is a planning tool, not a security, legal or compliance assessment. Test the design with representative non-sensitive examples before connecting live accounts or customer data.

## The three roles

| Role | Best fit | Example | Required control |
| --- | --- | --- | --- |
| **Fixed rule** | The input and correct result can be stated exactly. | Reject a form when a required field is empty. | Test normal, missing, duplicate and invalid inputs. |
| **AI-assisted step** | The step requires interpretation, classification, extraction or draft preparation. | Suggest the topic of a free-text enquiry. | Limit the source material, validate the output and make uncertainty visible. |
| **Human review** | The action affects a customer, money, access, safety, a contract or an irreversible record. | Approve an individual quote before it is sent. | Name the responsible person and show the evidence needed to decide. |

A workflow can use all three. A fixed rule can validate the input, AI can prepare a draft, and a person can approve the final action.

## Decide one step at a time

Write one action from the current process, then answer these questions.

### 1. Is there one exact correct result?

- **Yes:** start with a fixed rule.
- **No:** continue to the next question.

Examples of exact results include checking whether a required field is present, calculating a total from approved values, choosing an owner from a defined territory table, or preventing the same event from running twice.

### 2. Does the step require interpreting language, images or inconsistent documents?

- **Yes:** an AI-assisted step may help.
- **No:** map the missing business rule before choosing a tool.

Good AI-assisted candidates include topic classification, draft preparation, summarization and extracting selected fields. The workflow should keep the original source available for review.

### 3. Can the output be checked before it is used?

- **Yes:** define the validation rule or reviewer.
- **No:** keep the step manual until there is a dependable way to detect an incorrect result.

“The model usually gets it right” is not a verification method. A check should identify required fields, allowed values, source support or the person who approves the result.

### 4. What happens when information is missing or contradictory?

Choose a visible response:

- ask for the missing information;
- route the item to a named person;
- keep the existing record unchanged;
- place the item in an exception queue;
- stop the workflow and record why.

Do not ask AI to invent a missing date, price, customer detail or approval.

### 5. What is the consequence of a wrong action?

Require human review before actions involving:

- a customer-facing promise or individual price;
- payments, refunds or financial records;
- account permissions or credentials;
- legal, medical, employment or safety decisions;
- deletion, publication or another hard-to-reverse change.

The reviewer should see the source, proposed action and reason for the handoff.

### 6. Can failure be found and recovered?

Before launch, define:

- where a failed run appears;
- who is notified;
- whether retrying could create a duplicate;
- what information is safe to log;
- how the team completes the task manually;
- how the workflow is paused.

If the team cannot see or recover from a failure, the step is not ready to run unattended.

## Copyable decision table

Duplicate one row for every step in the proposed workflow.

| Step | Input | Exact rule or interpretation? | Fixed rule, AI assist or human? | Validation | Missing-data response | Owner | Reversible? |
| --- | --- | --- | --- | --- | --- | --- | --- |
| 1 |  |  |  |  |  |  |  |
| 2 |  |  |  |  |  |  |  |
| 3 |  |  |  |  |  |  |  |
| 4 |  |  |  |  |  |  |  |

## Worked example: a new business enquiry

| Step | Choice | Why |
| --- | --- | --- |
| Check that name, reply method and message are present | Fixed rule | Required fields are exact and testable. |
| Detect a repeated submission | Fixed rule | The duplicate key and time window can be defined. |
| Suggest whether the enquiry concerns leads, documents, reporting or another topic | AI assist | The customer writes in natural language and may use unexpected wording. |
| Flag an urgent, sensitive or explicit human request | Fixed rules plus human review | Known terms can trigger the route, but a person owns the conversation. |
| Prepare a reply from approved business information | AI assist | A draft can save time while remaining editable and source-bound. |
| Send an individual quote | Human review | Price and commitments require an accountable person. |
| Update the lead record after approval | Fixed rule | The approved fields and destination are defined. |

This example describes a design pattern using synthetic information. It is not a customer result or evidence that the workflow fits every business.

## Minimum pilot tests

Run at least these cases before launch:

1. A complete, ordinary input.
2. A required field is missing.
3. The same event arrives twice.
4. Two sources disagree.
5. The AI output is unsupported or uncertain.
6. The connected tool is unavailable.
7. A person rejects the proposed action.
8. The workflow is paused and the task is completed manually.

Record the expected route, actual route, reviewer and correction needed. A successful normal case does not prove that the workflow handles exceptions safely.

## Stop conditions

Pause the pilot when:

- a customer-facing action occurs without the agreed approval;
- missing information is filled with an invented value;
- duplicate protection fails;
- a result cannot be traced to its source;
- an account has broader permissions than the workflow needs;
- failures are invisible to the named owner;
- the manual recovery path no longer works.

Fix the process or control before adding volume.

## Next step

Use the [workflow brief](workflow-brief.md) to map the full process, then run the [four launch gates](launch-gates-checklist.md) before a pilot handles real work.

Automations For Business offers a free 15-minute review of one repeated task. No passwords or private customer records are needed for the first conversation.

https://automationsforbusiness.com/contact?utm_source=github&utm_medium=organic&utm_campaign=ai_or_rules_sheet
