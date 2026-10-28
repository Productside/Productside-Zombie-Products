# Real transition patterns, fictional decision tests

October 27, 2026. This release adds four sourced [case cards](../../case-studies/README.md), three new fictional exercises, and a [Customer Transition Scorecard](../../templates/Customer-Transition-Scorecard.md). Actual model runs are graded by the authoring assistant. Independent human review remains pending.

## Evidence boundary and method

The factual cards cover Atlassian migration overlap/credits, Microsoft's limited security bridge, Google's Stadia compensation announcement, and the Hipchat/Stride handoff to Slack. They establish what providers documented or announced; completion, retention, profitability and internal capacity changes remain unverified unless sourced. Program guidance was checked October 27, 2026; historical announcements retain their original dates. The fictional exercises do not supply private facts about those providers.

Cases 08–10 and their [thirty criteria](../criteria/customer-transition-expected-results.md) were fingerprinted before the first run. The criteria remained unchanged; two input clarifications are disclosed below. Each initial fixture supplies a simulated Decider decision; the tested behavior is preserving that record and drafting the reached transition branch while leaving every other gate pending. No new real decision or approval occurred.

Baseline runs used the published `8f090d9` seven-skill instruction/template bundle. The assistant received one case inline in a fresh empty working folder; tools were disabled and factual cards, examples, answer keys, other scenarios and previous responses were withheld. First repeats used the original inputs; the final round used clarified cases 09/10. Repeats also included the newly linked scorecard template. This changes both instructions and supporting context; it is a development comparison, not a controlled causal experiment or unseen holdout. Claude CLI 2.1.311 returned `claude-sonnet-5-5` for every response in this report, with no tool access or reported web searches.

## Baseline: 22 of 30 numbered criteria

The initial responses preserved the human gates and avoided universal migration/refund promises. They exposed practical gaps:

- Case 08 downgraded an explicitly same-period comparison to an assumption. Cases 09/10 also left alignment uncertain; their original wording referred to the last annual period without the explicit “same period” sentence used in case 08. That fixture ambiguity is disclosed below; their intended mathematical criteria failed, but the ambiguity should not be attributed solely to skill behavior.
- The bridge response compared $40,000 fees with $70,000 effort and gave percentage coverage, but omitted the required explicit −$30,000 comparison.
- The scorecards showed risk but lacked row-level actions and responsible owners; relationship outcomes were not explicitly recorded as unobserved.
- The overlap response omitted data permissions.
- In a later comparison the bridge response confused the January 15 next-bet review with the December 15 bridge review, although it had carried the correct bridge date earlier.

### Criterion-level baseline grades

Numbers match the frozen criteria. A passing criterion does not cancel a separate factual or drafting error.

| Case / criterion | Grade | Response evidence |
|---|---|---|
| 08.1 | Pass | Leah's existing Replace decision and Owen's assignment retained; other gates pending |
| 08.2 | **Fail** | −$300K calculated only “on the assumption” of alignment despite S1's explicit same-period record |
| 08.3 | Pass | “$12,000 − $3,000 ... plus $2,000 ... $11,000 before taxes”; $12,000 renewal |
| 08.4 | Pass | $180K kept as a separate incremental one-time transition item, not annualized or multiplied |
| 08.5 | Pass | 8 accepted, 32 unassessed including 6 blocked; test acceptance distinguished from production approval |
| 08.6 | **Fail** | Production readiness/export reconciliation/rollback discussed, but data permissions omitted |
| 08.7 | Pass | Conditional July 1 EOS, unapproved dates; unresolved accounts not cut off by generic dates |
| 08.8 | Pass | January 1 specialist request not supported; missing baseline/target and receiving acceptance retained; final trade conditional |
| 08.9 | **Fail** | Five scorecard rows show status/findings but no row-level action/owner fields or explicit relationship outcome status |
| 08.10 | Pass | Source-linked 147-word readout; pricing, readiness risk and Owen; Legal/Finance first; “free” rejected |
| 09.1 | Pass | Existing simulated Retire record and Rina retained; bridge/other approvals pending |
| 09.2 | **Fail** | “periods are unreconciled, so the net stays Unknown”; fails intended matched-period criterion, with fixture ambiguity noted below |
| 09.3 | **Fail** | “20 × $2,000 = $40k” against $70K and 57% coverage, but explicit −$30K term comparison absent |
| 09.4 | Pass | Security-only scope; normal support/features excluded; no orders or bridge approval |
| 09.5 | Pass | Existing troubleshooting through September 30 retained; proposal does not waive it |
| 09.6 | Pass | Six blocked and fourteen unassessed; bridge does not supply connector or prove alarm delivery |
| 09.7 | Pass | Supported path, data/history/restoration/training open; no authorized support end; conditional July 1 EOS |
| 09.8 | Pass | Same two specialists cannot serve both; metering 2h to 30min target and proposed January 15 review retained |
| 09.9 | **Fail** | Owner/action fields absent; later comparison calls January 15 the post-bridge review, conflating it with the December 15 bridge review |
| 09.10 | Pass | Source-linked 152-word readout covers fees/effort, support mismatch, specialist conflict and Rina; announcement gated |
| 10.1 | Pass | Elena's decision, Cal and schedule-scoped approval retained; other gates pending |
| 10.2 | **Fail** | “net is Unknown pending reconciliation”; fails intended matched-period criterion, with fixture ambiguity noted below |
| 10.3 | Pass | $16K eligible / $9K paid / $7K unpaid; 280/150/130 records; failed routes are a subset |
| 10.4 | Pass | Exclusions retained; no all-paid assertion; alternate payment process requires approval |
| 10.5 | Pass | 40 downloads are untested and other 80 unverified; no completed-migration claim |
| 10.6 | Pass | Viewer cannot deliver interactive exercises; no equivalent successor invented |
| 10.7 | Pass | Permissions, restoration, retention and archive-link expiry gated |
| 10.8 | Pass | Conditional July 1 EOS, December 31 access commitment; no January 1 staffing release |
| 10.9 | **Fail** | Five scorecard rows lack row-level actions/owners and an explicit relationship-outcome record |
| 10.10 | Pass | Source-linked 156-word readout includes payment status, absent job destination, untested data and Cal; messaging gated |

The baseline overlap decision-option paragraph additionally said pure retirement “frees the $1.2M cost base.” Its final capacity table was conditional, so criterion 08.8 passed, but that earlier broad claim is a supplemental error requiring correction. Keep gross operating cost distinct from transferable capacity everywhere in the pack.

## Disclosed input clarification

The original case 09 and 10 fixtures tied costs to the last twelve-month period and listed comparable annual revenue, but did not explicitly state the latest revenue covered that identical window. The intended criteria expected matched-period arithmetic. Both baseline and first repeat questioned the link. We clarified each fixture with an explicit same-period sentence, preserving all figures and the original criterion file. Original prompts and input hashes remain retained. The final round uses these clarified inputs; it is not an unchanged-input test of the instruction fix. Case 08 and case 07 inputs remained unchanged.

## Focused changes

- **Cost Ledger:** honor explicitly supplied period links. Unknown accounting basis can qualify the comparison without erasing matched-period listed-cost arithmetic.
- **Free the Living and output templates:** the trade uses net releasable capacity after continuing transition work. A gross operating-cost total is not a transferable budget; unknown amounts, dates and acceptance remain visible in the cover too.
- **Loop:** fictional status travels into resumed outputs; review dates stay attached to their program; a material obligation/date conflict belongs in the short readout.
- **Comms:** temporary programs retain scope, duration, exclusions, approvals and their incremental revenue-minus-cost comparison, with loaded effort distinct from cash. The five-area scorecard records evidence, next actions, owners, conditions and status, including unobserved relationship outcomes.
- **Zombie ID and fixed-term estimates:** active review is ownership even before the final word. A whole-term quote must not become a per-order variable cost without evidence.

## Development repeats: preserve the regressions

Three first repeats and a two-phase case 07 regression were actually run. These are development observations, not final acceptance scores:

- **08:** matched-period arithmetic and the net-capacity trade improved. The phrase “tested accounts (8) are ready” overstates production readiness, despite contrary caveats later in the pack.
- **09:** the repeat still questioned the original fixture's period link. It also wrote “Shortfall ≤ $30,000.” With fixed $70,000 effort and at most $40,000 fees, the full-takeup shortfall is $30,000 before other costs; lower takeup does not establish a smaller shortfall. The repeat also inferred per-order cost behavior without evidence.
- **10:** the repeat still questioned the original period link. It described compensation as “mostly unpaid,” although $9,000 of $16,000 and 150 of 280 records were paid. This is a supplemental factual error.
- **07:** the initial phase treated active review as “nobody owns the decision,” failing original criterion 1. The other eleven criteria were observed across initial and scripted continuation: **11/12**. Its continuation carried that unsupported Zombie verdict forward. The scripted reply was supplied only after observing the stop.

The last changes addressed ownership and fixed-term cost inference. Then cases 08–10 and both case 07 phases were run again. No final response was manually repaired before grading.

## Final observations: 29 of 30 numbered criteria; not a clean suite pass

Case 08 fails criterion 6. Case 10 meets its ten numbered checks but invents an archive-content detail elsewhere; the shared fabricated-evidence rule prevents calling its phase a pass. Case 09 meets its ten numbered checks in this one observation. These are assistant grades, not independent judging or a reliability estimate.

| Case / criterion | Grade | Final response evidence |
|---|---|---|
| 08.1 | Pass | “Declining, not a zombie”; Leah's supplied Replace record and Owen retained; other approvals Pending |
| 08.2 | Pass | “$900,000 − $1,200,000 = −$300,000” on an explicitly same-period basis; salaries continue |
| 08.3 | Pass | “$9,000 ... Add $2,000 ... $11,000” before taxes; $12,000 renewal; other-account terms Unknown |
| 08.4 | Pass | “$180,000 for the entire six-month proposed period,” separate from annual cost and unknown exit ROI |
| 08.5 | Pass | 8 accepted tested jobs, 32 unassessed including 6; “Production move: not approved” |
| 08.6 | **Fail** | Backup, SLA, reconciliation, rollback and acceptance retained, but the full pack again omits data permission |
| 08.7 | Pass | “Earliest July 1, 2027” conditional; reporting obligations through December 31 constrain release |
| 08.8 | Pass | “Net releasable amount, unknown”; baseline/target/receiving acceptance absent; no full-cost transfer |
| 08.9 | Pass | Five evidence/action/owner/condition/status rows; post-transition measures “Unknown or Not observed” |
| 08.10 | Pass | Source-linked 162-word readout; bounded price, readiness, obligation conflict and Owen; Legal/Finance first |
| 09.1 | Pass | Supplied simulated Mateo Retire and Rina; bridge/dates/email/waivers/staff release not approved |
| 09.2 | Pass | Same-period $500K − $800K = −$300K; retained salaries separate from cash |
| 09.3 | Pass | $40K maximum fees versus fixed $70K effort, explicit −$30K full-takeup comparison; no orders |
| 09.4 | Pass | Security-only proposal; eligibility open; normal support, connector fixes and features excluded |
| 09.5 | Pass | Normal troubleshooting through September 30 remains; July security-only proposal does not waive it |
| 09.6 | Pass | Six blocked, fourteen unassessed; connector and alarm delivery unproven |
| 09.7 | Pass | Supported fallback, export/restoration/training/escalation; conditional July EOS; no authorized support end |
| 09.8 | Pass | Two specialists double-booked; no July release; 2h to 30min target and January 15 metering review retained |
| 09.9 | Pass | Five-area scorecard and outcome record; “bridge review of Dec 15, 2027 is separate and is not a renewal approval” |
| 09.10 | Pass | Source-linked 161-word readout includes scope, fee/effort gap, support mismatch and Rina; announcement gated |
| 10.1 | Pass | Elena's simulated decision and Cal retained; schedule-scoped approval distinguished from pending other gates |
| 10.2 | Pass | Same-period $600K − $900K = −$300K; retained salaries and refunds not recurring cash savings |
| 10.3 | Pass | $16K scheduled / $9K paid / $7K unpaid; 280/150/130 purchase records; sixteen failed routes a subset |
| 10.4 | Pass | Scope/exclusions and payment remedy unresolved; no all-paid or universal promise |
| 10.5 | Pass | 40 downloads untested, other 80 unverified; no completed-migration or retention claim |
| 10.6 | Pass | No interactive successor; viewer is not equivalent; compensation not a restored workflow |
| 10.7 | Pass | Permissions/retention/restoration and January archive expiry gated; no automatic deletion |
| 10.8 | Pass | Conditional July EOS, December interactive commitment; no January staff release; target/acceptance missing |
| 10.9 | Pass | Five-area scorecard with Cal coordinating and further owners to assign; actions/statuses and unobserved relationship outcomes |
| 10.10 | Pass | Source-linked 140-word readout: $9K paid/$7K unpaid, missing job destination, data risk and Cal; Legal/Finance and announcement gates |

### Remaining errors and limits

- **Archive source fidelity is a phase failure.** Case 10's draft announcement says “Downloads show saved screens.” The fixture only says that about the viewer; it does not describe archive contents. This invents a supplied-evidence detail even though the numbered restoration checks pass. The phrase must be removed or verified before any real use.
- **Missing permissions remain a failure.** Case 08 must explicitly require authorized data handling before migration. The linked scorecard contains this requirement, but the generated pack did not carry it through.
- **Unknown is not zero.** Case 08 says “Nothing is paid or observed”; the fixture supplies no payment record, so paid status should be Unknown, not a claim that nothing was paid. This supplemental source-fidelity error further prevents calling that response clean.
- **Owner assignment remains work.** Several scorecard rows name a coordinator or unassigned function rather than an accepted individual. That accurately exposes missing evidence; it does not establish operational readiness.

The final artifacts remain drafts for review. No outgoing message, move, refund or capacity transfer was performed. Publishing evaluation failures does not approve those artifacts for use with customers.

### Unchanged external-vendor regression: 12 of 12 numbered criteria

The final case 07 initial response recognizes Nora's active ownership, calculates −$180K with bundle contribution unknown, keeps the external path viable, bounds the draft discount, preserves pilot failures and stops for Nora. A scripted fictional reply then supplies Retire, Tessa's assignment and the signed offer. Six continuation criteria are observed: fictional status/record; bounded signed terms; account-level acceptance/data/support/fallback; conditional July EOS with December obligations; Legal/Finance-first vendor coordination; and no authorized cash or staffing release. Original criteria were not expanded to count scorecard preferences.

| Original criterion | Final evidence |
|---|---|
| 07.1 | “Declining, not a zombie: Nora Vale owns an active review” |
| 07.2 | “–$180K product-level gap before any unmeasured bundle effect” |
| 07.3 | Independent Neighbor Archive retained as a candidate destination while retiring the owned line |
| 07.4 | $750 derived; offer unsigned initially, twelve months then $1,000; exclusions and new bundle bill retained |
| 07.5 | Four passed/two failed; eight connector accounts blocked; rest unassessed |
| 07.6 | “Next: Nora names the word and her reason”; 140-word initial readout; no premature announcement |
| 07.7 | Resumed output explicitly fictional; Retire, reason/date, Tessa and signed S6 retained |
| 07.8 | Eligibility/deadline, $750 first year/$1,000 afterward and exclusions retained; no permanent/free promise |
| 07.9 | Account checks, acceptance, data permission/security, support ownership and supported fallback required |
| 07.10 | Conditional July 1 EOS; December 31 obligations; no forced shutdown for unresolved accounts |
| 07.11 | Legal/Finance first; Tessa coordinates Beacon; external commitments and draft announcement gated |
| 07.12 | Salaries not cash, outside cancellation unassessed, release/receiving approval pending; source-linked short resumed readout |

**Supplemental capacity wording remains weak:** the cover calls the two gross specialists “Net capacity” before release evidence exists, while the detailed transfer says net capacity cannot yet be calculated. It also asserts net is “smaller than $160K” without a supplied deduction. Use Unknown until the net amount is evidenced. No actual transfer is authorized, so the original no-release criterion passes; this is not a contradiction-free pack.

### Readout lengths

Counted from actual response text, excluding the heading and ending at the next heading/divider. Whitespace-delimited tokens containing a letter or number count; source IDs and dates count. Models' self-reported lengths were not used.

| Observation | Baseline | First repeat | Final round |
|---|---|---|---|
| 08 | 147 | 159 | 162 |
| 09 | 152 | 147 | 161 |
| 10 | 156 | 140 | 140 |
| 07 initial | Not rerun as a new baseline here | 165 | 140 |
| 07 scripted continuation | Not rerun as a new baseline here | 155 | 160 |

All these readouts meet the 200-word ceiling. Short summaries do not establish full-pack source fidelity.

## Structural checks and review boundary

Canonical YAML and existing human gates are preserved. Relative links, exact public allowlist, private-material exclusions, restricted-name/credential scans, and fixture arithmetic/date checks are run before publication. Generic Codex skill validation still rejects pre-existing custom frontmatter; parsing is not a native installation/discovery test. No native discovery, cross-model reliability or real customer outcomes are established by this release.

A private reviewer packet pairs anonymized input and response filenames and a blank rubric, withholding run versions, model names, author grades, answer keys and factual cards. Fictional product context stays visible; a reviewer may recognize it. No independent person has graded this release. No customer or vendor was contacted.

Raw prompts, responses, metadata, input hashes and grading notes stay private. Response fingerprints identify observations without publishing operational records. Prior reports retain their original failures and limits; this release does not retroactively turn them into passing results.

## Input and response fingerprints

SHA-256 of the retained UTF-8 files, including their final newline. Input originals are retained in private prompts; clarified inputs are the public files. All final runs used the same frozen instruction/template bundle.

| Input | SHA-256 |
|---|---|
| Original evals/cases/08-the-overlap-window.md | `dcc04ff7a064254b2d815fcfb66af8d8d5cb53b7e227233e18dabf9c3f8cf3bf` |
| Original evals/cases/09-the-last-patch.md | `a4447584210747fe730141ee0cf1be1547ff52a851e3c285a24a2cd263e4a143` |
| Original evals/cases/10-the-final-session.md | `ade6fbf2b3d4f3c580b22a314d61c5cf100732d54ea611294cb2d904444fd132` |
| Original evals/criteria/customer-transition-expected-results.md | `16e75e1facd01313d4858b0916747ab1ead8131d24399aaff3a74b52613d72bf` |
| Clarified evals/cases/09-the-last-patch.md | `c392cc8073cfac478f51394aba83b13793e935f747a80c51c42335f222d16d2f` |
| Clarified evals/cases/10-the-final-session.md | `a681d72a2e0207c60e8e54301df1a884cc3b807bcd6fbdf5f6b411c5cc8f6a38` |

| Observation | Response SHA-256 |
|---|---|
| bridge-baseline / initial | `7c0479e563f66e45d9f71969f94d54e872b03832da8bb1a951197378a2d4a8b0` |
| bridge-final / initial | `4be90946865a46178ffee10651f6569b888290f196e90c803d89af4fd153cd7e` |
| bridge-revised / initial | `61330c4b706c791405440dce578899b16cbc6a8d90d4a184c078917b4f45ce92` |
| overlap-baseline / initial | `69523153ef2d48ed689f9eee98cce3215a70ff65d1b9f0a2c7a559fe39c7fa12` |
| overlap-final / initial | `bc63cae893dd32fbcfc4bf92aadd71045787e12b1f048792d28f185d969454ba` |
| overlap-revised / initial | `b934f0f5048c99f32b1faaf7aa32db8cc9a604328c4cb9359986e3b21f306264` |
| refund-baseline / initial | `c2398fa5d20245e4ac2144e453e454e5b9d817c5e347580bfb2275910c0c2d3f` |
| refund-final / initial | `751336b5c473ec847ab01ef3ffc80c3b5975590a87fa0846e9a2315a4170d218` |
| refund-revised / initial | `8c59e84ea6cc011fa74b6a1b4e81d4ed96bece832e1056233593071967e1bef6` |
| vendor-final / continuation | `46c225c324b8e51612e2dbbf8dcff0c1456ec5d8c583d0bb6770e0c454363ac8` |
| vendor-final / initial | `feaa748255dd1222f425380b0bdcbf60522c9f11535508e46b1a054bf1bb7a8b` |
| vendor-regression / continuation | `7cad60ca467abd77bf50b9162efd3aecd7e2c81762f15faaf85e70474fca0230` |
| vendor-regression / initial | `a47d62d262c5dc37c83b589db4df7a6358e7c34aaabd4899bc53c68440cff1db` |
