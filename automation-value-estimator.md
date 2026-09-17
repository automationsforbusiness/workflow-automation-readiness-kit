# Automation Value Estimator

Use this worksheet to estimate whether a small workflow-automation pilot is worth testing. It separates time value, error or rework value, operating cost and setup cost so the result can be reviewed instead of guessed.

This is a planning estimate, not a promise of savings or return on investment.

## Step 1: Describe the repeated task

| Input | Your estimate |
| --- | ---: |
| Times the task runs each month |  |
| Minutes currently spent per run |  |
| Minutes expected after automation |  |
| Number of people doing the repeated work |  |
| Cost per working hour |  |

Keep the expected time after automation realistic. Include review, exception handling and any manual approval that will remain.

## Step 2: Calculate time value

```text
Minutes saved per run = current minutes − expected minutes after automation

Monthly hours saved =
  runs per month × minutes saved per run × people affected ÷ 60

Monthly time value = monthly hours saved × cost per working hour
```

If the result is negative, use zero and reconsider the proposed workflow.

## Step 3: Estimate avoidable rework

| Input | Your estimate |
| --- | ---: |
| Errors or rework events per month |  |
| Average cost or staff time value per event |  |
| Percentage the pilot can realistically prevent |  |

```text
Monthly rework value =
  events per month × value per event × preventable percentage
```

Do not include losses that the workflow cannot actually prevent. Keep regulatory, contractual and safety decisions with the responsible person.

## Step 4: Include operating cost

| Monthly cost | Your estimate |
| --- | ---: |
| Automation platform |  |
| AI or API usage |  |
| Monitoring and maintenance |  |
| Human review |  |
| Other recurring cost |  |
| **Total monthly operating cost** |  |

## Step 5: Compare the pilot

```text
Monthly gross value = monthly time value + monthly rework value

Monthly net value = monthly gross value − total monthly operating cost

Estimated payback period in months =
  one-time setup cost ÷ monthly net value
```

Calculate a payback period only when monthly net value is positive. A short payback estimate still does not prove the workflow is reliable or adopted.

## Step 6: Add a confidence range

Create three cases:

| Case | Minutes saved | Preventable rework | Monthly net value |
| --- | ---: | ---: | ---: |
| Conservative |  |  |  |
| Expected |  |  |  |
| Optimistic |  |  |  |

Use the conservative case to decide whether a small pilot is still sensible. Do not use the optimistic case as a sales promise.

## Step 7: Record non-financial checks

Value alone is not enough. Confirm:

- the team can pause the workflow;
- an owner reviews failures and exceptions;
- required approvals remain visible;
- customer-facing outputs can be checked;
- private data and credentials are handled appropriately;
- the current process is stable enough to automate;
- the pilot has a clear stop or rollback condition.

## Synthetic worked example

The figures below are fictional and use a generic currency symbol `$` only to demonstrate the calculation.

| Input | Example |
| --- | ---: |
| Runs per month | 80 |
| Current minutes per run | 12 |
| Expected minutes after automation | 4 |
| People affected | 2 |
| Cost per working hour | $12 |
| Rework events per month | 5 |
| Value per rework event | $8 |
| Preventable percentage | 100% |
| Monthly operating cost | $60 |
| One-time setup cost | $450 |

```text
Monthly hours saved = 80 × 8 × 2 ÷ 60 = 21.33 hours
Monthly time value = 21.33 × $12 = $256.00
Monthly rework value = 5 × $8 × 100% = $40.00
Monthly gross value = $256.00 + $40.00 = $296.00
Monthly net value = $296.00 − $60.00 = $236.00
Estimated payback period = $450 ÷ $236.00 = 1.91 months
```

These example numbers do not represent a customer result. Replace them with observed process data and compare the estimate with actual pilot results.

