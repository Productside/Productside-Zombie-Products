---
name: eol-step3-comms-plan
description: Turn Replace into a successor launch and old-product exit plan, or Retire into closure without a successor. Sequence conversations, actions, dates and customer commitments. Use after the named human decision; not for Retain or Revive.
license: CC-BY-NC-SA-4.0
argument-hint: "[the Decision Record, or the product, the decision, and the target end-of-sale date]"
intent: >-
  Help a Product Manager plan the communications and actions for a product exit, so legal and
  finance hear first, customers are never surprised or stranded, and every team knows what to
  do at each phase from notice of status change to end of service life.
type: interactive
theme: product-end-of-life
phase: 3
best-for:
  - "Building the matching Replacement Launch and Exit or Retirement Closure Worksheet"
  - "Sequencing who hears about an exit, and in what order"
  - "Giving customers a calendar and a path instead of a surprise"
scenarios:
  - "The decision to retire is made and someone wants to send the announcement tomorrow"
  - "A replacement launches next quarter and the old product's exit has no plan"
  - "Sales is still bundling a product that has been declared end of sale"
produces:
  - "Selected Replacement Launch and Exit Worksheet OR Retirement Closure Worksheet: phase timeline, tell order, team actions, customer impact and approval checks"
depends-on:
  - eol-step2-revive-or-replace
downstream:
  - eol-message
  - eol-step4-free-the-living
source-basis:
  - "Productside product lifecycle and end-of-life teaching materials, adapted for the How to Kill Zombie Products digital takeaways"
---

# EOL Comms Plan

## Purpose

Produce the worksheet for the recorded decision: **Replacement Launch and Exit** for Replace, or **Retirement Closure** for Retire. Both record who speaks to whom, in which order, what each conversation resolves, and who owns the next action.

Nobody fails at deciding to kill a product. They fail at who they tell, when, and how. The nightmare is not the decision; it is the communication. This skill exists so the exit does not unravel in the handoffs.

Use this skill when you need to:

- plan an exit after a retire or replace decision, before anything is announced
- decide who hears first and in what order
- give customers a supported migration plan for Replace or a clear closure/records/support plan for Retire
- make sure sales, support, partners, and systems change on the same dates

This is not the decision. If the product has not been decided, run `eol-step2-revive-or-replace` first. This is also not a press release; it is the plan the announcement comes out of.

## Key Concepts

**Select one branch before drafting.** Read the recorded human word, reason, date and product boundary. Replace introduces a successor product; Retire ends this product without one. Retain (operate as is) and Revive (extend the existing product) return to step 2's branch plans, without an EOL worksheet. If the record is missing, stop for the Decider. If Retire names a successor or otherwise conflicts with its scope, preserve the record and stop for clarification, including in Best guess; do not relabel it or fabricate a replacement.

- **Replace:** use [replace-template.md](replace-template.md). Coordinate successor rollout/go-to-market and old-product exit separately. Establish coverage, integration, prices, readiness, migration tests, customer acceptance, overlap, rollback and support ownership. The successor may be internal or external; adoption of an existing successor still needs rollout evidence.
- **Retire:** use [retire-template.md](retire-template.md). Explain the capability that ends and that no successor is provided. Plan notice, obligations, final support, refunds where applicable, records/export access, retention and authorized disposition. Do not promise that customers will migrate or a new product will restore their job. Records access and temporary runoff support do not make this Replace or Retain.

**End of life is a sequence of phases, not a date.**

| Phase | Definition | Milestone | Default timing |
|---|---|---|---|
| **GA** General Availability | Fully available for purchase and supported | Launch date | Ongoing until notice |
| **NSC** Notice of Status Change | Formal announcement of the product's upcoming end of life | Announcement date | **Lead time before EOS: default 6 months, range 3 to 12** (longer for contracted, enterprise, or regulated products) |
| **EOS** End of Sale | No longer available for purchase | Last day to order | Set by the lead time |
| **EOE** End of Expansion | No further expansions, add-ons, or upgrades | Last day for add-ons or upgrades | About 3 months after EOS |
| **EOL** End of Life | The product reaches the end of its lifecycle; support transition begins | Support transition begins | About 3 months after EOE |
| **EOSL** End of Service Life | All support and services cease | Final day of support | About 3 months after EOL |

Preserve actual historical milestones: if EOS already occurred, record it and plan catch-up controls for bundle/catalog promises; do not invent a new EOS or restart its notice cycle.

Timings are planning defaults. Their configurable range is not an applicable legal or contractual minimum. When obligations are unknown, say they are unverified; do not assert that a requested date breaches a contract merely because it is shorter than a default. Confirm actual constraints before proposing a committed notice or closure date. Verified obligations may require longer intervals.

**First stop: legal or finance. Last stop: engineering.** Everyone goes to engineering first because that is where the product lives. It is exactly backward. Legal needs to know what is owed (contracts, SLAs, regulatory obligations). Finance needs to know what it does to forecasts and revenue. Then sales, partners, customer success, and enablement. Engineering is the last internal stop, after the groups who carry the commitments.

*Violation signal:* The first internal conversation in the plan is with engineering, or the announcement date comes before legal and finance have signed off.

**Tailor the team grid to the branch.** End of life is a team sport. The defaults below contain replacement activities: use successor/launch/migration cells only for Replace. For Retire, substitute closure, capability-loss explanation, final support and records tasks; mark inapplicable work explicitly. Default activities by team and phase:

| Team | NSC | EOS | EOE | EOL | EOSL |
|---|---|---|---|---|---|
| Product strategy | Plan transition, prepare replacement | Offer alternatives | End feature requests | | Manage legacy issues |
| Legal and compliance | Review legal implications | Address contractual obligations | Mitigate risks | Finalize legal matters | |
| Financial planning | Adjust forecasts | Review revenue implications | Budget for transition | Plan support costs | Close financials |
| Customers and stakeholders | Notify of changes | Manage key players | Provide timelines | Update continuously | Send final notices |
| Partner management | Provide partner EOL strategy | Manage partner expectations | | Conclude partner programs | |
| Production and supply chain | Begin ramp-down | Manage suppliers | Adjust production | Finalize production | Complete phase-out |
| Inventory management | Plan inventory strategy | Last-time buy options | Additional purchase options | Clear remaining inventory | |
| Sales | Communicate changes | Focus on last-time sales | Manage final orders | Transition to new product | Evaluate sales impact |
| Customer success | Prepare for inquiries | Transition knowledge transfer | | Support new product | Provide limited support |
| Product enablement | Update EOL materials | Prepare transition guides | | Highlight similarities and changes | Archive all materials |
| IT and systems | Plan system updates | Begin system changes | Stop all enhancements | Implement final changes | Decommission old systems |

For a digital or subscription product, production, supply chain, and inventory usually become **licensing and provisioning** (stop new licenses, honor renewals, plan data export). Rename the rows rather than leaving them blank.

**Branch-specific actions.** Replace includes successor rollout, old/new feature and price comparison, customer migration and acceptance, and old-product exit. Retire includes closure notice, impact of the lost capability, final entitlements/payments/support, and records access/disposition. Both include channel/bundle review, forecasts, licensing/provisioning, materials, customer-impact measures and system changes. Do not force a replacement announcement into Retire.

**The rules of the road.** A supported retirement addresses the loss of the job honestly; it does not guarantee a substitute exists.

| Do not | Do |
|---|---|
| Surprise users. Warn them early. | Communicate early, clearly, and often. |
| Leave users without a supported closure or migration plan. | Align stakeholders before announcing. |
| Ignore contracts and SLAs. | Plan migration for Replace; supported closure for Retire. |
| "Brick" paid-for hardware. Ever. | Review legal and regulatory obligations. |
| Ignore public safety risks. | Create a partner transition plan. |
| Treat support as an afterthought. | Offer paid support where strategic. |
| Leave users exposed to risks. | Use data to identify impacted users. |

*Violation signal:* The plan has an announcement date but no branch-specific customer path, or customers hear before partners and sales are ready to answer them.

**An unknown path is not an absent path or an available one.** A coverage gap, an unassessed replacement, and a confirmed alternative are different findings. Say “no confirmed alternative yet” when the assessment is missing. Do not turn the complement of an unavailable share into verified replacement coverage, or convert a share of the catalog into a share of customers. Every availability or migration promise needs its own supplied evidence.

**Coordinate an external replacement through a named owner.** If another vendor’s product takes over the job, this is Replace. For that successor, verify account eligibility, job and integration coverage, data-transfer permission, customer acceptance, and support ownership/escalation between providers. Carry signed commercial terms into the customer path: calculate the discounted price and show its duration, renewal price, exclusions and any bundle repricing. Keep unresolved accounts on a supported path; do not force their support end from generic dates while the alternative or required acceptance remains unverified. A vendor offer alone does not approve migration or an announcement.

**Temporary transition programs need their own comparison.** For overlap, a limited-support bridge or compensation, retain duration, eligibility, covered work, exclusions and approvals. Show the incremental revenue minus delivery cost when both are supplied; separate loaded effort from cash and distinguish expected orders from paid amounts. Keep each review date attached to its own program. A security-only extension does not waive existing normal-support commitments or prove a missing integration works.

For either selected branch, append the [Customer Transition Scorecard](../../templates/Customer-Transition-Scorecard.md) to the customer path. Its five areas need evidence, next action, responsible owner, acceptance/release conditions and status. For Retire, explicitly record no successor and the capability lost; replace migration tests with closure/records/support evidence where appropriate. Never treat successful refunds as restoration of that job. Record relationship and post-transition outcomes as unobserved until evidence exists; a download, signed offer or paid refund does not establish a successful customer transition.

**A plan is not completed alignment.** In the action grid and rules-of-the-road check, use Planned / Pending / Confirmed with evidence. A proposed tell order does not mean the teams have been told or approved it. A drafted billing pull does not mean affected users have been identified. Keep draft dates and promises visibly gated until their owners confirm them.

## Guided Context Capture

Open with: "We'll build the worksheet for your Replace or Retire decision: dates, who hears first, each conversation’s purpose and owner, team actions, and the customer path. If you have the Decision Record, I need very little else. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered:

1. `Comms Q1/5`: Who chose Replace or Retire, for what product scope and reason? For Replace, what is the successor? For Retire, confirm no successor is provided.
2. `Comms Q2/5`: Which milestones already occurred? What dates are proposed and, for Replace, when is the successor actually ready?
3. `Comms Q3/5`: What commitments exist: contracts, SLAs, regulation, partners, key customers?
4. `Comms Q4/5`: Is the product physical, digital, or a service? (This decides which team rows apply.)
5. `Comms Q5/5`: Who owns the plan, and who owns each team's part?

In **Context dump** mode, sort what was given into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the worksheet with default timings and label every inferred item *(assumed)*.

## Workflow

1. **Select and load the worksheet** through [template.md](template.md). Confirm the record is a compatible Replace or Retire decision before proceeding.
2. **Set conditional dates.** Preserve historical milestones. For Replace, separately show successor rollout/readiness and the old-product phases. For Retire, show closure phases without a launch. Use verified commitments first, label default dates assumed, and leave approvals Pending.
3. **Write the tell order.** Legal/Compliance and Finance first; then Sales/catalog/bundle owners, partner management, Customer Success, enablement and IT/data, with maintainers/engineering the last internal briefing, followed by external partners and customers. Tailor participants to the product. Give each conversation a purpose, speaker/owner, needed decision, next action/owner, proposed date and status. Unknown owners/dates remain explicit; a draft is not completed alignment.
4. **Fill the selected action grid and customer path.** Replace: rollout, readiness, migration/acceptance, overlap, rollback, price and support. Retire: lost capability, notices, obligations, refunds if applicable, final support, usable records, permission, retention and authorized disposition. Neither label authorizes a generic cutoff or automatic data move/deletion.
5. **Place branch-specific actions and risks** on the timeline with owners. Review new bundle promises, quotes, entitlements and renewals; an old EOS does not erase existing commitments. Sales/catalog restrictions need responsible approval.
6. **Append the Customer Transition Scorecard and check promises.** Keep evidence, actions, owners, release conditions and status separate. Record missing approvals and unobserved customer outcomes. Do not invent a successor for Retire or claim gross costs as savings.

## What It Produces

Complete one worksheet, selected through [template.md](template.md):

- [Replacement Launch and Exit Worksheet](replace-template.md): successor rollout and readiness plus old-product exit, migration, acceptance and overlap
- [Retirement Closure Worksheet](retire-template.md): capability loss, no successor, obligations, records, final support and closure

Both include the ordered conversation plan, dates/statuses, team action grid, customer impact/cost, approval and promise checks, open risks and the Customer Transition Scorecard. Preserve separate approval of the plan, notice, customer text and any capacity transfer.

## Human Decision Gate

The PM and the plan's owner approve the tell order and the notice date before anyone outside legal and finance hears about the exit. The agent drafts; humans announce.

## Common Pitfalls

**Engineering first.** *Symptom:* step one is "tell the engineering team." *Fix:* legal and finance first; engineering last.

**A date, not a plan.** *Symptom:* one cutoff and an email. *Fix:* show applicable historical/proposed phases, obligations, owners and approval status.

**Bundling after historical EOS.** *Symptom:* new promises continue despite a past catalog date. *Fix:* reconcile commitments and propose approved Sales/catalog controls; do not reset EOS or erase entitlements.

**Replace and Retire collapse.** *Symptom:* Retire promises migration to a successor, or Replace has no rollout/readiness plan. *Fix:* clarify the decision and use the matching worksheet. Do not silently change the human’s word.

## References

- [template.md](template.md): worksheet selector; read only the selected Replace or Retire worksheet
- [replace-template.md](replace-template.md): Replacement Launch and Exit Worksheet
- [retire-template.md](retire-template.md): Retirement Closure Worksheet
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Downstream:** `eol-message`, from Dean Peters' Product Manager Skills (CC BY-NC-SA 4.0, [eol-message in Product Manager Skills](https://github.com/deanpeters/Product-Manager-Skills/tree/main/skills/eol-message)), writes the announcement from this worksheet's customer path and key messages; [eol-step4-free-the-living](../eol-step4-free-the-living/SKILL.md) moves the capacity the exit frees
- **Upstream:** [eol-step2-revive-or-replace](../eol-step2-revive-or-replace/SKILL.md) provides the Decision Record
- **Related:** the Productside Playbook's stakeholder alignment play maps interest and influence for the tell order
