# Internet Explorer to Edge: replace the browser while preserving legacy jobs

**Record:** Microsoft retirement announcement, June 15, 2022; lifecycle FAQ and IE-mode documentation. **Sources checked:** October 28, 2026.

## What the public record establishes

Microsoft announced retirement and end of support for the Internet Explorer 11 desktop application on June 15, 2022, for affected Windows versions. It described a staged redirection to Microsoft Edge, importing favorites, passwords and settings, followed by disabling the desktop application. It identified exceptions for certain Windows editions; this was not a simultaneous end to every IE component on every system. [Microsoft's retirement announcement](https://blogs.windows.com/windowsexperience/2022/06/15/internet-explorer-11-has-retired-and-is-officially-out-of-support-what-you-need-to-know/).

Edge's IE mode uses the legacy Trident/MSHTML engine for configured sites and Chromium for modern sites. Microsoft's documentation describes policy-based site lists and compatibility boundaries: for example, IE toolbars are unsupported. Installing the successor does not establish that every legacy workflow works. [Microsoft's IE-mode documentation](https://learn.microsoft.com/en-us/deployedge/edge-ie-mode).

At the source-check date, Microsoft's lifecycle FAQ commits to IE-mode support through at least 2029 on supported operating systems, with at least one year's notice before its end of support. Operating-system support remains a separate dependency and may require an available Extended Security Updates license. “At least 2029” is not a fixed shutdown date or unconditional support for any Windows installation. [Microsoft's lifecycle FAQ](https://learn.microsoft.com/en-us/lifecycle/faq/internet-explorer-microsoft-edge).

## What this teaches — our interpretation

This is a **Replace teaching pattern**: Edge is the successor browser, and IE mode supplies a compatibility path within it. The retirement of the old desktop application is part of that replacement plan; it does not make the overall motion Retire without a successor. Keeping a compatibility engine is not a decision to Retain the old desktop application as is.

Run successor rollout and old-product exit as related work with separate acceptance conditions. Inventory the customer jobs and dependencies, identify legacy sites, test complete workflows with their owners, configure the compatibility path and resolve blockers before disabling the old entry point. A successful installation or imported bookmark is not customer-job acceptance.

Sequence IT and security, application owners and support teams before broad user notice and rollout. Give every exception an owner, support boundary and review date. Budget for compatibility support and modernization work; do not count the full legacy cost base as immediate savings.

## What the evidence cannot establish

These provider documents do not establish that every organization completed migration, every legacy site worked, customers accepted the change or any specified capacity was released. A support commitment is not measured migration success. The 2022 announcement describes the transition plan; current eligibility, component lifecycles and remediation offers require checking against the relevant platform and terms.

## Practice the decision

Use the [Replacement Launch and Exit Worksheet](../skills/eol-step3-comms-plan/replace-template.md) and [Customer Transition Scorecard](../templates/Customer-Transition-Scorecard.md) to separate successor readiness from old-product exit. Ask who accepts each critical workflow and what happens to a blocked account.

[The Missing Export](../evals/cases/04-the-missing-export.md) is a related existing fictional exercise about an incomplete successor, not an Internet Explorer simulation. Its users, gaps, obligations and economics are invented. This card adds historical context, not a new evaluation or passing result; keep it outside the closed-fixture run.
