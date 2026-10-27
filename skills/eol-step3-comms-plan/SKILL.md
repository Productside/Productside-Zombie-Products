---
name: eol-step3-comms-plan
description: Turn a retire or replace decision into a completed EOL Action Planning Worksheet (phases, dates, who to tell first, what each team does at each phase, and the customer path), following Productside's end-of-life timeline and rules of the road. Use once a product's exit is decided, before anything is announced.
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
  - "Building the EOL Action Planning Worksheet for a product that is being retired or replaced"
  - "Sequencing who hears about an exit, and in what order"
  - "Giving customers a calendar and a path instead of a surprise"
scenarios:
  - "The decision to retire is made and someone wants to send the announcement tomorrow"
  - "A replacement launches next quarter and the old product's exit has no plan"
  - "Sales is still bundling a product that has been declared end of sale"
produces:
  - "EOL Action Planning Worksheet: phase timeline, tell order, action grid by team and phase, key action items, rules-of-the-road check"
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

Produce a completed **EOL Action Planning Worksheet**: the dates, the tell order, what every team does at each phase, and the customer path, on one worksheet.

Nobody fails at deciding to kill a product. They fail at who they tell, when, and how. The nightmare is not the decision; it is the communication. This skill exists so the exit does not unravel in the handoffs.

Use this skill when you need to:

- plan an exit after a retire or replace decision, before anything is announced
- decide who hears first and in what order
- give customers a calendar and a migration path
- make sure sales, support, partners, and systems change on the same dates

This is not the decision. If the product has not been decided, run `eol-step2-revive-or-replace` first. This is also not a press release; it is the plan the announcement comes out of.

## Key Concepts

**End of life is a sequence of phases, not a date.**

| Phase | Definition | Milestone | Default timing |
|---|---|---|---|
| **GA** General Availability | Fully available for purchase and supported | Launch date | Ongoing until notice |
| **NSC** Notice of Status Change | Formal announcement of the product's upcoming end of life | Announcement date | **Lead time before EOS: default 6 months, range 3 to 12** (longer for contracted, enterprise, or regulated products) |
| **EOS** End of Sale | No longer available for purchase | Last day to order | Set by the lead time |
| **EOE** End of Expansion | No further expansions, add-ons, or upgrades | Last day for add-ons or upgrades | About 3 months after EOS |
| **EOL** End of Life | The product reaches the end of its lifecycle; support transition begins | Support transition begins | About 3 months after EOE |
| **EOSL** End of Service Life | All support and services cease | Final day of support | About 3 months after EOL |

Timings are planning defaults. Their configurable range is not an applicable legal or contractual minimum. When obligations are unknown, say they are unverified; do not assert that a requested date breaches a contract merely because it is shorter than a default. Confirm actual constraints before proposing a committed notice or closure date. Verified obligations may require longer intervals.

**First stop: legal or finance. Last stop: engineering.** Everyone goes to engineering first because that is where the product lives. It is exactly backward. Legal needs to know what is owed (contracts, SLAs, regulatory obligations). Finance needs to know what it does to forecasts and revenue. Then sales, partners, customer success, and enablement. Engineering is the last internal stop, after the groups who carry the commitments.

*Violation signal:* The first internal conversation in the plan is with engineering, or the announcement date comes before legal and finance have signed off.

**Every team has work at every phase.** End of life is a team sport. Default activities by team and phase:

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

**Key action items.** Whatever the product, these eight actions appear in every exit: announce the replacement product; compare old and new features; engage distributors and channels; revise sales forecasts; plan old versus new inventory (or licensing); update marketing materials; capture churn versus conversions; modify sales and service systems.

**The rules of the road.**

| Do not | Do |
|---|---|
| Surprise users. Warn them early. | Communicate early, clearly, and often. |
| Strand users. Offer a path. | Align stakeholders before announcing. |
| Ignore contracts and SLAs. | Offer a clear migration path. |
| "Brick" paid-for hardware. Ever. | Review legal and regulatory obligations. |
| Ignore public safety risks. | Create a partner transition plan. |
| Treat support as an afterthought. | Offer paid support where strategic. |
| Leave users exposed to risks. | Use data to identify impacted users. |

*Violation signal:* The plan has an announcement date but no migration path, or customers hear before partners and sales are ready to answer them.

**An unknown path is not an absent path or an available one.** A coverage gap, an unassessed replacement, and a confirmed alternative are different findings. Say “no confirmed alternative yet” when the assessment is missing. Do not turn the complement of an unavailable share into verified replacement coverage, or convert a share of the catalog into a share of customers. Every availability or migration promise needs its own supplied evidence.

**Coordinate an external transition through a named owner.** For another vendor's product, verify account eligibility, job and integration coverage, data-transfer permission, customer acceptance, and support ownership/escalation between providers. Carry signed commercial terms into the customer path: calculate the discounted price and show its duration, renewal price, exclusions and any bundle repricing. Keep unresolved accounts on a supported path; do not force their support end from generic dates while the alternative or required acceptance remains unverified. A vendor offer alone does not approve migration or an announcement.

**A plan is not completed alignment.** In the action grid and rules-of-the-road check, use Planned / Pending / Confirmed with evidence. A proposed tell order does not mean the teams have been told or approved it. A drafted billing pull does not mean affected users have been identified. Keep draft dates and promises visibly gated until their owners confirm them.

## Guided Context Capture

Open with: "We'll build the EOL Action Planning Worksheet: dates, who hears first, what every team does at each phase, and the customer path. If you have the Decision Record, I need very little else. How do you want to work? 1. Guided, 2. Context dump, 3. Best guess."

In **Guided** mode, ask one at a time and skip anything already answered:

1. `Comms Q1/5`: What was decided (retire or replace), and is there a replacement product? What is it?
2. `Comms Q2/5`: What is the target end-of-sale date, or the date by which the product must be gone?
3. `Comms Q3/5`: What commitments exist: contracts, SLAs, regulation, partners, key customers?
4. `Comms Q4/5`: Is the product physical, digital, or a service? (This decides which team rows apply.)
5. `Comms Q5/5`: Who owns the plan, and who owns each team's part?

In **Context dump** mode, sort what was given into `Known / Assumed / Missing / Conflicting` and ask only the material gaps. In **Best guess** mode, draft the worksheet with default timings and label every inferred item *(assumed)*.

## Workflow

1. **Set the dates.** Work back from end of sale: the notice date (lead time), then EOE, EOL, and EOSL using the defaults. Lengthen any interval a contract or regulation requires. Write real dates.
2. **Write the tell order.** Legal and compliance, financial planning, then the internal teams (sales, partner management, customer success, product enablement, IT and systems), engineering last, then partners, then customers at the notice date. Give each a "by" date before the announcement.
3. **Fill the action grid.** Start from the defaults; tailor each cell to this product; rename rows for digital products; assign an owner per row.
4. **Plan the customer path.** Who is affected (use data, not guesses), what they move to, what it costs them, what support continues and for how long, and what the announcement says.
5. **Place the eight key action items** on the timeline with an owner each.
6. **Run the rules-of-the-road check.** Every "do" has a line in the plan; no "do not" is violated. Flag anything that fails.
7. **List the open risks.** The two or three things most likely to make the exit unravel, with a mitigation for each.

## What It Produces

Complete the [EOL Action Planning Worksheet](template.md):

- the phase timeline with real dates
- the tell order, with "by" dates and owners
- the action grid by team and phase
- the customer path and the announcement's key messages
- the eight key action items on the timeline
- the rules-of-the-road check
- the open risks

## Human Decision Gate

The PM and the plan's owner approve the tell order and the notice date before anyone outside legal and finance hears about the exit. The agent drafts; humans announce.

## Common Pitfalls

**Engineering first.** *Symptom:* step one is "tell the engineering team." *Fix:* legal and finance first; engineering last.

**A date, not a plan.** *Symptom:* one end-of-life date and an email. *Fix:* all six phases, with real dates and owners.

**Selling after end of sale.** *Symptom:* sales keeps bundling the product into other offers after EOS. *Fix:* sales activities and IT and systems change on the EOS date; put "stop the bundles" in the sales row.

**Stranded customers.** *Symptom:* no migration path, or support ends before customers can move. *Fix:* the customer path is written before the notice date, and EOSL comes after customers can realistically migrate.

## References

- [template.md](template.md): the EOL Action Planning Worksheet (this is also the downloadable template)
- [examples/sample.md](examples/sample.md): a worked example on a fictional product
- **Downstream:** `eol-message`, from Dean Peters' Product Manager Skills (CC BY-NC-SA 4.0, [eol-message in Product Manager Skills](https://github.com/deanpeters/Product-Manager-Skills/tree/main/skills/eol-message)), writes the announcement from this worksheet's customer path and key messages; [eol-step4-free-the-living](../eol-step4-free-the-living/SKILL.md) moves the capacity the exit frees
- **Upstream:** [eol-step2-revive-or-replace](../eol-step2-revive-or-replace/SKILL.md) provides the Decision Record
- **Related:** the Productside Playbook's stakeholder alignment play maps interest and influence for the tell order
