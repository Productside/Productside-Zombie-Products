# The zombie-to-exit skills

Seven skills help you examine one aging product, decide what should happen, plan the transition, and redirect the freed capacity. Six cover individual steps; the seventh runs them together. These are digital takeaways and examples supporting Productside's teaching and advisory services.

## Choose a starting point

| Skill | Use it to | Produces |
|---|---|---|
| [Run the zombie-to-exit loop](eol-run-zombie-to-exit/SKILL.md) | Work through the whole sequence with one shared context | Zombie-to-Exit Pack, including human decisions and open items |
| [PLC Mapper](eol-util-plc-mapper/SKILL.md) | Place a product on its lifecycle and compare its current approach with its stage | PLC Strategy Map |
| [Zombie ID](eol-step1-zombie-id/SKILL.md) | Separate a zombie from a healthy, declining, or merely dated product | Zombie ID Card |
| [Cost Ledger](eol-util-cost-ledger/SKILL.md) | Count what it earns, what it eats, and what it prevents | Cost Ledger |
| [Retain, Revive, Replace, or Retire](eol-step2-revive-or-replace/SKILL.md) | Prepare an evidence-backed recommendation for one named Decider | Decision Record |
| [EOL Comms Plan](eol-step3-comms-plan/SKILL.md) | Sequence conversations, dates and actions for Replace or Retire | Replacement Launch and Exit OR Retirement Closure Worksheet |
| [Free the Living](eol-step4-free-the-living/SKILL.md) | Give the freed people, money, and roadmap room a new purpose | Capacity Transfer |

The optional announcement companion, [eol-message](https://github.com/deanpeters/Product-Manager-Skills/tree/main/skills/eol-message), belongs to Dean Peters' separate Product Manager Skills collection (CC BY-NC-SA 4.0). It is linked, not included. For Replace or Retire, if unavailable, the loop drafts an announcement from the selected worksheet and explicitly labels that fallback.

## The sequence

Lifecycle map → Zombie ID → Cost Ledger → Retain/Revive/Replace/Retire → Selected branch plan.

| Motion | Meaning | Branch |
|---|---|---|
| **Retain** | Operate as is | Operating Plan: value, scope, budget/capacity ceiling, owner, review and triggers |
| **Revive** | Extend the current product | Extension Plan: hypothesis, investment, outcome/test, owner and evidence review |
| **Replace** | Introduce a successor product; phase out the old one | [Replacement Launch and Exit Worksheet](eol-step3-comms-plan/replace-template.md), then a gated replacement announcement |
| **Retire** | Close without a successor | [Retirement Closure Worksheet](eol-step3-comms-plan/retire-template.md), then a gated closure announcement |

Step 2 compares and stack-ranks all four, then stops for the human Decider. Keep `eol-step2-revive-or-replace` as the command; its scope now includes all four motions. A conflicting label/successor requires clarification, not automatic reclassification.

The lifecycle map is optional. A healthy or merely dated finding still stops the exit sequence unless a new four-motion decision is explicitly requested. Preserve valid funding records without inventing a Retain choice. The Cost Ledger is required before a Capacity Transfer; continuing work and approvals constrain any release. Retain/Revive skip the EOL worksheet and announcement. Replace and Retire use distinct worksheets and only assess capacity that may actually become available.

At each hard stop and at the end, the loop leads with a readout of at most 200 words, with source references, decision status, risks, and the next action. The reached artifacts follow separately.

## How to use a skill

Open its `SKILL.md` and supply the instructions to your AI assistant, together with the linked template and companion skills it needs. Each skill folder includes:

- `SKILL.md`: instructions and human decision gates.
- `template.md`: the output structure, also usable by hand.
- `examples/sample.md`: a worked example following **Classic Reports**, a fictional product with illustrative figures and dates.

Choose **Guided** for questions one at a time, **Context dump** to work from existing notes, or **Best guess** to draft with assumptions labeled. Best guess never authorizes the assistant to make the retain, revive, replace, or retire decision.

For local Claude Code use and a starter prompt, see the [Project README](../README.md#use-the-skills).

## Manual demo

Use the [three-prompt Classic Reports demo](../demos/classic-reports.md) in one conversation. It is the separate 1994 fintech variant; the skill examples remain the 2014 fleet-reporting product. The prepared third prompt records Replace only if the human chooses it; Retain/Revive follow their own plans and Retire has no successor. New behavioral evaluation remains pending.

## Use the worksheet directly

For the four-motion flow, use the Replace or Retire worksheet linked above. The Markdown/Excel takeaway now includes the four-motion Decision Record, Retain Operating Plan and Revive Extension Plan. Excel also has separate Replace/Retire tabs and the fictional Classic Reports Replace example. Existing behavioral reports record the earlier inputs/instructions and do not validate these new branches.

The [Markdown worksheet](../templates/EOL-Action-Planning-Worksheet.md) and [Excel worksheet](../templates/EOL-Action-Planning-Worksheet.xlsx) can be used without an assistant. Excel includes the decision worksheet, separate branch worksheets and a fictional Replace example; that example is a starting point, not a completed plan for your product.

A successor from another vendor is a Replace path. Coordinate rollout, integration, data/support handoff, eligibility, pricing/renewal and any new bill for bundled users. Retire provides no successor; explain capability loss, obligations, records and final support.

Timing intervals are planning defaults. Confirm actual obligations with the responsible legal, finance, and plan owners before making customer promises.

## Attribution and limits

Adapted from Productside's product lifecycle and end-of-life teaching materials for this webinar takeaway. Copyright © 2026 280 Group LLC dba Productside. [CC BY-NC-SA 4.0](../LICENSE).

Outputs remain drafts until the named humans confirm the evidence and decisions. Use public or fictional context until you are working in an organization-approved environment. Keep completed plans and customer information outside this public Project.

## Customer-transition evidence

For a retire/replace plan, the comms skill uses the [Customer Transition Scorecard](../templates/Customer-Transition-Scorecard.md). It keeps five areas visible: customer job and destination; cost/compensation; data, integrations and support; blocked customers; and net capacity for the next bet. Every area carries actions, owners, acceptance conditions and evidence status. Post-transition results remain unobserved until measured.

The [real-world case cards](../case-studies/README.md) explain public transition patterns. Use their paired fictional cases to practice, keeping the factual cards and evaluator answers out of a closed-fixture run.
