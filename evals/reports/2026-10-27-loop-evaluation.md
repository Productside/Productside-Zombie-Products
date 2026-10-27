# Zombie-to-Exit Loop: behavioral evaluation

Date: October 27, 2026 (America/New_York). Test model reported by the CLI: **claude-sonnet-5-5**. The scenarios and skills were assistant-authored, and another assistant reviewed the test responses against the criteria. This is a two-scenario synthetic evaluation, not customer validation or an independent human review.

## Method

The unchanged [case inputs](../README.md) and [expected results](../criteria/expected-results.md) were authored before the runs. Each initial session received the seven skills' instructions and templates plus one case, with examples and expected answers withheld. Model tools, skill discovery, and MCP access were disabled; no browsing was available. The runner used the configured Claude model and recorded its returned identifier rather than assuming a model version.

Baseline and development passes used ignored local workspaces. Final acceptance sessions started in separate, empty temporary folders outside the Project to avoid inheriting its production instructions. Each case used a fresh session. The retirement continuation resumed only its own session after observing the required Decider stop, then supplied the prewritten **simulated** facilitator reply. This tests a scripted gate crossing, not a real person's approval or a real multi-turn business decision.

Prompts, responses, model metadata, session IDs, and hashes of every supplied skill/template and case are retained locally. Raw sessions, local paths, and production materials are not published. The excerpts below support the grades; exact wording is evidence of these responses only, not a future word-match test.

## What the baseline exposed

Both products received the intended overall finding, and the first case stopped at the Decider. That did not make the runs passes.

| Weakness | Observed response or conflict | Correction |
|---|---|---|
| Reversed question polarity | “Is defending market share still profitable?” was answered “Yes: it is not profitable.” The healthy case answered No because it was profitable. | Rephrased the question so every Yes points toward decline; aligned both skills, templates, and the existing worked example. |
| Missing evidence became absence | “Users migrating: Not present — No migration is recorded.” Support uncertainty was also answered No. | Required Unknown for missing evidence and affirmative counterevidence for Not present; added the distinction directly to the Zombie ID template. |
| A count looked like a verdict rule | The rubric implied mostly Yes was needed, even when economics and ownership established a problem while other answers were Unknown. | Made the count diagnostic, with current value, economics, and decision ownership carrying the finding. |
| Early branch still did extra work | The healthy case said the loop stopped “after Step 1 and the ledger” and left a conditional Decider item among pending gates. | Stop before the ledger and later exit work; preserve existing funding records and mark skipped gates Not applicable. |
| Readouts lost their receipts | Baseline summaries had no S1–S5 references despite using those records. | Required source references in the short readout and consequential artifact claims. |
| Cost and cash were blurred | Outside payments were described as cash saved while cancellability, exit costs, and revenue run-off were unknown. | Separated operating net, redeployable people, potentially avoidable payments, lost revenue, and unknown exit cash effects. |
| Generic release timing overrode obligations | Continuation released support “partly” after EOL although the case retained those roles through closure. | Specific return, support, and contractual obligations now override the generic release examples. |
| Unknown replacement coverage sounded confirmed | The continuation said some titles were available and that no alternative existed for the remainder, despite an unassessed path. | Distinguished unassessed, unavailable, and confirmed available; a catalog percentage is not a customer percentage. |
| Drafted steps looked completed | Rules-of-the-road rows marked alignment and data pulls Yes merely because the plan listed them. | Required Planned / Pending / Confirmed status with evidence. |
| Short readout overran its limit | One later development response had 207 words against a 200-word ceiling. | Added a 120–150-word target to leave headroom for citations and labels. |

The baseline also had important strengths: the $960,000 cost total and $120,000 loss were correct; salaries were recognized as retained payroll; the notice conflict was found; the healthy product was not retired; and the scripted retirement did not automatically approve later gates.

## Final acceptance grades

Grades below apply to the final skill versions. Pass means the observed response met the listed criterion in this exercise. It does not establish reliability across future runs.

### Case 01: The Last Envelope — initial response

| Original criterion | Grade | Response evidence |
|---|---|---|
| Classification | Pass | “declining zombie (recommended; PM confirmation pending)” with shrinking demand and default funding (S1, S2, S4). |
| Lifecycle | Pass | Decline derived from current demand/cost signals rather than the product's age. |
| Ledger | Pass | “$960,000 ... $840,000 ... Net on listed costs: −$120,000, excluding overhead and exit costs.” |
| Capacity versus cash | Pass | “$540,000 ... loaded people cost for 8 roles” separated from “$420,000 ... outside payments”; moved salaries are not savings. |
| Alternatives | Pass | Separate revive, replace, and retire arguments; collector demand, streaming coverage, migration costs, and exit costs remain unknown. |
| Mandatory stop | Pass | “Pending. Hard stop. No name, word, or reason.” No exit worksheet, announcement, or transfer was produced. |
| Customer boundary | Pass | The supplied “everything online, nothing changes” email was identified as unsupported, not adopted. |
| Readout | Pass | **159 words**, source-linked, decision pending, and asks for one named Decider and their word/reason. |

### Case 01 — scripted continuation

| Original criterion | Grade | Response evidence |
|---|---|---|
| Decision record | Pass | “Confirmed (simulated): Retire” for Ellis Rowan on October 27, 2026, with the exact supplied reason. |
| Contract overrides default | Pass | Draft EOS November 1, 2027; the sponsor's August 1 request is rejected under the unconfirmed nine-month rule. |
| Later phases | Pass | Draft EOE February 1, 2028; EOL May 1, 2028; EOSL August 1, 2028. All remain gated. |
| Communication order | Pass | Legal and finance first; sales/support aligned before customer notice; bundling has a planned stop; no external send authorized. |
| Promise check | Pass | “No confirmed alternative yet”; no claim that the remaining 60% is covered. Dates and the title-level guide are gated, and the original unsupported email is removed. |
| Capacity | Pass | Support and platform remain through closure, warehouse through returns; payment terms and benefit are Unknown; no transfer is approved. |
| Pending gates | Pass | Stage, verdict, figures, notice, text, and trade remain Pending. “The Retire decision is not an approval of dates, the announcement, or the trade.” |
| Final readout | Pass | **169 words**, sources inline, simulated decision distinguished from the unconfirmed plan and capacity request. |

### Case 02: The Second Exposure — early stop

| Original criterion | Grade | Response evidence |
|---|---|---|
| Classification | Pass | “looks Healthy, not a zombie”; retirement argument identified as image-only. |
| Current evidence | Pass | Revenue/repeat-purchase growth and Mina Chen's current funding record, rather than age or the earlier decline. |
| Economics | Pass | $3.6M minus $2.7M equals $0.9M, about a 25% margin; no exit cash or ROI claim. |
| Customer job | Pass | Physical keepsake distinguished from a filter service; opinion survey not treated as purchase evidence. |
| Early branch | Pass | “Cost Ledger: Not applicable / skipped” and decision, exit plan, announcement, and transfer skipped. |
| Ownership | Pass | “existing record funding the line for 12 months ... is preserved”; no fresh revive word requested. |
| Next step | Pass | Mina's existing quarterly review, with demand, margin, safety, supply, and replacement-evidence triggers. |
| Readout | Pass | **179 words**, cites S1–S4, preserves the small-sample limit, and names the next owner. |

Additional checks added after the baseline: missing migration evidence now remains Unknown; the question's yes/no direction is consistent; skipped gates are absent from outstanding approvals. These are regression observations, not previously unseen holdout tests.

**Observed result:** all 24 original criterion rows passed in the final three-response acceptance sequence, with no shared critical failure observed. This is a bounded observation, not a reliability estimate. Development responses and baseline failures remain retained separately rather than being replaced by the successful outputs.

### Acceptance response fingerprints

SHA-256 of the locally retained response Markdown, including its trailing newline:

| Response | SHA-256 |
|---|---|
| Last Envelope, initial | `6837bb73ae403cc83a587039b9f0b771da060dbe0d50c996c0d4f4ff01441a8a` |
| Last Envelope, continuation | `c44d2b74afc1b170a5b94d49e843e87fae5fe5d90781f4daaf93c3858b738bb4` |
| Second Exposure, early stop | `be7e811cb5fe3ed0bc0913706c18fb44b8b7fc29d8b78b70b49572f2df33630f` |

## Limits and follow-up

- These are two author-written fictional cases on one model, graded by the author. They do not establish representative customer usefulness, statistical reliability, other assistants' behavior, or blind human agreement.
- Skills and templates were supplied inline. Native installation, automatic discovery, and the separately linked announcement skill were not exercised; the documented fallback was used.
- The generic Codex skill validator rejects the Project's existing custom frontmatter fields. Those fields were preserved; successful local content checks do not mean a native Codex package has been validated.
- More cases should cover a genuine revive, replace with a verified migration path, thin evidence, and adversarial requests to bypass gates. Those paths have not been evaluated here.
- The 200-word count excludes the readout heading and includes the body labels and citations. Shorter output was not accepted as a substitute for the required reached artifacts.

The readout, gates, and artifacts remain drafts until their actual human owners confirm them in real use. A simulated Decider reply in this exercise changes none of those real-world permissions.
