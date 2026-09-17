# First-automation scorecard

Use this scorecard when several repeated tasks could be automated but the team needs one safe place to start.

List up to three candidates. Score each factor from **0 to 2**.

- **0** — weak, unknown or high risk
- **1** — partly suitable
- **2** — strong and clearly suitable

## Compare the candidates

| Factor | What to check | Candidate A | Candidate B | Candidate C |
| --- | --- | ---: | ---: | ---: |
| Repetition | Does the same task happen often enough to test repeatedly? |  |  |  |
| Time spent | Does the task consume noticeable staff time? |  |  |  |
| Rule clarity | Can the normal decisions be explained without hidden judgment? |  |  |  |
| Input quality | Are the required inputs usually available and consistent? |  |  |  |
| Exception visibility | Can missing data, duplicates and failures be detected? |  |  |  |
| Review ease | Can a person check the result before it affects a customer or source of truth? |  |  |  |
| Low blast radius | Can a mistake be contained to a small sample or draft? |  |  |  |
| Reversibility | Can the workflow be paused and the old process restored easily? |  |  |  |
| **Total** | Add the eight scores. Maximum: 16. |  |  |  |

## Use the score

- **13–16:** strong candidate for a small, monitored pilot.
- **9–12:** promising, but resolve the lowest-scoring factor first.
- **0–8:** choose a clearer or safer task, or map the process before automating it.

The highest score is not an automatic decision. Prefer the candidate whose result can be reviewed safely with sample or non-sensitive data.

## Stop before building if

- every case depends on expert judgment;
- the source data is incomplete or changes format frequently;
- the workflow would need broad administrator permissions;
- a wrong result could immediately charge, delete, publish or message without review;
- nobody owns failures, approvals or rollback;
- success cannot be measured against the current process.

## Define the first pilot

**Chosen task:**  
**Owner:**  
**Sample size:**  
**Sample or non-sensitive data:**  
**Human-review point:**  
**Success measure:**  
**Pause condition:**  
**Rollback method:**  

Run the pilot beside the current process. Compare completion time, errors, rework and staff effort. Expand only after the result is consistently correct and the failure path is visible.

## Next step

Use the [workflow brief](workflow-brief.md) to map the selected task. Then use the [automation readiness checklist](readiness-checklist.md) before choosing tools or connecting live systems.
