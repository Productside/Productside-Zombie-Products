---
name: eol-util-cost-ledger
description: Count what keeping an aging product alive really costs (what it earns, what it eats below the P&L line, and what it forgoes) so the retain, revive, replace, or retire call is argued from the full ledger, not just revenue. Use after Zombie ID, or whenever someone says "but it still makes money."
license: CC-BY-NC-SA-4.0
argument-hint: "[the product, the Zombie ID Card if you have it, and whatever cost and revenue figures you can find]"
intent: >-
  Help a Product Manager make the hidden costs of a declining product visible (support, maintenance,
  compliance, technical debt, and the next bet it crowds out) beside the revenue it still earns, so
  the decision that follows is made on the whole ledger and leadership can see the trade.
type: interactive
theme: product-end-of-life
phase: utility
best-for:
  - "Answering 'but it still makes money' with the costs that sit in other teams' budgets"
  - "Putting a number, or an honest range, on support, maintenance, compliance, and tech debt"
  - "Naming the next bet the product is crowding out"
scenarios:
  - "Revenue is flat, the product looks profitable on the P&L, and engineering says it eats a third of their time"
  - "A leader wants to keep the product because of what it earns, and nobody has counted what it costs"
produces:
  - "Cost Ledger: what it earns, what it eats, what it forgoes, the net, and the confidence behind each line"
depends-on:
  - eol-step1-zombie-id
downstream:
  - eol-step2-revive-or-replace
  - eol-step4-free-the-living
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# Cost Ledger

## Purpose

Produce a **Cost Ledger**: three columns that show what keeping a product alive really costs.

Revenue sits on the P&L, so everyone sees it. The costs are spread across support, engineering, legal, and operations budgets, so nobody sees all of them. The biggest cost, the next bet that never got funded, is on nobody's budget at all. Most of the iceberg is below the waterline.

Use this skill when you need to:

- answer "it still makes money" with the costs it does not show
- give the retain, revive, replace, or retire decision (`eol-step2-revive-or-replace`) a full ledger
- name what the product's capacity would fund instead (`eol-step4-free-the-living`)

This is not a financial model or an accounting allocation. It is an honest, sourced estimate, good enough to change a decision. Ranges are fine; invented precision is not.

## Key Concepts

**Three columns.**

| Column | What goes in it | Where it hides |
|---|---|---|
| **Earns** | Revenue and renewals, plus strategic value a human would recognize (a key account, a contract, a reference customer) | On the P&L; usually overstated by memory |
| **Eats** | Support load, maintenance effort, compliance exposure, technical debt, infrastructure and licenses | Spread across four or more teams' budgets |
| **Forgoes** | The next bet the same people and money would fund, and roadmap room it occupies | On nobody's budget |

*Violation signal:* The ledger has numbers in Earns and blanks in Eats and Forgoes.

**Count people, not just dollars.** Most of a zombie's cost is people's time: engineers patching it, support answering its tickets, a lawyer reviewing its contracts. Count it as a share of a team (for example, "about a third of one squad") before converting to money.

**Label every line.** Each figure is *measured* (from a system or finance), *estimated* (from the team, with how), or *unknown*. Unknowns stay visible; they become the questions for finance.

*Violation signal:* A figure appears with no source, or an unknown is quietly filled with a guess.

**Cost is not cash released.** Keep three views distinct: revenue minus the listed costs for the same period; people capacity that may be redeployed; and outside payments that may be avoided. Loaded salaries stay a cost when people remain employed. A supplier payment is not automatically cancellable, and revenue also disappears on closure. Do not add a person's time to a loaded cost that already includes it. List notice, leases, refunds, severance, and other exit obligations as unknown until supplied. Do not call retirement ROI or a cash saving known when these terms are missing.

**Align the records before netting.** Preserve period, product/bundle scope, and basis (cash, recognized revenue, contract value, forecast, headcount, or FTE). Do not infer calendar or fiscal dates from a year label alone. Honor explicit period links such as “same period” or “the last period”; do not invent a mismatch or mark the supplied alignment assumed. An unstated accounting basis can remain a caveat without erasing a valid listed-cost comparison for an explicitly matched period. A historical invoice does not establish a current expense or contract. Deduplicate identified people and work before converting effort to cost; headcount and FTE are not interchangeable. If the records cannot be aligned, keep the figures separately, leave the net Unknown, and ask for reconciliation. Preserve fixed-term delivery quotes as quoted; do not assume their cost scales linearly with orders or convert a full-cohort average into a marginal cost. Keep a full-take-up comparison distinct from actual orders and payments.

**The forgone column is the point.** A product that breaks even can still be the most expensive thing in the portfolio if it holds the people who would build the next bet. Name the bet, not just "opportunity cost."

## Guided Context Capture

Open with: "We'll fill three columns: what it earns, what it eats, and what it forgoes. Ranges are fine. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered (the Zombie ID Card answers some):

1. `Ledger Q1/5`: What does it earn: annual revenue or renewals, and any account or contract that matters beyond its revenue?
2. `Ledger Q2/5`: What does support spend on it: tickets, people, escalations?
3. `Ledger Q3/5`: What does engineering spend: maintenance, patches, keeping its dependencies alive? As a share of a team is fine.
4. `Ledger Q4/5`: What compliance, security, or vendor exposure does it carry, and what tech debt is it holding in place?
5. `Ledger Q5/5`: If those people and that money were free next quarter, what would you fund?

In **Context dump** mode, sort what was given into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the ledger and label every inferred line *(assumed)*.

**Never invent a figure.** A range is only allowed when it is built from something supplied (a headcount, a ticket count, an invoice, a quote) and the arithmetic is shown. When nothing is supplied, record the **direction** (rising, falling, steady) and mark the amount *unknown*; write "the net cannot be calculated yet" and turn every unknown into a question for finance. A ledger of directions and good questions is a useful result; a ledger of made-up numbers is not.

## Workflow

1. **Fill Earns.** Revenue with its source; strategic value in words, not inflated numbers.
2. **Fill Eats.** One line each for support, maintenance, compliance and security, technical debt, and infrastructure or licenses. People first, then money.
3. **Fill Forgoes.** Name the next bet the capacity would fund and the roadmap room it holds. If nobody can name a bet, say so; that is a finding.
4. **Label every line** measured, estimated, or unknown, with the source.
5. **Net it.** Earns minus Eats, as a range. Then put Forgoes beside it in words.
6. **Write the waterline sentence.** One line a leader can repeat: what it earns above the line, what it eats below.
7. **List the questions for finance.** Every unknown that could change the answer.

## What It Produces

Complete the [Cost Ledger](template.md):

- what it earns, eats, and forgoes, line by line, each labeled
- the net as a range, with the forgone bet beside it
- the waterline sentence
- the open questions for finance

## Human Decision Gate

The PM confirms the figures and their labels before the ledger is shared. The agent drafts estimates; it never presents an estimate as measured.

## Common Pitfalls

**Revenue only.** *Symptom:* "It still makes money" ends the conversation. *Fix:* fill Eats and Forgoes before anyone nets anything.

**False precision.** *Symptom:* a cost to the dollar, or a range, from a guess. *Fix:* build ranges only from supplied inputs, show the arithmetic, and otherwise record direction and mark the amount unknown.

**A nameless opportunity.** *Symptom:* Forgoes says "opportunity cost." *Fix:* name the bet the capacity would fund.

**Allocation fights.** *Symptom:* the meeting turns into how to allocate shared costs. *Fix:* use the direct costs you can see; list allocation as a question for finance.

## References

- [template.md](template.md): the Cost Ledger
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Upstream:** [eol-step1-zombie-id](../eol-step1-zombie-id/SKILL.md) provides the Zombie ID Card
- **Downstream:** [eol-step2-revive-or-replace](../eol-step2-revive-or-replace/SKILL.md) weighs the ledger; [eol-step4-free-the-living](../eol-step4-free-the-living/SKILL.md) moves what it frees
