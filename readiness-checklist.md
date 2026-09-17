# Automation readiness checklist

Score each item from **0 to 2**.

- **0** — unknown or inconsistent
- **1** — partly defined
- **2** — clear and repeatable

| Area | Question | Score |
| --- | --- | ---: |
| Trigger | Can the start of the process be detected reliably? |  |
| Inputs | Are required inputs available and consistently formatted? |  |
| Steps | Can the normal path be written without hidden decisions? |  |
| Exceptions | Are common failure and edge cases known? |  |
| Ownership | Is one person responsible for the process and pilot? |  |
| Approval | Are human-review points and timeouts defined? |  |
| Access | Can the workflow use limited, auditable permissions? |  |
| Privacy | Are sensitive fields, retention and deletion needs known? |  |
| Recovery | Can the workflow retry safely or hand work to a person? |  |
| Measurement | Can the team compare time, errors and completion before and after? |  |
| Rollback | Can the automation be paused without losing work? |  |
| Value | Is the likely benefit larger than setup and maintenance effort? |  |

## Interpret the score

- **20–24:** ready for a small, monitored pilot.
- **14–19:** resolve the lowest-scoring areas before building.
- **0–13:** map and stabilize the process first.

The score is a discussion aid, not a guarantee. A low-volume task can still matter when errors are expensive, while a frequent task may be a poor candidate if every case depends on judgment.
