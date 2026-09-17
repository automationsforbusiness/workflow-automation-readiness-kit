# Workflow Automation Readiness Kit

A free, vendor-neutral set of worksheets for deciding whether a repeated business task is ready to automate.

Use this kit before choosing Zapier, Make, n8n, Power Automate, custom code, or an AI tool. It helps a team describe the work, expose exceptions, decide where a person must approve an action, and define a small test that can be reversed safely.

## Who this helps

This kit is for small-business owners, operations teams and consultants planning practical workflow automation. It is especially useful for:

- lead capture, qualification and handoff;
- customer follow-up and approval steps;
- document and reporting workflows;
- connecting forms, inboxes, spreadsheets, CRMs and task tools;
- AI assistants that need grounded answers and a clear human handoff;
- teams comparing automation tools before committing to a larger build.

The worksheets are vendor-neutral. The included n8n examples demonstrate the method with synthetic data; they are not claims of a customer deployment.

## What is included

- [Workflow brief](workflow-brief.md) — map the trigger, steps, systems, exceptions and desired result.
- [First-automation scorecard](first-automation-scorecard.md) — compare several repeated tasks and choose a narrow, low-risk first pilot.
- [Readiness checklist](readiness-checklist.md) — score whether the process is stable enough for a pilot.
- [Four launch gates](launch-gates-checklist.md) — run a final go/no-go check for required input, duplicate protection, visible failures and human approval.
- [Automation tool selection matrix](automation-tool-selection-matrix.md) — compare built-in automation, no-code platforms, workflow engines, RPA, custom code and AI-assisted workflows against the same operational requirements.
- [Automation value estimator](automation-value-estimator.md) — estimate time value, avoidable rework, operating cost and payback without presenting the estimate as a guaranteed result.
- [Copyable value template](automation-value-template.csv) — enter the same inputs in a simple CSV for your own calculation or spreadsheet.
- [AI assistant pilot checklist](ai-assistant-pilot-checklist.md) — define approved sources, answer boundaries, human handoff, tests and launch checks for a customer or employee assistant.
- [Rules, AI or human review decision sheet](ai-or-rules-decision-sheet.md) — decide which workflow steps need fixed rules, AI-assisted interpretation or an accountable person, then test missing data and failure paths.
- [Free daily-task automation tracker](daily-task-automation-tracker.md) — measure expected runs, completed work, exceptions, review time and estimated minutes released with a copyable CSV for Excel or Google Sheets.
- [Lead-enquiry handoff example](examples/lead-enquiry-handoff.md) — see a completed example with human review and failure handling.
- [n8n lead-enquiry review workflow](n8n/lead-enquiry-review.md) — import a credential-free example that validates two synthetic enquiries and routes them for review.
- [n8n verification record](n8n/verification.md) — see the exact local test boundary and successful branch results from n8n 2.39.6.
- [n8n weekly report review workflow](n8n/weekly-report-review.md) — import a second credential-free example that calculates fictional weekly metrics and routes exceptions for human review.
- [Weekly report verification](n8n/weekly-report-verification.md) — inspect the exact execution boundary and branch results after the local n8n check.
- [n8n customer-message handoff workflow](n8n/customer-message-handoff.md) — inspect a third credential-free example that separates a routine assistant draft from an urgent human-review conversation.
- [Customer-message handoff verification](n8n/customer-message-handoff-verification.md) — inspect the isolated n8n execution result and both final routing states.

## Five-minute quick check

A process is usually a good automation candidate when:

1. The trigger is clear and observable.
2. The inputs are available in a consistent format.
3. The normal path can be written as a short sequence.
4. Exceptions can be named and routed to a person.
5. The result can be checked before it affects a customer or system of record.
6. The team knows what success means and how to pause the workflow.

If several of these are unclear, map the process first. Automating an unstable process usually makes the instability move faster.

## A practical first pilot

Choose one repeated task with a narrow boundary. Run the automation beside the current process on sample or non-sensitive data. Compare the result, failure cases and staff time. Keep a person in the approval step until the outputs are consistently correct.

## Need a second set of eyes?

Automations For Business offers a free 15-minute workflow review. We can help turn a repeated task into a clear first pilot without asking for passwords or private customer records during the first conversation.

https://automationsforbusiness.com/contact

## License

MIT — copy, adapt and share the worksheets with attribution.
