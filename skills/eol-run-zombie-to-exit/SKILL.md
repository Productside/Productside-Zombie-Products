---
name: eol-run-zombie-to-exit
description: Run diagnosis and a retain-revive-replace-retire decision on one product, then route to its operating, extension, replacement or closure plan and only applicable downstream work, stopping at human decisions. Use when you want the appropriate operating, extension, replacement or retirement branch in one session.
license: CC-BY-NC-SA-4.0
argument-hint: "[the product and everything you know: lifecycle, revenue trend, costs, customers, contracts, owner]"
intent: >-
  Help a Product Manager take one aging product from diagnosis to a four-motion decision and
  its selected plan in a single guided run, reusing each step’s own instructions, carrying context
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
  - "Zombie-to-Exit Pack: diagnosis and Decision Record, the selected Operating, Extension, Replacement or Retirement plan, and only applicable downstream artifacts; every human decision recorded"
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

Produce a **Zombie-to-Exit Pack**: the artifacts appropriate to one product’s Retain, Revive, Replace or Retire decision, with skipped branches identified.

Each step already has its own skill. This one runs them in sequence, reads each step's instructions from its own `SKILL.md`, carries every answer forward, and stops wherever a human owns the call. It adds no new method; it removes the re-pasting.

Use this skill when you want the whole loop. Use the individual steps when you only need one artifact.

## The loop

| # | Step | Skill | Artifact | Stops for |
|---|---|---|---|---|
| 0 | Where it sits *(optional)* | `eol-util-plc-mapper` | PLC Strategy Map | The PM confirms the stage |
| 1 | Is it a zombie? | `eol-step1-zombie-id` | Zombie ID Card | The PM confirms the verdict |
| 1b | What it really costs *(optional)* | `eol-util-cost-ledger` | Cost Ledger | The PM confirms figures and labels |
| 2 | Retain, revive, replace, or retire? | `eol-step2-revive-or-replace` | Decision Record | **The Decider says one word** |
| 3 | Plan Replace or Retire | `eol-step3-comms-plan` | Replacement Launch and Exit Worksheet OR Retirement Closure Worksheet | The PM and plan owner approve the tell order and notice date |
| 3b | Write the announcement | `eol-message` (Product Manager Skills) | Announcement draft | Legal and the plan owner approve the text |
| 4 | Free the living | `eol-step4-free-the-living` | Capacity Transfer | The budget owner approves the trade |

**Early finding is not a Retain decision.** If step 1 says *healthy* or *just ugly*, preserve the existing early stop before step 1b, its evidence and any valid funding/ownership record. Mark remaining artifacts/gates Not applicable / skipped. Do not invent a Retain approval. If the user explicitly requests a new four-motion decision despite that finding, continue to step 2 without treating health or appearance as an exit recommendation. A separately requested ledger can still be run.

**Four branches after the human decision.** Use the definitions in [step 2](../eol-step2-revive-or-replace/SKILL.md): Retain operates as is; Revive extends this product; Replace introduces a successor; Retire ends it without one. If a supplied label conflicts with the proposed successor or scope, preserve the record and stop for clarification, even in Best guess. Never silently change the human's word.

| Chosen motion | Required branch artifact | Downstream routing |
|---|---|---|
| **Retain** | Operating Plan in the Decision Record: value, scope, budget/capacity ceiling, operating owner, review date, triggers and approvals | Skip steps 3, 3b and automatic step 4. Unknown limits stay Pending; do not approve indefinite operation. |
| **Revive** | Extension Plan in the Decision Record: hypothesis, customer/segment, outcome, investment, owner, test and evidence-review date | Skip steps 3 and 3b. Run step 4 only if separately evidenced capacity is actually being released elsewhere. |
| **Replace** | Replacement Launch and Exit Worksheet: successor rollout plus old-product exit, migration, acceptance and overlap | Step 3 uses `replace-template.md`; step 3b announces the replacement and supported old-product exit, with promises gated. |
| **Retire** | Retirement Closure Worksheet: lost capability, customer impact, obligations, records and final support; no successor | Step 3 uses `retire-template.md`; step 3b announces closure without fabricating a migration destination. |

Continued support during an approved Replace/Retire plan is execution of that plan, not a new Retain or Revive decision. For Replace/Retire, assess step 4 against the ledger and continuing obligations, including successor launch/overlap costs. Draft Unknown amounts where necessary; if there is no capacity transfer to propose, mark it Not applicable with the reason. No branch guarantees cash savings or authorizes staffing/budget moves.

**Where `eol-message` lives.** It is in Dean Peters' Product Manager Skills collection (CC BY-NC-SA 4.0): [eol-message in Product Manager Skills](https://github.com/deanpeters/Product-Manager-Skills/tree/main/skills/eol-message). Depending on how it was installed, it may be invoked as `eol-message` or with a collection prefix (for example `anthropic-skills:eol-message`); look for either. If it is not installed, draft a clearly labeled fallback announcement only for Replace or Retire, from the selected worksheet's customer path and key messages. Include the affected product and audience, the change and reason, dates, the branch-specific customer path (migration for Replace; closure/records/assistance for Retire), support commitment, and contact. Do not claim to have used the unavailable skill.

**The ledger is required for step 4.** The cost ledger is optional when the loop stops at a decision or an exit plan. If step 4 will run, run the ledger too: step 4 moves what the ledger counts.

## Key Concepts

**One context, never asked twice.** Collect what the user knows once, at the start. Every later step reads from it and from the artifacts already produced, and asks only what is still missing.

*Violation signal:* A later step asks for the product name, users, or dates that an earlier artifact already holds.

**The gates are the point.** The agent drafts every artifact; humans make every call. How the run stops depends on the mode:

| Mode | Hard stop (wait for the answer) | Every other gate |
|---|---|---|
| Guided, Context dump | Every gate in the loop table | |
| Best guess | **The Decider gate only** | Draft through it, mark the gate *pending* in the decision log, and list it under "Confirmations needed" at the end |

A *pending* gate is not a confirmation. The pack is a draft until every pending gate has a named person and a date. The agent never picks Retain, Revive, Replace or Retire, in any mode.

*Violation signal:* The pack contains a decision with no named person and date, or a pending gate shown as confirmed.

**No Decider, no decision.** The Decider is asked for in every mode, including Best guess. On a zombie, the honest answer is often "nobody"; that is the finding, not a gap to skip. If nobody owns the decision, recommend who should (a role with budget authority over the product, for example the leader whose budget funds it), then stop and ask for one name. The Decider gate asks for three things together: the name, the word, and the reason in the Decider's own words. Do not continue past step 2 without all three; a word with no reason is how a product drifts back into limbo.

*Violation signal:* The run reaches step 2 with no named Decider, the agent fills in a Decider the user did not name, or the Decision Record has a word but no reason.

**Promise only what the plan supports.** After step 3b, check every customer-facing promise in the announcement (dates, coverage, support, prices, what "nothing changes" means) against a line in the worksheet. A promise with no matching line is either removed, softened to what the plan supports, or turned into a gated plan item with an owner. Show the check as a table: promise, worksheet line, verdict (supported / gated / unsupported).

*Violation signal:* The announcement promises something (for example, "the new product will cover everything") that the worksheet lists as a risk or an unknown.

**Evidence and status travel with the artifact.** Reuse the input's evidence IDs, or short source names when no IDs exist, beside consequential findings, figures, constraints, and readout claims. Cite unnumbered context as “case introduction,” not an invented source ID. Missing evidence stays Unknown; do not convert it to No. Preserve existing supplied decisions as recorded, distinguish them from approvals requested during this run, and distinguish **Pending**, **Confirmed**, and **Not applicable / skipped**. A skipped gate is not an outstanding approval. A fictional fixture's records remain fictional; never imply independent verification. Label returned fictional artifacts explicitly, including resumed outputs. Keep dates attached to the program or decision they govern; a next-bet review is not a support-bridge renewal review.

**Each step follows its own skill.** Read the step's `SKILL.md` and fill its `template.md`. Apply that step's violation signals and pitfalls. Do not shorten a step to save time; skip optional steps instead, and say which.

## Guided Context Capture

Open with: "We'll take this product from 'is it a zombie?' to an explicit four-motion decision and its appropriate plan. I'll stop for you at each decision. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess. And do you want the optional lifecycle map and cost ledger? (Recommended: yes to both.)"

In **Guided** mode, ask one at a time, then start the loop:

1. `Loop Q1/6`: What is the product, who uses it day to day, and how long has it been in market?
2. `Loop Q2/6`: What are revenue, usage, and margin doing?
3. `Loop Q3/6`: What does it cost to keep alive: support, engineering, compliance, licenses?
4. `Loop Q4/6`: What supports operating as is, extending this product, introducing a successor, or closing without one? What commitments constrain these options?
5. `Loop Q5/6`: Who is the Decider? One name.
6. `Loop Q6/6`: Is it physical, digital, or a service, and is there a target end-of-sale date?

In **Context dump** mode, sort everything into `Known / Assumed / Missing / Conflicting` once, ask only the gaps that block step 1, and ask later gaps when their step needs them. In **Best guess** mode, run each applicable branch step with assumptions labeled *(assumed)*, mark the soft gates *pending*, and stop hard only at the Decider gate. Ask `Loop Q5/6` (the Decider) in every mode.

**Carry answers forward.** When step 0 has answered the seven transition questions, step 1 reuses those answers for its telltale questions (they are the same seven) and asks only the unknowns.

## Workflow

1. **Capture context** once, as above.
2. **Run each applicable step in order**, reading its `SKILL.md`, filling its template, and carrying the artifact forward.
3. **Handle each gate by mode** (see the gates table). At the Decider gate, record the name, the word, the reason in their words, and the date; ask again for any that is missing. At a hard stop, present the draft, the decision needed, and who owns it, and record the answer, the person, and the date before continuing. In Best guess, mark soft gates *pending* and keep going.
4. **Follow the branches** after step 1 and step 2.
5. **Run the promise check** after step 3b, and fix or flag every unsupported promise before the announcement goes to its approvers.
6. **Assemble the pack**: a cover page (product, verdict, decision, Decider, key dates, the trade) followed by each artifact in order.
7. **List what is still open**: every *(assumed)* item and unknown, with who can answer it, and every *pending* gate under "Confirmations needed," with who must confirm it. Keep skipped gates out of that list.
8. **Lead with a readout of at most 200 words**, at every hard stop and when the run ends. Aim for 120–150 words to leave room for source citations and labels; check the length before returning. State the product finding, strongest source-backed evidence, economics if known, decision status, customer risk or job, capacity status if relevant, and the next action and owner. Carry a material date or obligation conflict into the short readout when it blocks the customer path. Cite the supplied evidence IDs or source names inline. At a stop, call it interim; at an early branch, say which work was skipped. Keep the reached artifacts separately below it rather than replacing them with the short readout.

## What It Produces

Complete the [Zombie-to-Exit Pack](template.md), including only the selected branch:

- a one-page cover
- each artifact in loop order, or a line saying why a step was skipped
- the decision log: every gate, who decided, and when (and the Decider's reason)
- the Operating Plan, Extension Plan, Replacement Launch and Exit Worksheet, or Retirement Closure Worksheet
- the promise check when an announcement is drafted
- the open items

## Human Decision Gate

Every gate in the loop table above. The agent never confirms a stage, a verdict, figures, a decision, a notice date, announcement text, or a trade on a human's behalf.

## Common Pitfalls

**Racing the Decider.** *Symptom:* the run flows from verdict to exit plan without a named Decider saying the word. *Fix:* the Decider gate is a hard stop in every mode.

**The announcement outruns the plan.** *Symptom:* customers are promised a date, feature, or support level the worksheet doesn't guarantee. *Fix:* the promise check; every promise maps to a worksheet line or comes out.

**Stopping at everything.** *Symptom:* Best guess halts after the lifecycle map to ask the PM to confirm the stage. *Fix:* in Best guess, soft gates are marked pending and confirmed together at the end.

**Planning an exit for Retain or Revive.** *Symptom:* an EOL worksheet appears after either choice. *Fix:* complete the Operating or Extension Plan instead.

**Invented capacity release.** *Symptom:* every branch ends with a transfer or gross costs are called savings. *Fix:* assess the ledger, retained work and approvals; show Unknown or Not applicable when no transfer is evidenced.

**Thin steps.** *Symptom:* each artifact is a summary, not the template. *Fix:* fill each step's own template; skip optional steps rather than thinning required ones.

## References

- [template.md](template.md): the Zombie-to-Exit Pack
- [examples/sample.md](examples/sample.md): the cover and decision log for the fictional Classic Reports run
- Steps: [eol-util-plc-mapper](../eol-util-plc-mapper/SKILL.md), [eol-step1-zombie-id](../eol-step1-zombie-id/SKILL.md), [eol-util-cost-ledger](../eol-util-cost-ledger/SKILL.md), [eol-step2-revive-or-replace](../eol-step2-revive-or-replace/SKILL.md), [eol-step3-comms-plan](../eol-step3-comms-plan/SKILL.md), [eol-step4-free-the-living](../eol-step4-free-the-living/SKILL.md)
