---
name: eol-run-zombie-to-exit
description: Run the whole zombie-to-exit loop on one product (lifecycle map, Zombie ID, cost ledger, revive-replace-retire decision, exit plan, announcement, and capacity transfer), handing each step's output to the next and stopping at every human decision. Use when you want the full end-of-life pack for a product in one session instead of running each step by hand.
license: CC-BY-NC-SA-4.0
argument-hint: "[the product and everything you know: lifecycle, revenue trend, costs, customers, contracts, owner]"
intent: >-
  Help a Product Manager take one aging product from "is it a zombie?" to "where does the freed
  capacity go?" in a single guided run, reusing each EOL step's own instructions, carrying context
  forward so nothing is asked twice, and pausing for the humans who own each decision.
type: workflow
theme: product-end-of-life
phase: workflow
best-for:
  - "Producing the full end-of-life pack for one product in one sitting"
  - "Running the loop live in a workshop or webinar without re-pasting outputs between steps"
  - "Seeing where a product's case breaks: stage, verdict, ledger, decision, or plan"
scenarios:
  - "A product has been limping for years and leadership wants a recommendation and a plan by Friday"
  - "A workshop team wants to practice the whole loop on one real product"
produces:
  - "Zombie-to-Exit Pack: PLC Strategy Map, Zombie ID Card, Cost Ledger, Decision Record, EOL Action Planning Worksheet, announcement draft, and Capacity Transfer, with every human decision recorded"
uses:
  - eol-util-plc-mapper
  - eol-step1-zombie-id
  - eol-util-cost-ledger
  - eol-step2-revive-or-replace
  - eol-step3-comms-plan
  - eol-message
  - eol-step4-free-the-living
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# Run the Zombie-to-Exit Loop

## Purpose

Produce a **Zombie-to-Exit Pack**: every artifact in the end-of-life loop for one product, in order, from one guided run.

Each step already has its own skill. This one runs them in sequence, reads each step's instructions from its own `SKILL.md`, carries every answer forward, and stops wherever a human owns the call. It adds no new method; it removes the re-pasting.

Use this skill when you want the whole loop. Use the individual steps when you only need one artifact.

## The loop

| # | Step | Skill | Artifact | Stops for |
|---|---|---|---|---|
| 0 | Where it sits *(optional)* | `eol-util-plc-mapper` | PLC Strategy Map | The PM confirms the stage |
| 1 | Is it a zombie? | `eol-step1-zombie-id` | Zombie ID Card | The PM confirms the verdict |
| 1b | What it really costs *(optional)* | `eol-util-cost-ledger` | Cost Ledger | The PM confirms figures and labels |
| 2 | Revive, replace, or retire? | `eol-step2-revive-or-replace` | Decision Record | **The Decider says one word** |
| 3 | Plan the exit | `eol-step3-comms-plan` | EOL Action Planning Worksheet | The PM and plan owner approve the tell order and notice date |
| 3b | Write the announcement | `eol-message` (Product Manager Skills) | Announcement draft | Legal and the plan owner approve the text |
| 4 | Free the living | `eol-step4-free-the-living` | Capacity Transfer | The budget owner approves the trade |

**Branches.** If step 1 says *healthy* or *just ugly*, stop immediately before step 1b and record why. Mark the remaining loop artifacts and gates **Not applicable / skipped**, including an optional ledger requested as part of the loop. A user can request a standalone ledger separately; explain that distinction rather than running an exit sequence to fill every slot. Preserve existing evidence-backed funding and ownership records; do not require a fresh revive/replace/retire word for a healthy product. If step 2's Decider says **revive**, skip steps 3 and 3b, record the extension play, its owner, and the evidence check date, then run step 4 only if the revive itself frees capacity elsewhere.

**Where `eol-message` lives.** It is in Dean Peters' Product Manager Skills collection (CC BY-NC-SA 4.0): [eol-message in Product Manager Skills](https://github.com/deanpeters/Product-Manager-Skills/tree/main/skills/eol-message). Depending on how it was installed, it may be invoked as `eol-message` or with a collection prefix (for example `anthropic-skills:eol-message`); look for either. If it is not installed, draft a clearly labeled fallback announcement from the worksheet's customer path and key messages. Include the affected product and audience, the change and reason, dates, migration path, support commitment, and contact. Do not claim to have used the unavailable skill.

**The ledger is required for step 4.** The cost ledger is optional when the loop stops at a decision or an exit plan. If step 4 will run, run the ledger too: step 4 moves what the ledger counts.

## Key Concepts

**One context, never asked twice.** Collect what the user knows once, at the start. Every later step reads from it and from the artifacts already produced, and asks only what is still missing.

*Violation signal:* A later step asks for the product name, users, or dates that an earlier artifact already holds.

**The gates are the point.** The agent drafts every artifact; humans make every call. How the run stops depends on the mode:

| Mode | Hard stop (wait for the answer) | Every other gate |
|---|---|---|
| Guided, Context dump | Every gate in the loop table | |
| Best guess | **The Decider gate only** | Draft through it, mark the gate *pending* in the decision log, and list it under "Confirmations needed" at the end |

A *pending* gate is not a confirmation. The pack is a draft until every pending gate has a named person and a date. The agent never picks revive, replace, or retire, in any mode.

*Violation signal:* The pack contains a decision with no named person and date, or a pending gate shown as confirmed.

**No Decider, no decision.** The Decider is asked for in every mode, including Best guess. On a zombie, the honest answer is often "nobody"; that is the finding, not a gap to skip. If nobody owns the decision, recommend who should (a role with budget authority over the product, for example the leader whose budget funds it), then stop and ask for one name. The Decider gate asks for three things together: the name, the word, and the reason in the Decider's own words. Do not continue past step 2 without all three; a word with no reason is how a product drifts back into limbo.

*Violation signal:* The run reaches step 2 with no named Decider, the agent fills in a Decider the user did not name, or the Decision Record has a word but no reason.

**Promise only what the plan supports.** After step 3b, check every customer-facing promise in the announcement (dates, coverage, support, prices, what "nothing changes" means) against a line in the worksheet. A promise with no matching line is either removed, softened to what the plan supports, or turned into a gated plan item with an owner. Show the check as a table: promise, worksheet line, verdict (supported / gated / unsupported).

*Violation signal:* The announcement promises something (for example, "the new product will cover everything") that the worksheet lists as a risk or an unknown.

**Evidence and status travel with the artifact.** Reuse the input's evidence IDs, or short source names when no IDs exist, beside consequential findings, figures, constraints, and readout claims. Cite unnumbered context as “case introduction,” not an invented source ID. Missing evidence stays Unknown; do not convert it to No. Preserve existing supplied decisions as recorded, distinguish them from approvals requested during this run, and distinguish **Pending**, **Confirmed**, and **Not applicable / skipped**. A skipped gate is not an outstanding approval. A fictional fixture's records remain fictional; never imply independent verification. Label returned fictional artifacts explicitly, including resumed outputs. Keep dates attached to the program or decision they govern; a next-bet review is not a support-bridge renewal review.

**Each step follows its own skill.** Read the step's `SKILL.md` and fill its `template.md`. Apply that step's violation signals and pitfalls. Do not shorten a step to save time; skip optional steps instead, and say which.

## Guided Context Capture

Open with: "We'll take this product from 'is it a zombie?' to 'where does the freed capacity go?' I'll stop for you at each decision. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess. And do you want the optional lifecycle map and cost ledger? (Recommended: yes to both.)"

In **Guided** mode, ask one at a time, then start the loop:

1. `Loop Q1/6`: What is the product, who uses it day to day, and how long has it been in market?
2. `Loop Q2/6`: What are revenue, usage, and margin doing?
3. `Loop Q3/6`: What does it cost to keep alive: support, engineering, compliance, licenses?
4. `Loop Q4/6`: What replaces it, if anything, and what commitments constrain an exit (contracts, SLAs, regulation)?
5. `Loop Q5/6`: Who is the Decider? One name.
6. `Loop Q6/6`: Is it physical, digital, or a service, and is there a target end-of-sale date?

In **Context dump** mode, sort everything into `Known / Assumed / Missing / Conflicting` once, ask only the gaps that block step 1, and ask later gaps when their step needs them. In **Best guess** mode, run every step with assumptions labeled *(assumed)*, mark the soft gates *pending*, and stop hard only at the Decider gate. Ask `Loop Q5/6` (the Decider) in every mode.

**Carry answers forward.** When step 0 has answered the seven transition questions, step 1 reuses those answers for its telltale questions (they are the same seven) and asks only the unknowns.

## Workflow

1. **Capture context** once, as above.
2. **Run each step in order**, reading its `SKILL.md`, filling its template, and carrying the artifact forward.
3. **Handle each gate by mode** (see the gates table). At the Decider gate, record the name, the word, the reason in their words, and the date; ask again for any that is missing. At a hard stop, present the draft, the decision needed, and who owns it, and record the answer, the person, and the date before continuing. In Best guess, mark soft gates *pending* and keep going.
4. **Follow the branches** after step 1 and step 2.
5. **Run the promise check** after step 3b, and fix or flag every unsupported promise before the announcement goes to its approvers.
6. **Assemble the pack**: a cover page (product, verdict, decision, Decider, key dates, the trade) followed by each artifact in order.
7. **List what is still open**: every *(assumed)* item and unknown, with who can answer it, and every *pending* gate under "Confirmations needed," with who must confirm it. Keep skipped gates out of that list.
8. **Lead with a readout of at most 200 words**, at every hard stop and when the run ends. Aim for 120–150 words to leave room for source citations and labels; check the length before returning. State the product finding, strongest source-backed evidence, economics if known, decision status, customer risk or job, capacity status if relevant, and the next action and owner. Carry a material date or obligation conflict into the short readout when it blocks the customer path. Cite the supplied evidence IDs or source names inline. At a stop, call it interim; at an early branch, say which work was skipped. Keep the reached artifacts separately below it rather than replacing them with the short readout.

## What It Produces

Complete the [Zombie-to-Exit Pack](template.md):

- a one-page cover
- each artifact in loop order, or a line saying why a step was skipped
- the decision log: every gate, who decided, and when (and the Decider's reason)
- the promise check for the announcement
- the open items

## Human Decision Gate

Every gate in the loop table above. The agent never confirms a stage, a verdict, figures, a decision, a notice date, announcement text, or a trade on a human's behalf.

## Common Pitfalls

**Racing the Decider.** *Symptom:* the run flows from verdict to exit plan without a named Decider saying the word. *Fix:* the Decider gate is a hard stop in every mode.

**The announcement outruns the plan.** *Symptom:* customers are promised a date, feature, or support level the worksheet doesn't guarantee. *Fix:* the promise check; every promise maps to a worksheet line or comes out.

**Stopping at everything.** *Symptom:* Best guess halts after the lifecycle map to ask the PM to confirm the stage. *Fix:* in Best guess, soft gates are marked pending and confirmed together at the end.

**Planning an exit for a revive.** *Symptom:* the worksheet is filled after the Decider said revive. *Fix:* follow the branch; record the extension play instead.

**The loop ends at the announcement.** *Symptom:* no Capacity Transfer. *Fix:* step 4 is part of the loop; the exit is not done until the capacity moves.

**Thin steps.** *Symptom:* each artifact is a summary, not the template. *Fix:* fill each step's own template; skip optional steps rather than thinning required ones.

## References

- [template.md](template.md): the Zombie-to-Exit Pack
- [examples/sample.md](examples/sample.md): the cover and decision log for the fictional Classic Reports run
- Steps: [eol-util-plc-mapper](../eol-util-plc-mapper/SKILL.md), [eol-step1-zombie-id](../eol-step1-zombie-id/SKILL.md), [eol-util-cost-ledger](../eol-util-cost-ledger/SKILL.md), [eol-step2-revive-or-replace](../eol-step2-revive-or-replace/SKILL.md), [eol-step3-comms-plan](../eol-step3-comms-plan/SKILL.md), [eol-step4-free-the-living](../eol-step4-free-the-living/SKILL.md)
