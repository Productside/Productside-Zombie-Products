---
name: eol-step1-zombie-id
description: Decide whether an aging product is healthy, declining, a zombie, or just ugly, using Productside's business and product reasons to retire and the mature-to-declining telltale questions. Use when a product keeps consuming capacity and nobody can say whether it should live.
license: CC-BY-NC-SA-4.0
argument-hint: "[the product, and whatever evidence you have: revenue trend, support load, customers, strategy]"
intent: >-
  Help a Product Manager tell a declining product from a zombie, using the business and product
  reasons to retire a product and the lifecycle telltale questions, so the team stops funding a
  product by default and hands a clear finding to the retain, revive, replace, or retire decision.
type: interactive
theme: product-end-of-life
phase: 1
best-for:
  - "Naming whether a product is a zombie, with evidence, before anyone argues about it"
  - "Separating good reasons to retire from emotional or image-driven ones"
  - "Surfacing the forces that keep a product alive: inertia, sunk cost, politics, legacy commitments"
scenarios:
  - "A product has stopped growing, still has loyal customers, and nobody wants to pull the plug"
  - "Leadership wants to kill a product because it looks dated, and you are not sure that is a reason"
  - "Support and maintenance keep growing on a product nobody owns"
produces:
  - "Zombie ID Card: verdict, evidence by reason, telltale answers, lingering forces, decision owner"
depends-on: []
combine-with:
  - eol-util-plc-mapper
downstream:
  - eol-util-cost-ledger
  - eol-step2-revive-or-replace
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# Zombie ID

## Purpose

Produce a **Zombie ID Card**: a one-page finding that says whether a product is **healthy**, **declining**, a **zombie**, or **just ugly**, with the evidence behind the call.

Every product ends up in decline. That is the lifecycle, not a failure. A product becomes a zombie when it sits in decline with the reasons to retire it in plain view, and nobody owns the decision to stop. This skill makes that line visible.

Use this skill when you need to:

- decide whether a long-running product is a zombie before the team argues about what to do with it
- separate business and product reasons from image, nostalgia, or politics
- show leadership what is keeping the product alive
- hand a clear, evidenced finding to the retain, revive, replace, or retire decision (`eol-step2-revive-or-replace`)

This is not the decision itself. The Zombie ID Card says what the product *is*. Whether to retain, revive, replace, or retire it is the next step, with its own evidence bar and its own Decider.

## Key Concepts

**Diagnosis is not disposition.** Healthy, Declining, Zombie and Just ugly describe the finding, not the chosen motion. Retain operates as is; Revive extends this product; Replace introduces a successor; Retire closes without one. Recommend investigation from this card; the named human chooses in step 2.

**Decline is a stage. Zombie is a failure to decide.** A declining product with a plan is healthy lifecycle management. A declining product that keeps getting funded because no one has decided is a zombie. The difference is ownership of the decision, not the revenue curve. Preserve a supplied named owner who is actively reviewing options; no final word or unassigned transition owner does not erase that ownership. Do not infer inertia or an ownership vacuum merely because that review has not concluded.

*Violation signal:* The card calls a product a zombie only because sales are falling, without asking who owns the decision.

**Ugly is not dead.** A product can look dated and still earn its keep. The test is whether you would fund it today if it did not exist, not whether it embarrasses the brand. For example, an unfashionable product that customers still value may deserve continued investment. Appearance alone is not evidence for retirement.

*Violation signal:* The only reasons recorded are "it looks old," "a new executive wants a fresh start," or "nobody remembers why it exists."

**Two kinds of good reasons.** Productside groups the reasons to retire a product into two families. Use these exact families.

| Family | Category | Signals |
|---|---|---|
| **Business reasons** | Financial viability | Costs now exceed product revenue. High support costs drain resources. Operating at a significant loss. |
| | Strategic alignment | Conflicts with new company strategy. Exiting this specific market. Refocusing on core business priorities. |
| **Product reasons** | Solution replacement | A new internal product supersedes it. A superior, modern solution has been developed. Users are being migrated to a new platform. |
| | Market irrelevance | Market and user needs have shifted. Technology makes the solution obsolete. The core problem no longer exists. |

**The telltale questions.** When a product moves from mature to declining, its posture changes in seven areas. Each area has a question that tells you which side you are on.

| Area | Mature posture | Declining posture | The question |
|---|---|---|---|
| Marketing objective | Defend market position | Maximize remaining value | Has defending market share stopped being profitable? |
| Competition | Emphasize brand loyalty | Consolidate customer base | Are loyalty efforts no longer retaining users? |
| Product | Optimize extended CX | Streamline support | Are legacy support costs becoming unsustainable? |
| Promotion | Loyalty incentives | Migration campaigns | Should we consider a product replacement? |
| Place | Optimize channels | Profitable channels focus | Are we losing money on certain distribution channels? |
| Price | Value-add bundles | Selective discounting | Are our value-add bundles losing effectiveness? |
| Data strategy | Predictive modeling | Transition planning data | Is data shifting from predictive to transitional? |

**Read each question literally.** Every Yes names a declining-side condition, including the first question. Missing evidence is **Unknown**, not No or Not present. “No evidence of migration” is Unknown; a supplied record affirmatively showing no migration can support Not present. Profitable overall economics do not prove support costs or every channel are healthy; falling subscriptions do not by themselves prove a loyalty program failed. Label proxy-based inferences and cite their source. Count Yes, No, and Unknown separately; the count is a diagnostic, not a majority-vote verdict.

**What keeps a zombie alive.** Zombies survive on four forces, not on customer value: **inertia** (nobody chose it, the budget just rolled), **sunk cost** (we have come too far), **politics** (someone senior remembers when it printed money), and **legacy commitments** (contracts, SLAs, a few loud customers). Naming the force is what makes the next conversation possible.

*Violation signal:* The card lists reasons to retire but never says why the product is still alive.

## Guided Context Capture

Open with: "We'll work out whether this product is healthy, declining, a zombie, or just ugly, and write it on one card. I need the product and whatever evidence you have. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered:

1. `Zombie ID Q1/5`: What is the product, who uses it day to day, and roughly how long has it been in market?
2. `Zombie ID Q2/5`: What is happening to revenue, usage, and support load? Trends are enough; exact numbers are better.
3. `Zombie ID Q3/5`: Has the company strategy, the market, or the technology moved since this product was built? Is there a replacement?
4. `Zombie ID Q4/5`: Why is it still alive? Who would object to retiring it, and what commitments exist (contracts, SLAs, key customers)?
5. `Zombie ID Q5/5`: Who owns the decision to keep or stop it today? A name, not a team.

In **Context dump** mode, sort what was pasted into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the card and label every inferred item inline as *(assumed)*. Never invent a number that was not given.

**Confirm the real user.** Before drafting, confirm who uses the product day to day. Do not default to developers or engineers unless the PM confirms they are the actual users.

## Workflow

1. **Place it on the lifecycle.** Introduce, grow, mature, or decline, with one line of evidence. If unsure, run `eol-util-plc-mapper` first.
2. **Score the business reasons.** For each signal in financial viability and strategic alignment, mark `present`, `not present`, or `unknown`, with the evidence.
3. **Score the product reasons.** Same, for solution replacement and market irrelevance.
4. **Answer the seven telltale questions.** `Yes`, `no`, or `unknown`, each with a short reason. Count the yeses. If a PLC Strategy Map is supplied, its transition questions are the same seven: reuse those answers and ask only the unknowns.
5. **Run the ugly test.** "If it did not exist today, would we fund it?" Record the answer and whether any reason to retire is image-only.
6. **Name the lingering forces.** Which of inertia, sunk cost, politics, legacy commitments are at work, and how.
7. **Name the decision owner.** One person. If nobody owns it, say so; that alone is a strong zombie signal.
8. **Call the verdict** using the rubric below, and write the one-sentence finding.
9. **Hand off.** State what `eol-step2-revive-or-replace` needs from this card.

### Verdict rubric

| Verdict | When |
|---|---|
| **Healthy** | Growing or mature with affirmative evidence of current value and viability; no material retirement case established. Unknown telltales remain unknown rather than being counted as healthy answers. |
| **Declining** | In decline, with reasons emerging, and a named owner who is actively planning (extension, replacement, or exit). |
| **Zombie** | In decline, material business or product reasons to reconsider funding are supported, and no one owns the decision or the product survives mainly on lingering forces. Telltales strengthen the diagnosis; a majority of Yes answers is not required or sufficient. |
| **Just ugly** | The only reasons offered are image or emotion; customers still get real value; it would be funded today. |

When evidence is thin, say which verdict the evidence leans toward and what single fact would settle it. Do not force a verdict the evidence cannot carry.

## What It Produces

Complete the [Zombie ID Card](template.md):

- the product, its users, and its place on the lifecycle
- business and product reasons, each marked with evidence
- the seven telltale answers and the count of yeses
- the ugly test
- the lingering forces
- the decision owner (or the absence of one)
- the verdict and a one-sentence finding
- the handoff to the retain, revive, replace, or retire decision

## Human Decision Gate

The PM confirms the verdict before it moves on. The agent may recommend a verdict; the PM owns it. Record who confirmed it and anything they weighed differently.

## Common Pitfalls

**Calling decline a zombie.** *Symptom:* falling sales alone triggers the verdict. *Fix:* check for an owner and a plan; a declining product with both is not a zombie.

**Killing the spork.** *Symptom:* the strongest reason is that the product looks dated. *Fix:* run the ugly test and require at least one business or product reason.

**Skipping the forces.** *Symptom:* a strong case to retire, no explanation of why the product is still alive. *Fix:* name the force, because that is who the PM has to persuade.

**Inventing evidence.** *Symptom:* precise numbers appear that nobody supplied. *Fix:* mark unknowns as unknown and say what would settle them.

## References

- [template.md](template.md): the Zombie ID Card
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Combine with:** [eol-util-plc-mapper](../eol-util-plc-mapper/SKILL.md) to place the product on the lifecycle
- **Downstream:** [eol-step2-revive-or-replace](../eol-step2-revive-or-replace/SKILL.md) takes the card and makes the call
