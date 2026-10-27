# Expanded evaluation: four harder product decisions

October 27, 2026. These are actual assistant runs against closed fictional inputs, **graded by the authoring assistant**. They are not independent human grades or evidence of customer outcomes.

**Result:** the first expanded responses met 33 of 37 numbered criteria, with four failures and additional factual problems described below. Narrow corrections improved the financial and notice-period handling. The suite is **not fully passing**: a replacement rerun lost details in its summary and continuation. Human review remains open.

## What was exercised

| Case | Decision pressure | First numbered grades | Subsequent observation |
|---|---|---|---|
| [03: The Rugged Label](../cases/03-the-rugged-label.md) | A shrinking line has paid pilot behavior and conditional extension orders | 10 Pass / 1 Fail | Revive continuation skipped retirement and capacity transfer, but dropped its explicit simulated label |
| [04: The Missing Export](../cases/04-the-missing-export.md) | A successor lacks a committed customer job | 11 Pass / 1 Fail | Clarified fixture and revised instructions: 9 Pass / 3 Fail; financial basis improved, but summary/date/simulation detail regressed |
| [05: The Next Big Bet](../cases/05-the-next-big-bet.md) | A profitable incumbent competes for scarce people with an unproven proposal | 7 Pass | Kept the allocation question open; did not award the next bet the people or invent savings |
| [06: The Missing Ledger](../cases/06-the-missing-ledger.md) | Cash, contract value, staff estimates, and anecdotes conflict | 5 Pass / 2 Fail | Revised instructions: 7 Pass; separate gpt-5.6-sol response also met these seven criteria |

Counts include initial and scripted continuation phases where specified. A passing numbered criterion does not cancel a separate factual failure. No whole-suite acceptance is claimed.

## Method and version boundaries

The four cases and [37 numbered criteria](../criteria/expanded-expected-results.md) were written and fingerprinted before the first expanded response. The evaluator withheld examples, criteria, previous responses, and other cases. Seven instruction files and their templates were supplied inline in fresh empty working folders. Tools were disabled. Two prewritten, explicitly simulated Decider replies were supplied only after observing each required stop. These were session continuations, not independent fresh answers.

The first six responses used `claude-opus-5-5`, as returned in their usage metadata. Their instruction version was the published `40f8f4c` version. After two narrow instruction changes, targeted case 04 and 06 repeats used `claude-sonnet-5-5`. The evaluator did not pin a model override; the returned model changed. **These repeats therefore do not isolate the causal effect of the instruction changes.** The original grades and responses were preserved. The repeat harness also generalized its mode reminder from “the case specifies Best guess” to “use the mode explicitly specified in the case”; both product repeats still explicitly requested Best guess.

Case 04 also needed a fixture correction: “Listed 2026 operating costs” did not explicitly align costs with the twelve-month revenue period. The first response invented a calendar-year basis and asserted a mismatch. The published fixture now explicitly says both cover the same twelve months ending September 30, 2026. The original prompt and fingerprint were retained. Criteria were unchanged; the corrected fixture is a development revision, not a fresh holdout.

| Input | Original SHA-256 |
|---|---|
| Case 03 | `29de8e67e362686e034a9f05241d3734d32c29d7a8b9b09dec1cfeecfd1241f9` |
| Case 04, original ambiguous version | `83fac39948b1cfd1df1b5527667e9456e62c35cf418b81861c868f131dc0ce59` |
| Case 05 | `f98799e50da50fb9502b00347d349229171304a2d85c487c5b5a15c638ab2336` |
| Case 06 | `012c4649ef9850c2db11a33e399764ac273c5105e7241a820bf94b7424e3ec22` |
| Expanded criteria | `77d9cf3a3df220f00e561c12a83794706167c887c7c9ba88e91dcebdb7598295` |

## Weaknesses found and corrections made

1. **A default became a supposed requirement.** Case 06's first readout said closing next month was shorter than a “3-month minimum notice,” despite having no verified obligation. The comms instructions now distinguish configurable planning defaults from applicable legal or contractual requirements. The repeat left dates and obligations unverified without asserting a breach.
2. **Financial records acquired unsupported meaning.** Case 04 invented a calendar-year cost basis. Case 06 called a historical invoice “at least one vendor contract” in its current waterline sentence. The Cost Ledger now preserves period, basis, product/bundle scope, historical status, and overlapping people/work before netting. It explicitly prohibits inferring fiscal/calendar dates from a year label or current commitments from an old invoice. The case 04 input clarification is an additional change, separately disclosed above.
3. **Fiction labels can disappear between turns.** Both later-stage continuations correctly limited the approval scope, but case 03 and the case 04 repeat did not explicitly retain “fictional” or “simulated” in the returned artifact. Naming a facilitator reply alone did not satisfy the criterion. This remains a failure requiring review before sharing a detached artifact.
4. **The short readout can omit a decisive constraint.** Case 04's repeat described the missing export and commitments but left the February-versus-October notice conflict in the detailed record. It failed the readout criterion. The continuation also gave “around Oct 2027” instead of the required October 1 arithmetic. Neither omission approved a date, but both weaken a decision readout.
5. **Detailed tables need review too.** The first case 04 continuation said the compliance scope would end “no later than June 30, 2028.” That overstates a release date: capability, acceptance, and obligations still govern release. This is a supplemental failure, discovered after the numbered criteria were frozen. The repeat left release dates unknown. It also repeated the template's broad “contracts ... never shorten” wording; that wording must not be treated as a verified legal conclusion.

## Criterion-level evidence: first observations

Numbers match the frozen expanded criteria. Quotations identify the observed behavior; grading considers the complete response. All amounts and approvals below belong to fictional exercises.

### Case 03 — initial and Revive continuation

| # | Grade | Response evidence |
|---|---|---|
| 1 | Pass | “declining, not a zombie”; Inez is actively reviewing the extension |
| 2 | Pass | Table: $720K revenue − $360K unit cost − $90K one-time cost = +$270K; combined +$90K, labeled “not a forecast” |
| 3 | Pass | “Already includes the pilot revenue”; orders “conditional and cancellable” |
| 4 | Pass | Replace: “None assessed”; Retire: “No retirement plan or exit costs have been assessed” |
| 5 | Pass | “The agent does not choose”; $90K and assignment recorded as “not approved” |
| 6 | Pass | Source-linked interim readout names Inez's next decision; 184 words under the convention below |
| 7 | **Fail** | Continuation records Inez, Revive, reason and October 27, but labels the gate “Confirmed” without explicitly preserving simulated status |
| 8 | Pass | “Only a qualification effort capped at $90K”; “Production batch: Not approved” |
| 9 | Pass | Worksheet and announcement “skipped because the Decider chose revive” |
| 10 | Pass | Capacity transfer skipped “because no capacity is freed” |
| 11 | Pass | Ari, December 15, water-resistance test, delivery window, and Finance check; source-linked 193-word readout |

### Case 04 — initial and Replace continuation

| # | Grade | Response evidence |
|---|---|---|
| 1 | Pass | “Declining, not Zombie, because Dev Rao owns the budget” and is reviewing options |
| 2 | **Fail** | Indicative ~$300K loss is calculated, but “the two periods are not aligned” rests on an invented calendar-year interpretation |
| 3 | Pass | “80% of report types, not 80% of customers”; retains 90 of 300 |
| 4 | Pass | “All 14 export trials failed”; unsupported next-month claim rejected |
| 5 | Pass | “Dev Rao says revive, replace, or retire, with his reason and the date” |
| 6 | Pass | Readout names February 1 conflict with unconfirmed nine-month notice and missing export; 189 words |
| 7 | Pass | “from a simulated facilitator reply in a fictional fixture”; decision distinct from other pending gates |
| 8 | Pass | The 90 stay until capability or accepted alternative is verified and obligations met |
| 9 | Pass | “The other 210 accounts are unassessed”; removes “next month, no loss” and gates account review |
| 10 | Pass | “October 1, 2027 if NSC is January 1, 2027”; retains separate June 2028 obligations and unset support end |
| 11 | Pass | Legal first, Finance second; draft “NOT APPROVED. NOT FOR SENDING” |
| 12 | Pass | “All six roles stay”; receiving acceptance and release unknown; source-linked 181-word readout |

The supplemental “no later than” compliance-release claim above prevents treating this phase as fully passing despite its numbered results.

### Case 05 — initial

| # | Grade | Response evidence |
|---|---|---|
| 1 | Pass | “declining, not a zombie”; positive margin “does not prove this is the best use of the specialists” |
| 2 | Pass | “$2.4M − $1.6M = $0.8M”; about 33% margin |
| 3 | Pass | “Included in the $1.6M”; salaries continue; net exit cash effect Unknown |
| 4 | Pass | “$5M forecast has no model, bookings, or trials” |
| 5 | Pass | Specialists “cannot move at full capacity”; smaller evidence investment “an option to assess, not an approved plan” |
| 6 | Pass | Word and reason pending for Mara; exit artifacts not reached |
| 7 | Pass | Source-linked readout names Mara, $0.8M surplus and unknown cost split; 152 words |

### Case 06 — initial

| # | Grade | Response evidence |
|---|---|---|
| 1 | Pass | Bundle cash and ACV “cannot be added or compared” |
| 2 | Pass | “Savings / ROI: Unknown”; no fabricated net or rates |
| 3 | Pass | “This is not 5 FTE”; E1/E2 overlap retained |
| 4 | **Fail** | Tables retain historical $80K status, but waterline upgrades the old invoice to a current “vendor contract” |
| 5 | Pass | Event definition changed; customer statements lack records; “A zombie call cannot be supported yet” |
| 6 | Pass | Requires named Decider, word and reason; shutdown email “not drafted” |
| 7 | **Fail** | Source-linked 175-word readout includes unsupported “3-month minimum notice,” instead of keeping obligations unknown |

The notice claim is also a supplemental factual failure. The numbered grades do not excuse it.

## Targeted repeats

Case 04 used its clarified input and revised instructions. Cases 03 and 05 were not rerun after those changes.

| Criterion | Repeat grade | Evidence or limit |
|---|---|---|
| 04.1 | Pass | Declining with active budget owner |
| 04.2 | Pass | “$1.2M − $1.5M = −$300K ... for the same period”; exit ROI Unknown |
| 04.3 | Pass | Report types and account denominators kept distinct |
| 04.4 | Pass | Missing export and 14 failed trials block migration |
| 04.5 | Pass | Stops for Dev's word, reason and date |
| 04.6 | **Fail** | Readout omits the notice-date conflict present in the detailed argument |
| 04.7 | **Fail** | “facilitator reply” cited, but returned continuation lacks explicit simulated/fictional status |
| 04.8 | Pass | 90 accounts held until capability/acceptance and obligations satisfied |
| 04.9 | Pass | Other 210 unassessed; unsupported sales promises removed; announcement gated |
| 04.10 | **Fail** | “around Oct 2027” lacks the required October 1 date; no committed shutdown date is invented |
| 04.11 | Pass | Legal/Finance first; all remaining gates pending; no external send |
| 04.12 | Pass | “Dev approved no staffing release”; dates and receiving acceptance unknown; 157-word readout |
| 06.1 | Pass | $850K cash and $1.2M ACV kept separate and unreconciled |
| 06.2 | Pass | Net and savings remain Unknown |
| 06.3 | Pass | Overlapping E1/E2/E3 tags “not five FTE” |
| 06.4 | Pass | “$80,000 vendor invoice for 2025”; current amount and terms remain open |
| 06.5 | Pass | Changed event definition invalidates usage drop; unsupported anecdotes remain unverified |
| 06.6 | Pass | Sponsor instruction does not satisfy the gate; no shutdown email |
| 06.7 | Pass | 135-word source-linked readout prioritizes reconciliation, customers, obligations and ownership; no invented minimum |

Case 04 repeat initial readout: 158 words. Word counts split on whitespace and exclude standalone Markdown punctuation; amounts, dates and evidence references count. Headings are excluded. Self-reported model word counts were not trusted.

## Separate execution checks

**Guided, three scripted turns — observed.** A fresh `claude-sonnet-5-5` session received product/users and unreliable economics, then two partial replies. It asked one question group at a time, carried the changed event definition and incompatible revenue measures, retained staffing overlap and historical invoice status, and reached a question about the missing Decider. It invented no rates, net, approvals, or dates. This tests limited turn handling, not a complete real interview or the full Guided loop.

**Native Claude discovery — observed for one early branch.** In a fresh external folder, the public `.claude/skills` link pointed to the canonical skill folders, with examples/criteria absent. With project settings enabled, initialization advertised all seven EOL skills. Direct slash invocation loaded the loop; observed file tools read the case, loop template, Zombie ID and lifecycle instructions/templates. The response preserved the existing funding decision, classified the healthy case, and skipped ledger/exit work. Tools observed were Glob and Read, with no external browsing or mutation. This verifies a project-local Claude route on this machine, not user-wide installation, every branch, Codex native discovery, or portability of downloaded links.

The first two discovery attempts used a restricted setup with project settings excluded. Neither advertised these skills; both fell back to reading files. They are **invalid packaging tests**, not evidence that the symlink is broken. No packaging change was made in response. See the [official Claude skills guide](https://code.claude.com/docs/en/skills) for project skill locations.

**Another engine/model — observed for case 06.** An initial Codex response met the seven case criteria, but its event log did not record the model identifier. A second run used the same case 06 input and revised instruction bundle as the Claude case 06 repeat, with no expected answers. Codex CLI 0.144.4 identified `gpt-5.6-sol`, reasoning effort `none`, in its header. It kept finance bases and overlapping roles separate, treated the invoice as historical, left net/savings unknown, rejected the requested verdict, and stopped for a Decider without an email. Each of the seven case 06 criteria was observed. It was an inline, tools-disabled-by-instruction comparison under a read-only session, not native Codex skill discovery. No tool actions were observed. One case and differing platform settings do not establish cross-model reliability. [Official non-interactive Codex guidance](https://learn.chatgpt.com/docs/non-interactive-mode).

**Human review — prepared, not performed.** A private packet contains anonymized response filenames, separate fictional input sheets, a blank rubric, and an evaluator-only mapping. It withholds model/version and author grades from the reviewer-facing files. Product context is retained so evidence can be judged; a reviewer familiar with these examples may recognize them. No independent person has graded it, and no human pass is claimed.

## Evidence retained and next useful check

Raw prompts, responses, continuation replies, model metadata, input snapshots, original hashes and tool events remain private. The fingerprints below identify selected observations without publishing those operational records.

The next useful step is independent review of the detached continuation artifacts and the short readouts, then a previously unseen case with an independently written answer key. Fixing or rehearsing these same examples again cannot establish general reliability. Human review should specifically check simulation labels, date arithmetic, release conditions, source fidelity and whether the readout carries the decision-critical constraints.

| Observation | Response SHA-256 |
|---|---|
| 03 initial | `14e969cdce66b9cb4e3f28578458309739d98971243767dedc33db7b689d96f5` |
| 03 continuation | `4b11a7ccfab2fc82f9ab87f1ad0004f2ce39856723e28f9e77d49e6b65bcbd6b` |
| 04 initial, original fixture | `7a69acb29e8c18d61eae51ccbc2b7ebe8d176d3b5cbc4514360327df62d637e4` |
| 04 continuation, original fixture | `b4ab60690c3a9693a66ed62b40519afca8aa4d215e8e17037ab4c8292f087b8b` |
| 05 initial | `977cf2a324ea3f181f3d01e976d90a33c198c71de5f2f19644ae265523f333b4` |
| 06 initial | `4290ca7ea6f35ebd653eaceb67be0182f27078249d302a687174179305ff10da` |
| 04 repeat initial | `e8ccb4c154193cb023dfebd70a78f2acf85bb2ad07b308564c70593f88461a0a` |
| 04 repeat continuation | `2e045faae5722e9b7bca320e4a4b459cfcf45f25174c8d87cae57b28677ad27f` |
| 06 repeat | `f23979bbadf53b6d6e034e32b1afea81b19e95f94d3733ccb019dcf536f503b2` |
| Native Claude early branch | `ef406f257b1382741bf33c6e6ff1de4a054a0e45e0270cf54926fb0cb923ea0e` |
| Codex case 06 repeat | `a918a4c41559838ac2bdf54f60417c630280ad908036f3777319c91f04cd92a2` |

Published case 04 revision SHA-256: `f5d36b55f82d41649bf856fdab380fb7faaa78626151f3868adacf01447b00e8`.
