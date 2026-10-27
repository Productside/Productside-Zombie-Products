---
name: eol-util-plc-mapper
description: Place a product on Productside's product lifecycle (design, introduce, grow, mature, decline) and map what its marketing, competition, product, promotion, place, price, and data strategy should be at that stage versus what the team is actually doing. Use before Zombie ID, or whenever a team is running a growth playbook on a declining product.
license: CC-BY-NC-SA-4.0
argument-hint: "[the product and what you know about its sales trend, customers, and current strategy]"
intent: >-
  Help a Product Manager locate a product on the product lifecycle and compare the strategy the
  stage calls for with the strategy the team is running, so mismatches (a growth playbook on a
  declining product) become visible and the right end-of-life or extension work starts on time.
type: interactive
theme: product-end-of-life
phase: utility
best-for:
  - "Placing a product on the lifecycle with evidence rather than opinion"
  - "Spotting a team still running a growth or defend playbook on a declining product"
  - "Setting stage-appropriate objectives and KPIs"
scenarios:
  - "Sales have been flat for a year and the roadmap still reads like a growth plan"
  - "A team wants to know whether to plan an extension, a replacement, or an exit"
produces:
  - "PLC Strategy Map: the four signals, stage and evidence, stage-appropriate posture in seven areas, current posture, gaps, transition questions"
downstream:
  - eol-step1-zombie-id
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# PLC Strategy Mapper

## Purpose

Produce a **PLC Strategy Map**: where the product sits on the lifecycle, what each of seven strategy areas should look like at that stage, what the team is actually doing, and where the two disagree.

The product lifecycle outlines the economic stages a product goes through from design to decline. Go-to-market happens on the left; end of life happens at the right. A team that runs the wrong stage's playbook either starves a growing product or feeds a dying one.

Use this skill when you need to:

- place a product on the lifecycle with evidence
- show leadership that the current plan belongs to a different stage
- set stage-appropriate objectives and KPIs
- decide whether to run `eol-step1-zombie-id` next (mature or declining products)

This is not a forecast. It uses the evidence the team has to name a stage and a posture.

## Key Concepts

**Five stages.**

| Stage | What happens |
|---|---|
| **Design** | Develop concept, create prototype, and plan launch |
| **Introduce** | Launch product, create awareness, and generate initial sales |
| **Grow** | Rapid sales increase, expand market, and build customer base |
| **Mature** | Peak sales, maximize profitability, and defend market position |
| **Decline** | Decreasing sales, manage inventory, and plan phase-out |

**Four signals tell you the stage.** Read these before naming a stage; they are the evidence. Mature is the column to watch: nothing looks wrong yet, and that is where zombies are born.

| Signal | Design | Introduce | Grow | Mature | Decline |
|---|---|---|---|---|---|
| Demand | Unproven demand | Low demand | Growing demand | **Growth slows** | Decreasing demand |
| Competition | Limited competitive evidence | Minimal competition | Growing competition | **High competition** | Falling competition |
| Cost and margin | Costs known, margin unproven | High cost, low margin | Cost and margin improving | **Stable costs, healthy margin** | Increasing costs, decreasing margin |
| Investment | Exploratory investment | Accelerating investment | High investment | **Sustaining investment** | Low investment |

*Violation signal:* The stage is named from the product's age or from one signal alone.

**The stage sets the strategy.** Each stage calls for a different posture in seven areas:

| Area | Design | Introduce | Grow | Mature | Decline |
|---|---|---|---|---|---|
| Marketing objective | Define value proposition | Create awareness | Expand market share | Defend market position | Maximize remaining value |
| Competition | Identify market gaps | Establish value | Differentiate | Emphasize brand loyalty | Consolidate customer base |
| Product | Prototype and test | Core feature set | Enhance and iterate | Optimize extended CX | Streamline support |
| Promotion | Early adopter outreach | Educational content | Success stories | Loyalty incentives | Migration campaigns |
| Place (distribution) | Channel strategy | Targeted placement | Channel expansion | Optimize channels | Profitable channels focus |
| Price | Value-based strategy | Premium or penetration | Competitive adjustment | Value-add bundles | Selective discounting |
| Data strategy | Establish KPIs | Usage patterns | Segment analysis | Predictive modeling | Transition planning data |

**The mature-to-declining questions.** The most expensive transition to miss is mature to declining. For each area, one question tells you which side you are on: Has defending market share stopped being profitable? Are loyalty efforts no longer retaining users? Are legacy support costs becoming unsustainable? Should we consider a product replacement? Are we losing money on certain distribution channels? Are our value-add bundles losing effectiveness? Is data shifting from predictive to transitional?

**The mismatch is the finding.** The map's value is the gap between the posture the stage calls for and the posture the team is running. "Enhance and iterate" on a declining product is how roadmaps feed zombies.

*Violation signal:* The map names a stage but never compares it with what the team is actually doing.

**Question polarity and uncertainty.** Yes always means the declining-side condition holds. Answer the first question literally; never write “Yes, it is not profitable” against a positively phrased question. Missing evidence remains Unknown. Overall margin, subscription counts, and product age do not establish every support, channel, loyalty, or strategy claim. Cite supplied evidence and label inferences rather than filling those gaps as facts.

## Guided Context Capture

Open with: "We'll place this product on the lifecycle and compare what the stage calls for with what the team is doing. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered:

1. `PLC Q1/4`: What is the product, and how long has it been in market?
2. `PLC Q2/4`: What are sales, usage, and margin doing: rising fast, rising slowly, flat, or falling?
3. `PLC Q3/4`: What is the team investing in right now: new features, loyalty, support cost reduction, migration?
4. `PLC Q4/4`: How do you price and sell it today: premium, discounts, bundles, which channels?

In **Context dump** mode, sort what was given into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the map and label every inferred item *(assumed)*.

## Workflow

1. **Read the four signals** (demand, competition, cost and margin, investment) and mark which stage each points to.
2. **Name the stage** from the signals, with one or two lines of evidence. If they split between stages (for example, late mature), say so.
3. **Fill the stage posture** for all seven areas from the table above.
4. **Fill the current posture**: what the team is actually doing in each area.
5. **Mark the gaps.** For each area: aligned, behind (still running an earlier stage's playbook), or ahead.
6. **If mature or declining, answer the seven transition questions** (yes, no, unknown).
7. **Recommend the next move:** keep the stage plan, plan an extension, or run `eol-step1-zombie-id`.

## What It Produces

Complete the [PLC Strategy Map](template.md):

- stage and evidence
- stage posture and current posture in seven areas, with the gap marked
- the transition questions (mature or declining products)
- the recommended next move

## Human Decision Gate

The PM confirms the stage before the map is shared. Stage calls are judgments; the evidence goes with them.

## Common Pitfalls

**Stage by age.** *Symptom:* "it's been out five years, so it's mature." *Fix:* use sales, margin, and usage trends, not age.

**Defend forever.** *Symptom:* every area reads "mature" for years. *Fix:* answer the transition questions; long maturity is often unacknowledged decline.

**Growth playbook on a declining product.** *Symptom:* the product row says "enhance and iterate" while sales fall. *Fix:* mark it behind, and run Zombie ID.

## References

- [template.md](template.md): the PLC Strategy Map
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Downstream:** [eol-step1-zombie-id](../eol-step1-zombie-id/SKILL.md) for mature or declining products
