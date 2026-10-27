# Retire our line; help customers move to another vendor

October 27, 2026. [The Neighboring Vendor](../cases/07-the-neighboring-vendor.md) tests a distinct exit path: a product no longer fits the mission, earns little directly, and is often included in bundles. A similar product from another vendor may give customers an integration path and a negotiated discount while the company retires its own line.

This is a fictional adaptation of a practitioner-described situation. Every name, amount, agreement, integration result, date and approval is invented. No real client or vendor is identified or evaluated.

## What was run

The evaluator froze the case and [twelve criteria plus the scripted continuation](../criteria/vendor-expected-results.md) before the first response. The assistant received only the seven skill instructions, their templates and this case, inline in a fresh empty working folder. Examples, answer keys, other cases and earlier responses were withheld; tools were disabled. After observing the stop for Nora's decision, the evaluator supplied the prewritten simulated Retire reply and the new signed vendor offer. Every other approval remained pending.

The baseline used the `d313795` skill version. The targeted repeat used the same case and criteria after two small instruction changes. Returned model identifiers and results are recorded below. These are author-assistant grades, not independent human review, negotiation, integration testing, or customer validation. The scripted approval is not a real person's decision.

## Baseline findings

The first pair of responses met **10 of 12 numbered criteria**. Both missed the required $750 discounted first-year base price, even though they preserved the percentage and duration. The baseline otherwise recognized the external destination, protected the uncertain bundle contribution, rejected universal sales promises, and kept the human approvals open.

A supplemental source-fidelity issue appeared: the assistant said the cost period was unstated, although S1 explicitly ties costs to the last revenue period. It still calculated the −$180,000 attributable comparison and kept bundle effects unknown, satisfying criterion 2, but introduced an unnecessary uncertainty. This issue is recorded separately rather than changing the prewritten criterion after seeing the response.

The later trade sentence also spoke broadly of redirecting the $240,000 cost base even though releases and receiving ownership were unknown. Its surrounding tables correctly separated continuing salaries, potentially avoidable supplier payments, and pending approvals. The trade is a draft requiring review, not a verified $240,000 cash release.

| # | Baseline grade | Observed evidence |
|---|---|---|
| 1 | Pass | Strategy excludes archive-only work; “Declining” while Nora's review remains active; bundle effect stays unknown |
| 2 | Pass | “−$180,000”; contribution to the $4M bundles “unknown, not zero”; cash effect Unknown; see supplemental period error above |
| 3 | Pass | “third-party product”; “retire-plus-partner-adoption”; no internal successor required |
| 4 | **Fail** | Offer is unsigned and limited to twelve months/base subscription; new bill flagged, but $750 is never calculated |
| 5 | Pass | “4 of 6 pilots passed”; eight connector accounts blocked; remaining readiness unassessed |
| 6 | Pass | Stops for Nora's word/reason; exit artifacts not reached; source-linked 162-word readout |
| 7 | Pass | Continuation title explicitly “fictional”; Nora's decision and Tessa's assignment recorded; S6 offer now signed while other gates remain pending |
| 8 | **Fail** | Signed offer retains eligibility, September 30 deadline, duration, subsequent $1,000 base and exclusions, but still omits $750 |
| 9 | Pass | Eligibility, customer acceptance, support/data handoff and escalation remain open; connector fallback required; no automatic transfer |
| 10 | Pass | Draft July 1 EOS derived from January 1 plus six months; dates pending, existing commitments retained and blocked accounts flagged |
| 11 | Pass | Legal/Finance first; Tessa coordinates; partner handoff pending; fallback announcement “not for sending” |
| 12 | Pass | Salaries continue, supplier cancellation unknown, no staffing release or receiving owner; bounded discount/migration risk and Tessa in the short readout |

A passing numbered criterion does not erase a supplemental problem. In particular, blocked-account support beyond generic draft dates and any proposed capacity trade still require review.

## Narrow instruction changes

The decision skill now explicitly allows another vendor's product as a customer destination while retiring the company's own line. It asks for actual discounted price, duration, renewal price, exclusions and eligibility, and distinguishes draft terms, signed terms and account acceptance. It flags that bundled users can face a new bill.

The comms skill carries those terms into the customer path and asks a named owner to coordinate integration coverage, authorized data transfer, customer acceptance and support/escalation. Unresolved accounts need a supported path rather than a forced support end from generic dates. No new skill, internal successor requirement, or vendor outreach was introduced.

## Targeted repeat: 12 numbered criteria observed, with a remaining supplemental issue

All four responses identified their model as `claude-sonnet-5-5`. With the revised instructions, the repeat met **12 of 12 numbered criteria** across its initial and continuation phases. This is an assistant-graded development observation, not a clean independent acceptance or proof that the instruction changes alone caused the difference.

| # | Repeat grade | Observed evidence |
|---|---|---|
| 1 | Pass | Declining, outside approved strategy, with an active named Decider; no automatic ownerless-zombie finding |
| 2 | Pass | −$180k attributable comparison; $4M bundle contribution unmeasured; cash effect Unknown |
| 3 | Pass | “Retire with a Neighbor Archive bridge”; no internal launch required for that path |
| 4 | Pass | “25% × $1,000 = $250 off, so $750 in year one”; draft, duration, renewal, exclusions, deadline and bundled new bill retained |
| 5 | Pass | Four passed/two failed pilots, eight blocked accounts, others unassessed; no connector delivery promise |
| 6 | Pass | Stops for Nora; source-linked 179-word readout; exit work not reached |
| 7 | Pass | “continued; fictional exercise”; Nora's Retire reason/date and Tessa's assignment recorded; S6 resolves signature only |
| 8 | Pass | Customer path and fallback announcement retain $750 for twelve months, quoted $1,000 afterward, eligibility, September 30 deadline and exclusions |
| 9 | Pass | Data/security/export/support handoff gated; vendor escalation planned; unresolved accounts stay supported pending alternative/acceptance |
| 10 | Pass | July 1 draft EOS conditional on six-month term; “Unresolved accounts are not given a support end from these generic dates” |
| 11 | Pass | Tessa takes the draft to Legal/Finance first; vendor coordination assigned; announcement “not to be sent” |
| 12 | Pass | Retained salaries not cash savings; outside-payment cancellation unknown; no release/receiving owner; short readout names price, connector risk and Tessa |

The repeat still marked the explicitly stated last-period cost alignment as “assumed” and asked Finance to confirm it. That source-fidelity problem remains unresolved. Its trade sentence also still proposes moving the full cost base to an unnamed bet, with the surrounding capacity table and approval gates qualifying the proposal. These artifacts need review before operational use; twelve numbered passes are not a claim that every sentence is correct.

Readout lengths, excluding headings and standalone Markdown punctuation: baseline **162 / 158 words**, repeat **179 / 160 words** (initial / continuation). Evidence references count.


## Verification and limits

The case's arithmetic is internally consistent: $60,000 − $240,000 = −$180,000 on attributable revenue/listed costs; 25% off $1,000 is $750 for twelve months, with $1,000 the subsequent quoted base. Bundle contribution and total customer costs remain unmeasured. July 1 is the date six calendar months after January 1, conditional on the fictional Legal summary.

Canonical YAML parses and the public-file checks pass. The generic Codex validator still rejects the skills' pre-existing custom frontmatter; those fields were preserved. This work does not establish native Codex installation or portability. Other scenarios were not rerun after these conditional external-transition instructions were added.

The two phases use scripted evidence updates; they do not test an actual commercial negotiation or real integration. Repeating the same authored case is a development check, not a previously unseen holdout or reliability estimate. Independent human review remains pending. Raw prompts, replies, response records and input fingerprints stay private; selected fingerprints below identify the observations.

| Record | SHA-256 |
|---|---|
| 07-the-neighboring-vendor.md | `cfb012e4eb750f58157feab29fe30ff3ab2391a8c12bb0fbd707a7958ee1c493` |
| vendor-expected-results.md | `656c4ec5005d31301b31cf553ebefd583d1323a1c8637509c11df1126772dc86` |
| vendor-bridge, initial response | `5a4866671a6e4c714883b066936b4ed202a49b63ecc673cd6366472614595a11` |
| vendor-bridge, continuation response | `afc10830fbfe9c01614c688d44e9736067e4d3ec9367b2c2b262457b1f152790` |
| vendor-bridge-revised, initial response | `78f55d6826ff075dcac96f35ec4f640f1d49ba6894a1c7f920ceb3eaae51be90` |
| vendor-bridge-revised, continuation response | `8886a1ed97d6b8bbd282ad0dcf3191b58244bbc36a7bbd844995288214cf2c47` |
