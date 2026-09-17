# Free daily-task automation tracker

This CSV helps a team measure one recurring task before and during a small automation pilot. Open it in Excel, Google Sheets or another spreadsheet application that supports standard formulas.

[Download the copyable CSV](daily-task-automation-tracker.csv)

The tracker uses a synthetic sample row. Replace or delete that row before using the sheet. Do not enter passwords, API keys, confidential customer details or sensitive employee information.

## What the tracker measures

| Column | What to enter |
| --- | --- |
| `date` | The day or reporting period being measured. |
| `workflow_name` | A plain-language task name, such as “lead handoff” or “weekly report preparation.” |
| `owner` | The role responsible for reviewing exceptions and the final result. |
| `expected_runs` | How many times the task should have run in the period. |
| `completed_runs` | How many runs reached the agreed useful result. |
| `exceptions` | Runs that stopped, failed, lacked information or required unusual handling. |
| `manual_minutes_per_run` | A measured estimate of the old manual work per completed run. |
| `remaining_minutes_per_run` | The manual work that remains after automation, including ordinary checks. |
| `review_minutes_total` | Additional time spent reviewing outputs and exceptions during the period. |
| `estimated_minutes_released` | Formula: completed runs × (manual minutes − remaining minutes) − review minutes. |
| `completion_rate` | Formula: completed runs ÷ expected runs. |
| `exception_rate` | Formula: exceptions ÷ completed runs. |
| `status` | A short state such as `Pilot`, `Review exceptions`, `Paused` or `Ready for owner review`. |
| `next_action` | One concrete owner action before the next period. |

Format `completion_rate` and `exception_rate` as percentages after opening the CSV.

## How to use it

### 1. Measure the task before automation

Track a normal period using the current process. Record real completed runs, exception count and manual time. A remembered estimate is less useful than several timed examples.

### 2. Define the useful result

“The workflow ran” is not enough. Define what counts as complete: the lead has an owner and next action, the report totals reconcile, or the document has all required fields and is ready for review.

### 3. Run a bounded pilot

Use representative non-sensitive data and keep the current process available. The owner should review the result before it affects a customer, payment, access permission or system of record.

### 4. Record exceptions honestly

Count missing information, duplicates, failed connections, rejected approvals and results that needed correction. Do not remove an exception from the count merely because a person fixed it later.

### 5. Compare periods carefully

The formulas estimate operational time released. They do not prove cash savings, revenue gains or staff reductions. Compare periods only when volume, task definition and review requirements are reasonably similar.

## Worked synthetic example

The included sample expects 25 lead handoffs. Twenty-three reached the defined result, two required exception handling, the old task took eight minutes per run, the new process still needs three minutes per completed run, and the team spent 20 additional minutes reviewing the period.

The formula estimates 95 minutes released:

`23 × (8 − 3) − 20 = 95`

The completion rate is 92%, and the exception rate is approximately 8.7%. These numbers are fictional and illustrate the calculation only.

## Review questions

- Did the expected event start every run?
- Were duplicate events stopped before creating another action?
- Were missing or contradictory inputs visible?
- Did the owner see every exception?
- Did a person approve high-impact actions?
- Could the team pause the workflow and complete the task manually?
- Did review time fall, stay stable or increase?

If failures are hidden, approvals are bypassed or the manual recovery path no longer works, pause the pilot and fix the control before increasing volume.

Use the [rules, AI or human-review decision sheet](ai-or-rules-decision-sheet.md) to assign the right control to each step. Use the [automation value estimator](automation-value-estimator.md) for a broader cost and payback estimate.

Automations For Business offers a free 15-minute workflow review. No passwords or private customer records are needed for the first conversation.

https://automationsforbusiness.com/contact?utm_source=github&utm_medium=organic&utm_campaign=daily_task_tracker
