![The Zombie Survival Kit: a glowing supply crate in a vintage B-movie graveyard, with bewildered product managers and reaching zombie hands. Free on GitHub.](media/zombie-survival-kit.png)

# Zombie Product Survival Kit

> Lose the legacy product, without losing the legacy customer.

**7 skills: the whole zombie-to-exit loop, six individual skills, and an action-planning worksheet.**

For Product Managers, product leaders, and product teams dealing with products that stopped earning their keep but somehow keep getting funded. Find the full cost, prepare a **Revive, Replace, or Retire** decision, protect customers through the transition, and give the freed capacity somewhere useful to go.

**Ugly is not dead. Declining is not a verdict.** Start with evidence before ordering the headstone.

## Start here

In Claude Code, open this Project as your working folder and try:

```text
/eol-run-zombie-to-exit
Classic Reports is a fictional reporting portal for fleet operations managers.
Revenue has fallen for three years and support load is rising.
Use guided questions. Label missing evidence and assumptions.
Stop for my revive, replace, or retire decision.
```

Replace the fictional product with your own situation when you are ready. Do not treat the sample's figures or dates as customer evidence.

**Other assistants:** provide [the loop instructions](skills/eol-run-zombie-to-exit/SKILL.md), its [output template](skills/eol-run-zombie-to-exit/template.md), and the companion skill files it calls for. If commands are not discovered, ask the assistant to read those files directly, or copy their contents into the conversation.

[How to use the skills](skills/README.md#how-to-use-a-skill) · [Fictional worked example](skills/eol-run-zombie-to-exit/examples/sample.md) · [Excel worksheet](https://github.com/Productside/Productside-Zombie-Survival-Kit/raw/refs/heads/main/templates/EOL-Action-Planning-Worksheet.xlsx) · [Markdown worksheet](templates/EOL-Action-Planning-Worksheet.md)

No assistant? Use the worksheet by hand. Excel includes a blank worksheet and a fictional worked example.

## The skills

Use one skill for the decision in front of you, or the loop to carry the same context through the sequence.

| Step | Skill | Use it to | Leaves you with |
|---|---|---|---|
| Whole loop | [eol-run-zombie-to-exit](skills/eol-run-zombie-to-exit/SKILL.md) | Work through one aging product without re-pasting every answer | Zombie-to-Exit Pack and decision log |
| Lifecycle | [eol-util-plc-mapper](skills/eol-util-plc-mapper/SKILL.md) | Check whether the product's approach fits its lifecycle stage | PLC Strategy Map |
| Recognize | [eol-step1-zombie-id](skills/eol-step1-zombie-id/SKILL.md) | Separate a zombie from a healthy, declining, or merely dated product | Zombie ID Card |
| Count the cost | [eol-util-cost-ledger](skills/eol-util-cost-ledger/SKILL.md) | Count what it earns, what it eats, and what it prevents | Cost Ledger |
| Decide | [eol-step2-revive-or-replace](skills/eol-step2-revive-or-replace/SKILL.md) | Prepare an evidence-backed recommendation for one named Decider | Decision Record |
| Plan the exit | [eol-step3-comms-plan](skills/eol-step3-comms-plan/SKILL.md) | Align the calendar, teams, communication order, and customer path | EOL Action Planning Worksheet |
| Free the living | [eol-step4-free-the-living](skills/eol-step4-free-the-living/SKILL.md) | Redirect the freed people, money, and roadmap room | Capacity Transfer |

The announcement companion, [eol-message](https://github.com/deanpeters/Product-Manager-Skills/tree/main/skills/eol-message), is part of Dean Peters' separate Product Manager Skills collection. It is linked, not bundled. The loop provides a labeled fallback when it is unavailable.

Each skill includes instructions, a blank template, and a worked example following the same fictional product, **Classic Reports**. See the [skill guide](skills/README.md) for handoffs and usage details.

## The zombie-to-exit loop

**Recognize → Count the cost → Decide → Protect the customer → Free the living**

The lifecycle map is optional when the stage is clear. The Cost Ledger is required before a capacity transfer. A healthy or merely dated product does not automatically need an exit. A revive decision follows an extension path; it does not trigger a retirement announcement.

**The assistant does the drafting. Humans make the calls.** A named Decider owns revive, replace, or retire. The responsible people confirm figures, communication dates, customer promises, and capacity commitments.

## Five rules for surviving your portfolio

| Rule | The nightmare it helps you avoid |
|---|---|
| **Recognize the Walking Dead** | Funding it by default because nobody counted the full cost |
| **Decide: Revive, Replace, or Retire** | Letting nostalgia or the loudest voice make the call |
| **Kill the Product, Not the Customer Relationship** | Leaving loyal customers stranded at the exit |
| **Make Retirement a Team Sport** | Discovering contracts, bundles, and promises after the announcement |
| **Free the Living from the Dead** | Retiring the product while the next good bet still starves |

Legal and finance hear early. Teams carrying customer commitments align before the notice. Every customer needs a path, and every capacity transfer needs an owner.

## Pick a working mode

| Mode | Best for | Ask for |
|---|---|---|
| **Guided** | You know something is wrong but need help working through it | Questions one at a time |
| **Context dump** | You have notes, metrics, obligations, and a pile of opinions | Sort what is known, assumed, missing, and conflicting |
| **Best guess** | You need a first draft and can see the gaps | Label assumptions and keep confirmations pending |

Best guess does not authorize the assistant to choose the decision or invent financial figures.

## Saw it in the webinar?

This is the companion kit for Productside's **Post Launch Success Series (Part 1): How to Kill Zombie Products**, October 28, 2026, with Dean Peters and Kenny Kranseler.

Take the [whole loop](skills/eol-run-zombie-to-exit/SKILL.md) back to your team, try the [Classic Reports example](skills/eol-run-zombie-to-exit/examples/sample.md), or start with the [worksheet](templates/EOL-Action-Planning-Worksheet.md).

## Use with judgment

All examples are fictional; figures, dates, and decisions are illustrative. Outputs are drafts. Verify evidence and calculations, and have the responsible people review commitments before acting. Planning intervals are defaults, not promises for your customers.

Start with public or fictional information. Use an organization-approved environment for confidential context, and keep completed plans outside this public Project.

For local Claude Code use, clone or download this Project and open that folder. The included `.claude/skills` link points to the skill folders. If your download or system does not preserve it, use the direct-file or copy-and-paste route above. File checks do not establish assistant-specific behavior or real-world outcomes.

## About Productside

Digital takeaways and examples that demonstrate and extend Productside's classes, workshops, webinars, consulting, and advisory services.

[Explore Productside](https://productside.com/) · [Training](https://productside.com/product-management-courses/) · [Tools and templates](https://productside.com/tools-and-templates/)

## License

Copyright © 2026 **280 Group LLC dba Productside**. Materials use [CC BY-NC-SA 4.0](LICENSE): preserve attribution and follow its noncommercial and share-alike terms. The separately linked `eol-message` skill carries its own attribution and license.

Provided **as is**, as instructional material, without warranties or a commitment to ongoing support. The content license grants no rights to Productside's names or logos; see [Trademarks](TRADEMARKS.md).

[Privacy Policy](https://productside.com/privacy-policy/) · [Terms & Conditions](https://productside.com/terms-conditions/)
