# Evaluation status

Updated October 27, 2026. See the [original behavioral findings](reports/2026-10-27-loop-evaluation.md) and [expanded criterion-level grades and execution checks](reports/2026-10-27-expanded-evaluation.md).

| Check | Status | What that means |
|---|---|---|
| Two fictional inputs and separate semantic grading criteria | Authored before baseline; now exercised | Inputs and original criteria were not changed to fit the responses |
| Historical anchors | Checked against linked first-party sources | Supports the limited background statements, not the invented case evidence |
| Arithmetic and date expectations | Checked locally | Cost totals, margins, and timeline arithmetic are internally consistent |
| Relative links, publication allowlist, and private-material exclusions | Checked locally | The scenario package is structurally ready to use |
| Fresh-assistant initial runs | Baseline, development, and final acceptance executed with claude-sonnet-5-5 | Final acceptance used separate empty temporary folders, inline instructions, no tools, and no expected answers |
| Case 01 scripted gate continuation | Executed after observing the Decider stop | A simulated facilitator reply supplied Retire, name, reason, and date; all other gates remained pending |
| Case 02 early-stop behavior | Observed in final acceptance | Healthy finding preserved the funding record and skipped the ledger and exit work |
| Final semantic criteria | Assistant-graded: 24 of 24 observed in the three acceptance responses | Includes both initial cases and the scripted continuation; this is not independent human judging |
| Readout length and traceability | Final readouts: 159, 169, and 179 words, with supplied evidence references | Length excludes the readout heading; reached artifacts are separate |
| Skill revisions | Applied and retested | Question polarity, Unknown versus absence, early branches, source-linked summaries, cash/capacity distinctions, obligations, and draft/confirmed states |
| Generic native Codex skill validator | Does not accept existing custom frontmatter | Canonical YAML, names, descriptions, intents, and licenses parse; native installation/discovery remains unverified |
| Four expanded cases and scripted Revive/Replace continuations | Executed; not fully passing | First responses: 33 of 37 numbered criteria; supplemental errors and repeat regressions are preserved in the expanded report |
| Targeted expanded repeats | Executed with revised instructions; model also changed | Case 04: 9 of 12; case 06: 7 of 7. Case 04 fixture period was clarified; no causal claim that instructions alone explain the changes |
| Guided interaction | Three scripted turns observed | Partial answers and unknowns carried forward; full Guided workflow and real interview quality untested |
| Native Claude discovery | Observed in fresh external folder with project settings enabled | All seven skills advertised; loop and companion/template access, healthy early branch observed; not user-wide installation or every branch |
| Separate Codex model comparison | Case 06 executed with gpt-5.6-sol | Seven criteria observed on this one case; inline instructions, not native skill discovery or reliability evidence |
| Independent human review | Private packet prepared; not graded | No completed human review or independent pass claimed |
| Unseen holdouts and real use | Not performed | Authored cases and development repeats do not establish reliability or customer outcomes |

Raw prompts, responses, session metadata, and input hashes are retained locally; the public report includes selected evidence and response fingerprints. They are actual model runs, not an author's simulated walkthrough. The grading is still author-performed and the cases are synthetic. Record new evidence before changing any remaining unverified status.
