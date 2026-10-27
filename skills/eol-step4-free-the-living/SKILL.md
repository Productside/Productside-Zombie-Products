---
name: eol-step4-free-the-living
description: Turn an exit plan into a Capacity Transfer (the people, money, and roadmap room the retirement frees, the next bet that gets them, the trade shown to leadership, and the date the outcome is checked) so the freed capacity moves instead of being absorbed. Use once an exit is planned, and again after the last day of support.
license: CC-BY-NC-SA-4.0
argument-hint: "[the EOL Action Planning Worksheet and the Cost Ledger, or the product and what its exit frees]"
intent: >-
  Help a Product Manager make sure retiring a product actually funds something better: name the
  capacity the exit frees and when, assign it to a next bet with an outcome, show leadership the
  trade, and set a date to check the outcome showed up, so the zombie's budget does not quietly
  become the next zombie's.
type: interactive
theme: product-end-of-life
phase: 4
best-for:
  - "Making the return on a retirement visible to leadership"
  - "Stopping freed capacity from being absorbed by meetings and side projects"
  - "Putting the next bet on the roadmap against an outcome and a date"
scenarios:
  - "The exit plan is approved and nobody has said what the squad works on afterward"
  - "Leadership asks what the company gets for the pain of retiring a product"
  - "Six months after end of support, the team is busy but nobody can name what the capacity went to"
produces:
  - "Capacity Transfer: what is freed and when, the next bet and its outcome, the trade for leadership, and the check-back date"
depends-on:
  - eol-step3-comms-plan
  - eol-util-cost-ledger
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# Free the Living

## Purpose

Produce a **Capacity Transfer**: where the people and money freed by a retirement go, and how anyone will know it worked.

A retirement that does not move capacity is just a smaller zombie. If the freed time is not assigned, it gets absorbed by the next meeting, and the zombie's budget rolls into somebody else's zombie. The return on killing a product is what you fund with it.

Use this skill when you need to:

- name exactly what the exit frees, and when each piece frees up
- assign it to a next bet with an outcome, not just a project
- show leadership the trade in one page
- set the date to check that the outcome showed up

This is not the exit plan (`eol-step3-comms-plan`) or the cost count (`eol-util-cost-ledger`). It uses both.

## Key Concepts

**Capacity frees in stages.** Not everything frees on the last day. Maintenance often drops at notice, support tapers after end of life, licenses and infrastructure end at end of service life. Tie each piece to a phase on the worksheet.

| Phase | What typically frees |
|---|---|
| NSC (notice) | Feature work: the product goes maintenance-only |
| EOS / EOE | Sales and enablement time; roadmap room |
| EOL | Most engineering maintenance; part of support |
| EOSL | The rest of support; infrastructure, licenses, compliance scope |

**Release and acceptance must both be earned.** The worksheet's specific support, return, and contractual obligations override generic phase-release examples. A requested team transfer is a proposal until the receiving owner accepts the work and the budget owner approves it. Keep loaded people cost separate from avoidable outside payments and net cash effects; salary does not disappear when a person moves. If benefit, target, owner, or date is unknown, leave it unknown or explicitly propose it for confirmation; do not claim a measured improvement or accepted commitment.

**Name the capacity, out loud.** "About a third of one squad from February, two support agents from next May" is a transfer. "Some engineering time" is not.

*Violation signal:* The freed capacity is described as "time back" with no people, amount, or date.

**A bet has an outcome.** The next bet is stated as the change it should cause for customers or the business, with a measure. A project name alone is not a bet.

*Violation signal:* The next bet is a feature list with no outcome or measure.

**Show the trade.** Leadership sees one line: we stop spending this on that, and start spending it on this, to get that. The trade is what keeps the budget from drifting back.

**Now, next, later.** Now: name the capacity. Next: put the bet on the roadmap against its outcome. Later: check the outcome, on a date, not "eventually."

*Violation signal:* "Later" has no date.

## Guided Context Capture

Open with: "We'll name what this exit frees, give it to a next bet, and set a date to check it worked. If you have the worksheet and the cost ledger, I need very little else. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered:

1. `Transfer Q1/5`: What does the exit free: people, money, licenses, roadmap room? (The Cost Ledger's Eats column answers this.)
2. `Transfer Q2/5`: When does each piece free up? (The worksheet's phase dates answer this.)
3. `Transfer Q3/5`: What is the next bet, and what outcome should it cause? (The ledger's Forgoes column is the starting point.)
4. `Transfer Q4/5`: Who owns the next bet, and who has to approve the trade?
5. `Transfer Q5/5`: How will you measure the outcome, and when will you check?

In **Context dump** mode, sort what was given into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the transfer and label every inferred item *(assumed)*.

## Workflow

1. **List what is freed**, line by line, from the Cost Ledger: people first, then money, then roadmap room. If there is no Cost Ledger, ask for what is freed directly (`Transfer Q1/5`), or run `eol-util-cost-ledger` first; never invent the amounts. Where the ledger has only directions and unknowns, carry them as-is and make "confirm the freed capacity" the first item in Now.
2. **Date each line** against the worksheet's phases.
3. **State the next bet** as an outcome with a measure, a baseline if known, and a target.
4. **Check the fit.** Does the freed capacity match what the bet needs, and when? Note gaps (for example, skills the squad lacks).
5. **Write the trade** in one line for leadership.
6. **Place it on now, next, later**, with a check-back date.
7. **Name the guardrail**: what stops the capacity being reassigned to maintenance or meetings (for example, the budget line closes at EOSL).

## What It Produces

Complete the [Capacity Transfer](template.md):

- what the exit frees, by line and by phase
- the next bet, its outcome, measure, and owner
- the fit between capacity and bet
- the trade, in one line
- now, next, later, with the check-back date
- the guardrail

## Human Decision Gate

The leader who owns the budget approves the trade, and the next bet's owner accepts the outcome and the check-back date. The agent proposes; it never reassigns people or budget.

## Common Pitfalls

**Time back.** *Symptom:* "The team gets time back." *Fix:* name the people, amount, and date.

**Absorbed capacity.** *Symptom:* six months later nobody can say where the squad went. *Fix:* the guardrail and the check-back date.

**A feature, not a bet.** *Symptom:* the next bet is a backlog. *Fix:* state the outcome and how it will be measured.

**The trade nobody saw.** *Symptom:* leadership hears about the retirement but not what it bought. *Fix:* one line, in the leadership update, at notice and again after EOSL.

## References

- [template.md](template.md): the Capacity Transfer
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Upstream:** [eol-step3-comms-plan](../eol-step3-comms-plan/SKILL.md) provides the phase dates; [eol-util-cost-ledger](../eol-util-cost-ledger/SKILL.md) provides what is freed and the forgone bet
