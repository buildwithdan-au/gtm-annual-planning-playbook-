# GTM Annual Planning — README

**Owner:** Dan McHugh, GSO (Global Sales Operations)
**Last updated:** July 2026

## What this solves

Every SaaS org between roughly $50M and $2B ARR runs into the same annual planning problem: bookings targets get set top-down, but nobody can cleanly answer *"do we have the right people, in the right places, covering the right accounts, with enough pipeline to hit the number?"*

That question breaks into five sub-problems that are usually solved in five different spreadsheets by five different people, none of which agree with each other by Q2:

1. **What kind of account is this, and how much does it matter?** (Segmentation)
2. **Who should own it?** (Territory design)
3. **How many reps do we need to cover it?** (Capacity planning)
4. **Is there enough pipeline in motion to hit the number?** (Pipeline coverage)
5. **How do we report on all of the above, consistently, every quarter?** (QBR reporting)

This toolkit treats those five as one connected system rather than five independent exercises — each artifact's output is the next one's input, so the annual plan and the quarterly reporting cadence stay grounded in the same numbers.

## How I do it

The approach is capacity-based and potential-based rather than headcount-based or revenue-based:

- **Segment first, territory second.** You can't design a fair territory until you know what "high-potential" and "low-potential" mean for an account — so segmentation logic (firmographic + usage + intent signals) is defined before any territory lines are drawn.
- **Size territories to capacity, not to historical revenue.** Equal-account-count and equal-current-ARR territories both under-serve whitespace. Territories are built by summing a composite potential score into equal buckets, then stress-tested against real-world constraints (travel, legal entity, ramp cohort balance).
- **Model headcount need against ramp-adjusted capacity, not raw quota math.** A new hire doesn't carry a full quota from day one — the capacity model blends new-hire ramp productivity and an attrition buffer into the headcount number, so the hiring plan isn't quietly short.
- **Treat pipeline coverage as two numbers, not one.** Raw coverage ratio (pipeline ÷ quota) tells you volume. Stage-weighted coverage (pipeline discounted by historical win rate per stage) tells you quality. The gap between the two is usually the more useful signal.
- **Report on all of it the same way, every quarter, across functions.** The QBR template pulls the same segment definitions, coverage logic, and retention framing through to Marketing (pipeline generation) and CX (retention) so Sales isn't the only function in the room with a number to defend.

## The toolkit

| Artifact | Type | Solves | Feeds into |
|---|---|---|---|
| `segmentation-framework.md` | Framework doc | Defines account tiers (Strategic/Enterprise/Mid-Market/SMB), scoring dimensions, and re-scoring triggers | Territory design, capacity model's segment rows, QBR segment reporting |
| `territory-planning.md` | Framework doc | Territory design principles, sizing methodology, whitespace/TAM analysis, governance cadence | Capacity model's bookings targets, Hiring Plan tab |
| `capacity-model.xlsx` | Calculator (Excel) | How many reps are needed per segment, ramp- and attrition-adjusted, phased into a quarterly hiring plan | QBR's Performance vs. Target and Segment Performance slides |
| `pipeline-coverage-calculator.xlsx` | Calculator (Excel) | Whether open pipeline (raw and stage-weighted) is sufficient to hit remaining quota, by segment | QBR's Pipeline Health & Coverage slide |
| `qbr-template.pptx` | Reporting template (PowerPoint) | Standing quarterly reporting structure across Sales, Marketing (pipeline generation), and CX (retention) | Feeds back into next cycle's segmentation/territory review |

## How the pieces connect

```
Segmentation Framework
        │
        ▼
Territory Planning  ──────────────┐
        │                         │
        ▼                         ▼
Capacity Model            Pipeline Coverage Calculator
        │                         │
        └───────────┬─────────────┘
                     ▼
              QBR Template
       (Sales + Marketing + CX)
                     │
                     ▼
      Feedback into next cycle's
      segmentation & territory review
```

## Annual planning cycle (suggested cadence)

| Phase | Timing | Artifact(s) in use |
|---|---|---|
| Segmentation review & threshold back-test | T-16 weeks before new FY | `segmentation-framework.md` |
| TAM/whitespace refresh, draft territory cuts | T-12 to T-8 weeks | `territory-planning.md` |
| Capacity modeling & hiring plan | T-8 weeks | `capacity-model.xlsx` |
| Territory + quota communication to reps | T-3 weeks | `territory-planning.md` (governance section) |
| Go-live | FY start | All of the above become the year's baseline |
| Quarterly: pipeline health check | Every quarter | `pipeline-coverage-calculator.xlsx` |
| Quarterly: cross-functional QBR | Every quarter | `qbr-template.pptx` |
| Quarterly: light territory rebalancing | Every quarter | `territory-planning.md` (minor rebalancing cadence) |

## Using this toolkit

- Start with the two framework docs (`segmentation-framework.md`, `territory-planning.md`) if you're setting up the planning process for the first time or re-validating it for a new fiscal year — everything else assumes those decisions are already made.
- The two calculators are templates: every blue/yellow-highlighted cell is an input meant to be replaced with real CRM/HR data. Formulas recalculate automatically — don't hardcode over them.
- The QBR template is meant to be reused every quarter with the same slide structure, so quarter-over-quarter comparisons stay apples-to-apples. Only the bracketed placeholders should change.
- None of these are static — the framework docs both call out a re-scoring/rebalancing cadence. Planning is treated as a system that runs continuously, not a one-time exercise each January.

## What's not in here yet

- Compensation plan design (referenced as a dependency in segmentation, not built out here)
- Deal desk / approval workflow documentation
- A consolidated data source — each artifact currently assumes a manual CRM/HR data pull rather than a live feed
