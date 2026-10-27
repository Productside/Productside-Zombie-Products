---
name: eol-step2-revive-or-replace
description: Turn a Zombie ID Card into one decision (revive with an extension play, replace with a replacement play, or retire) argued from evidence, with one named Decider. Use after a product is identified as declining or a zombie, before anyone plans an exit.
license: CC-BY-NC-SA-4.0
argument-hint: "[the Zombie ID Card, or the product and its evidence]"
intent: >-
  Help a Product Manager and a named Decider choose between a lifecycle extension play, a
  replacement play, and retirement, arguing each from current evidence rather than sunk cost,
  so the product leaves limbo with a recorded decision and a clear next step.
type: interactive
theme: product-end-of-life
phase: 2
best-for:
  - "Making a revive, replace, or retire call that survives a skeptical executive"
  - "Arguing all three options fairly, including the one nobody wants"
  - "Stopping 'we'll revisit it next quarter' from becoming the decision"
scenarios:
  - "The Zombie ID Card says zombie and the room still cannot agree what to do"
  - "A senior leader wants to revive the product because of what it used to earn"
  - "A replacement exists, but nobody has decided to move customers to it"
produces:
  - "Decision Record: the call, the Decider, the reason, the evidence, what must be true, and the next step"
depends-on:
  - eol-step1-zombie-id
combine-with:
  - eol-util-cost-ledger
downstream:
  - eol-step3-comms-plan
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# Revive, Replace, or Retire

## Purpose

Produce a **Decision Record**: one call, made out loud by one named Decider, with the reason written down.

There are three honest moves for a declining product. There is also a fourth one that everyone picks: do nothing and revisit it next quarter. That fourth move is how products become zombies. This skill does not offer it.

Use this skill when you need to:

- choose between reviving, replacing, and retiring a product with evidence, not nostalgia
- argue each option fairly before the Decider speaks
- record a reason a human would recognize, so the product cannot drift back into limbo
- hand the decision to the communications plan (`eol-step3-comms-plan`)

This is not the communications plan. It decides *what* happens to the product. Who hears it, when, and in what order is the next step.

## Key Concepts

**Three moves, defined by the lifecycle.**

| Move | Lifecycle play | What it is | Good reasons |
|---|---|---|---|
| **Revive** | Extension play | Introduce a new variant or additional features to the existing product line to extend its life | Expand into new customer segments. Meet diverse customer needs. Differentiate from competitors. Boost sales with new variants. Strengthen brand loyalty. |
| **Replace** | Replacement play | Introduce a new product to take the place of the existing one, offering similar or improved features while the old product is phased out. Go-to-market and end-of-life happen at the same time. | Address supply issues. Reduce production costs. Eliminate obsolete or unused features. Align with strategic business goals. Comply with regulatory issues. |
| **Retire** | End of life | Phase out, support, and discontinue the product while managing customer transitions, operational changes, and regulatory compliance | The need is gone, the costs beat the value, and no extension or replacement earns its keep. |

**There is no fourth option.** "Continue as is" and "revisit next quarter" are not on the list. A product that survives does so because someone bet on it again, on current evidence.

*Violation signal:* The record says "keep for now," "deprioritize," or "revisit," with no move chosen.

**Argue from today's evidence, not sunk cost.** The case for reviving must hold up as if the product did not exist yet. If the argument only works because of what has already been spent, it is sunk cost dressed as a decision. The test: would you start this today, knowing what you now know?

*Violation signal:* The revive case cites how much was invested, how long it has run, or what it used to earn.

**Three kinds of evidence.** Every move is argued from the same three sources:

- **Customer evidence:** what customers *do*, not what one loud customer says
- **Lifecycle signals:** where the product sits and what the telltale questions said
- **Business outcomes:** whether the product still moves a number the business cares about

*Violation signal:* "One customer really loves it" is the strongest evidence for a move.

**One Decider, by name.** One person with authority says the word. A committee produces alignment, and alignment adjourns. If the Decider is a group, name the one person who breaks ties.

*Violation signal:* The record says "we aligned on" rather than who decided.

## Guided Context Capture

Open with: "We'll argue revive, replace, and retire fairly, then stop for your Decider to choose. If you have the Zombie ID Card, I need very little else. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered (the Zombie ID Card answers most of these):

1. `Decision Q1/5`: What did the Zombie ID Card conclude, and what were the strongest reasons on each side?
2. `Decision Q2/5`: Is there a segment or variant that would genuinely want an extended version? What is the evidence?
3. `Decision Q3/5`: Does a replacement exist or is one planned? Could customers move to it?
4. `Decision Q4/5`: What commitments constrain retirement: contracts, SLAs, regulation, key customers?
5. `Decision Q5/5`: Who is the Decider? One name.

In **Context dump** mode, sort what was given into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the record and label every inferred item *(assumed)*. Never infer evidence that was not supplied.

## Workflow

1. **Restate the finding.** One line from the Zombie ID Card, including the verdict and the lingering forces.
2. **Argue revive.** What extension play would it take, which reasons from the extension list apply, and what customer evidence and business outcomes support it. Apply the sunk-cost test and write the answer.
3. **Argue replace.** What replaces it, which reasons from the replacement list apply, and whether customers can realistically move. Note that go-to-market and end-of-life will run at once.
4. **Argue retire.** What ending it frees up, what it costs customers, and which commitments must be honored.
5. **Weigh the evidence.** For each move, rate customer evidence, lifecycle signals, and business outcomes as strong, weak, or missing.
6. **Write what must be true.** For each move, the one or two conditions that would have to hold for it to be right.
7. **Stop for the Decider.** Present `Revive`, `Replace`, `Retire`, and `Other (specify)`, each with its strongest case, its weakest point, and what it frees or costs. Do not choose for them.
8. **Record the call.** The word, who said it, the reason in their words, and what they weighed differently.
9. **Set the next step.** Retire or replace: hand to `eol-step3-comms-plan`. Revive: name the extension play, its owner, and the evidence that will be checked, and by when.

If the evidence is thin, still argue all three moves, show what each case cannot establish, and stop for the Decider. Thin evidence weakens every case; it does not authorize the agent to decide.

## What It Produces

Complete the [Decision Record](template.md):

- the finding carried from the Zombie ID Card
- revive, replace, and retire, each argued with its evidence and its weakest point
- the evidence rating for each move
- what must be true for each move
- the call, the Decider, and the reason in their words
- the next step and its owner

## Human Decision Gate

The Decider says one word: revive, replace, or retire. Record the word, who said it, the reason, and the date. The agent never makes the call.

## Common Pitfalls

**The fourth option sneaks back.** *Symptom:* "Let's keep it for now and revisit." *Fix:* that is a decision to fund a zombie; ask the Decider to choose one of the three.

**Revive on nostalgia.** *Symptom:* the revive case is what the product used to earn. *Fix:* apply the sunk-cost test and require current customer evidence.

**Replace without a path.** *Symptom:* replace is chosen but nobody can say how customers move. *Fix:* write the migration path into "what must be true" before recording the call.

**Retire without commitments.** *Symptom:* retire is chosen before legal and finance have looked at contracts and forecasts. *Fix:* list the commitments in the retire case; the comms plan starts with legal and finance.

## References

- [template.md](template.md): the Decision Record
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Upstream:** [eol-step1-zombie-id](../eol-step1-zombie-id/SKILL.md) provides the Zombie ID Card; [eol-util-cost-ledger](../eol-util-cost-ledger/SKILL.md) gives the business-outcomes evidence its full ledger
- **Downstream:** [eol-step3-comms-plan](../eol-step3-comms-plan/SKILL.md) turns a retire or replace call into the EOL Action Planning Worksheet
