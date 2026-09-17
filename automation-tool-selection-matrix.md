# Automation tool selection matrix

Choose an approach after the workflow is mapped. A familiar tool can still be the wrong fit when it lacks a required connector, approval step, audit trail or recovery path.

This matrix compares **approaches**, not product marketing claims. Confirm current features, limits, data handling and pricing with each vendor before committing.

## Common approaches

| Approach | Often fits | Main strengths | Questions to answer first |
| --- | --- | --- | --- |
| Built-in app automation | A short process inside one existing business app | Fewer systems, simpler ownership, familiar interface | Can it cover the whole trigger-to-result path and show failures? |
| No-code integration platform | Connecting common cloud apps with straightforward triggers and actions | Fast setup, broad connector catalog, accessible to non-developers | Are the needed branches, approvals and error controls available on the intended plan? |
| Visual workflow engine | Multi-step integrations, data transformation and controlled branching | Flexible logic, reusable steps, stronger technical control | Who will host, monitor, update and secure it? |
| Robotic process automation | A legacy interface with no suitable API | Can reproduce structured interface steps | How will layout changes, pop-ups, session expiry and partial completion be handled? |
| Custom code | Unusual rules, high volume or a product-specific integration | Maximum control and testability | Is the extra build, security, deployment and maintenance effort justified? |
| AI-assisted workflow | Classification, drafting or extraction where inputs vary | Handles language and flexible content | What approved sources, confidence boundary, privacy rules and human review are required? |

Many reliable systems combine approaches. For example, a form may collect data, a workflow engine may validate it, an AI step may draft a summary, and a person may approve the final customer-facing action.

## Score the actual requirement

Give each candidate **0 to 3** for every requirement.

- **0** — missing or unacceptable
- **1** — possible with a major workaround
- **2** — adequate with manageable limits
- **3** — strong fit with clear evidence

Set the weight to **1** for useful requirements, **2** for important requirements and **3** for requirements that can block launch. Multiply score by weight.

| Requirement | Weight | Candidate A | Candidate B | Candidate C |
| --- | ---: | ---: | ---: | ---: |
| Required app connectors or usable APIs |  |  |  |  |
| Trigger reliability and duplicate protection |  |  |  |  |
| Branching, validation and exception routing |  |  |  |  |
| Human approval before consequential actions |  |  |  |  |
| Least-privilege authentication |  |  |  |  |
| Sensitive-data handling and retention controls |  |  |  |  |
| Logs, alerts and run history |  |  |  |  |
| Safe retry, rollback and manual recovery |  |  |  |  |
| Expected volume and rate limits |  |  |  |  |
| Team skill and maintainability |  |  |  |  |
| Setup effort and recurring operating cost |  |  |  |  |
| Portability and exit path |  |  |  |  |

## Apply launch gates

A high total does not override a critical failure. Mark a candidate **not ready** when any of these are unresolved:

- a required system cannot be connected through an approved method;
- the workflow needs more access than the business can safely grant;
- sensitive information would be stored or sent somewhere unacceptable;
- a customer-facing or financial action has no required approval step;
- failures cannot be detected or recovered without losing work;
- no one owns monitoring and maintenance;
- the cost model is unknown at expected volume.

## Run a small proof

Test the two strongest candidates with the same synthetic examples and edge cases. Record:

1. setup time;
2. successful normal-path runs;
3. duplicates prevented;
4. exceptions caught and routed;
5. time needed to understand a failure;
6. manual recovery steps;
7. expected monthly operating cost;
8. who can maintain the workflow six months later.

Choose the simplest candidate that passes every launch gate. Keep the runner-up documented as a fallback if a connector, price or policy changes.

## Decision record

| Item | Decision |
| --- | --- |
| Workflow being evaluated |  |
| Required systems |  |
| Non-negotiable launch gates |  |
| Candidates tested |  |
| Synthetic test cases used |  |
| Selected approach |  |
| Why it won |  |
| Known limitations |  |
| Owner and review date |  |

The matrix supports a reasoned comparison; it does not guarantee implementation success or future vendor availability.

