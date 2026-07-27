# Segmentation Framework: Best Practice for $50M–$2B ARR SaaS Organizations

## Purpose
This framework defines how to segment accounts and prospects so that coverage model, motion, and resourcing (sales, CS, marketing) match account potential and complexity. It's the layer that sits *underneath* territory design — territories carve up the map; segmentation decides which rules of engagement apply to each account on it.

---

## 1. Guiding Principles

1. **Segment by potential and complexity, not just current size.** A small account with high expansion potential may warrant more investment than a large, saturated one.
2. **One segmentation model should drive every downstream decision** — routing, quota, comp, playbook, CS tier, marketing treatment. If Sales and CS use different segment definitions, the org loses a shared language for prioritization.
3. **Segments must be re-scored on a cadence, not fixed at acquisition.** An account's segment can and should change as it grows, churns risk rises, or usage shifts.
4. **Fewer, clearer segments beat many overlapping ones.** Most orgs at this scale converge on 3–5 primary segments; more than that usually signals unresolved debate rather than real distinctions.
5. **Segmentation should be defensible with data, not just intuition.** Thresholds (employee count, ARR, usage) should be back-tested against actual win rate, expansion rate, and CAC:LTV by band before being finalized.

---

## 2. Core Segmentation Dimensions

Most SaaS orgs combine two to four of the following, rather than relying on one alone:

| Dimension | What it captures | Common at this scale |
|---|---|---|
| **Firmographic** (employee count, company revenue) | Rough proxy for deal size and buying complexity | Nearly universal — foundational layer |
| **Product usage / engagement** | Depth of adoption, seat penetration, feature usage, login frequency | Increasingly primary signal for expansion-stage companies |
| **Revenue / ARR band** | Current contract value | Used for CS/AM tiering more than initial sales routing |
| **Industry / vertical** | Buying behavior, regulatory needs, competitive landscape | Applied as an overlay once volume justifies specialization |
| **Deal complexity** (multi-stakeholder, security review, procurement) | Sales motion required (self-serve vs. high-touch) | Common differentiator between SMB and Enterprise motions |
| **Strategic value** (logo value, reference-ability, expansion ceiling) | Accounts worth over-investing in relative to current size | Used for named/strategic account carve-outs |
| **Growth trajectory / intent signals** | Hiring velocity, funding events, tech stack changes, website intent data | Increasingly used to flag "surge" accounts worth re-segmenting mid-cycle |

**Practical guidance:** firmographic + usage is the most common two-dimensional starting point. Vertical and strategic-value overlays are added once a segment reaches enough volume (typically 50–100+ accounts) to justify dedicated coverage.

---

## 3. Typical Segment Tiers by Company Stage

| ARR Stage | Typical Segment Structure |
|---|---|
| $50M–$150M | SMB / Mid-Market / Enterprise (3-tier, firmographic-driven) |
| $150M–$500M | SMB (self-serve/velocity) / Commercial (Mid-Market) / Enterprise / Strategic (named top accounts) |
| $500M–$1B | Above, plus vertical overlays in 2–4 priority industries; usage-based re-segmentation triggers for expansion |
| $1B–$2B | Full multi-dimensional model: Segment × Vertical × Usage tier, often with a distinct "Strategic/Global" tier for top 1–2% of accounts requiring executive sponsorship and multi-year account planning |

### Example 4-tier structure (most common at $150M+ ARR)

| Tier | Typical Profile | Motion | Primary Owner |
|---|---|---|---|
| **Strategic / Named** | Top 1–5% of TAM by potential; often existing large logos or greenfield accounts with outsized ceiling | High-touch, multi-threaded, exec sponsorship | Dedicated AE + AM, CBO/exec air cover |
| **Enterprise** | Large organizations, complex buying committee, security/procurement review | Consultative, longer cycle | Enterprise AE |
| **Mid-Market / Commercial** | Mid-sized organizations, moderate complexity | Structured sales process, shorter cycle | Commercial AE |
| **SMB / Velocity** | Small organizations, low deal complexity, often self-serve eligible | High-volume, templated, PLG-assisted | Inside sales / self-serve motion |

---

## 4. Scoring Methodology

### Step 1 — Define the composite potential score
Build a weighted score per account, typically combining:
- **Firmographic fit** (30–40%): revenue band, employee count, industry fit against ICP
- **Usage/engagement signal** (20–30%): active seats, feature adoption depth, login frequency (existing customers only)
- **Growth/intent signal** (15–25%): hiring velocity, funding events, website/content engagement, technographic signals
- **Strategic value** (10–20%): reference-ability, logo prestige, expansion ceiling, competitive displacement value

### Step 2 — Validate thresholds against outcomes
Before finalizing tier cutoffs, back-test candidate thresholds against:
- Historical win rate by band
- Expansion/net revenue retention by band
- CAC:LTV ratio by band
- Sales cycle length by band

A well-calibrated model shows a meaningful step-change in these metrics at each tier boundary — if metrics are flat across a proposed boundary, the segments aren't actually distinct and should be merged.

### Step 3 — Automate scoring in CRM/CDP
Segment scores should be calculated systematically (CRM formula field, CDP model, or reverse-ETL pipeline), not maintained manually in spreadsheets — manual scoring drifts out of date within a quarter and becomes a source of rep disputes.

---

## 5. Segment Migration & Re-scoring

Accounts move between segments as they grow, contract, or change behavior. Define explicit triggers:

| Trigger | Example | Action |
|---|---|---|
| **Usage surge** | Seat count or feature adoption crosses upper threshold | Flag for re-tier review, potential AE handoff to higher segment |
| **Funding/M&A event** | Target account raises a round or is acquired | Re-score firmographic component, notify owning AE |
| **Renewal risk** | Usage decline, support escalations, exec sponsor departure | Flag to CS for intervention regardless of segment tier |
| **Contract expansion** | ARR crosses tier boundary at renewal | Formal handoff to appropriate segment owner with account history transfer |
| **Scheduled review** | Quarterly | Full re-score against latest firmographic/usage data |

**Handoff discipline matters more than the scoring model itself.** Most segmentation friction in the field comes from poorly managed account transitions (losing context, relationship discontinuity) — not from disagreement over the scoring logic. Define a standard handoff packet (account history, open opportunities, relationship map, renewal date) before enabling automatic re-tiering.

---

## 6. Segmentation's Downstream Dependencies

A segmentation model earns its keep by driving consistent decisions across functions. Confirm alignment on each:

- **Sales**: routing rules, quota design, comp plan differentiation, playbook/methodology per tier
- **Customer Success**: CS-to-account ratio, QBR cadence, proactive vs. reactive coverage model
- **Marketing**: ABM investment allocation, content/messaging differentiation, event/field marketing targeting
- **Product**: roadmap prioritization signal (which segment's needs get weighted most heavily)
- **Deal desk/Legal**: approval thresholds and contract terms flexibility by tier
- **Executive sponsorship program**: which tier triggers exec-to-exec relationship assignment

If any function is using a different segment definition than the one Sales Ops maintains, reconcile before the next planning cycle — divergent segment definitions across functions is one of the most common causes of coverage gaps and duplicated outreach.

---

## 7. Common Anti-Patterns to Avoid

- **Segmenting only on firmographics** — misses usage-based expansion potential and strategic value, especially for existing customers.
- **Too many tiers** — more than 4–5 segments usually reflects unresolved organizational debate, not real market distinction.
- **Static segmentation** — accounts assigned once at acquisition and never re-scored, missing growth or risk signals.
- **Manual, spreadsheet-based scoring** — drifts out of date, creates disputes, doesn't scale past a few hundred accounts.
- **Segment definitions that differ by function** — Sales, CS, and Marketing each running their own version undermines coordinated coverage.
- **No validation against outcomes** — thresholds set by intuition or historical precedent rather than back-tested against win rate/NRR/CAC:LTV data.
- **Ignoring handoff quality during migration** — a technically correct re-tier that loses relationship context creates more friction than it solves.

---

## 8. Suggested Review Cadence

| Activity | Frequency | Owner |
|---|---|---|
| Full segmentation model review (dimensions, weights, thresholds) | Annually, ahead of territory/FY planning | Sales Ops / RevOps with cross-functional input |
| Threshold back-testing against outcomes | Annually (feeds into above) | Sales Ops / Analytics |
| Individual account re-scoring | Quarterly (automated) | Systems/RevOps |
| Ad hoc re-tier triggers (funding events, usage surge, M&A) | Continuous, event-driven | CRM automation + Sales Ops review |
| Cross-functional alignment check (Sales/CS/Marketing using same definitions) | Semi-annually | RevOps |

---

*This framework should be read alongside the territory planning model — segmentation defines "what kind of account is this," territory design decides "which rep or team owns it." Recommend validating proposed tier thresholds against Xero's own historical win-rate and NRR data by band before finalizing cutoffs.*
