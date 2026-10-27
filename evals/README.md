# Is it a zombie, or does it deserve to live?

Seven fictional scenarios exercise the Zombie-to-Exit Loop's judgment, arithmetic, branches, and human decision gates. They test zombies, useful incumbents, extension opportunities, incomplete replacements, and decisions made with unreliable records.

| Scenario | Situation or historical inspiration | What it tests |
|---|---|---|
| [The Last Envelope](cases/01-the-last-envelope.md) | A shrinking DVD-by-mail service with loyal holdouts | Full cost, missing Decider, exit obligations, unsupported replacement promises, and capacity versus cash |
| [The Second Exposure](cases/02-the-second-exposure.md) | Instant film's comeback | Current demand versus historical decline, “ugly is not dead,” and stopping before an unnecessary exit |
| [The Rugged Label](cases/03-the-rugged-label.md) | Fictional extension opportunity | Paid pilots, conditional orders, a capped qualification decision, and the revive branch |
| [The Missing Export](cases/04-the-missing-export.md) | Fictional incomplete replacement | Customer-job coverage, failed trials, conflicting dates, and gated migration |
| [The Next Big Bet](cases/05-the-next-big-bet.md) | Fictional allocation conflict | A profitable incumbent versus an unproven proposal; people capacity versus cash |
| [The Missing Ledger](cases/06-the-missing-ledger.md) | Fictional conflicting records | Incompatible revenue measures, overlapping roles, stale expenses, and pressure to bypass approval |
| [The Neighboring Vendor](cases/07-the-neighboring-vendor.md) | Fictional external-vendor transition | Mission mismatch, bundled economics, integration readiness, and a negotiated customer discount |

## Try one

In a fresh conversation with the skill files available, use:

```text
/eol-run-zombie-to-exit
Use evals/cases/01-the-last-envelope.md as a closed fictional fixture.
Use Best guess mode and only the evidence in that file. Do not browse.
Run the lifecycle map and Cost Ledger unless a branch stops the loop first.
Preserve the human gates. Give the required artifacts and a readout
of no more than 200 words. Do not read expected results or other cases.
```

For the non-zombie case, replace the filename with `evals/cases/02-the-second-exposure.md`. In another assistant, supply the loop instructions, its template, the six companion skill instructions and templates, and one case file. The external announcement skill is optional; the loop documents its fallback.

## Evaluate rather than rehearse the answer

For a blinded behavioral run, create a separate temporary folder containing only the seven skill folders' `SKILL.md` and `template.md` files, plus one case file. Exclude skill examples, evaluator criteria, this guide, prior responses, and every other scenario. Start a fresh assistant in that folder; do not give it access to the original Project. Follow the selected skill's human gates.

The evaluator keeps [original expected results and facilitator turns](criteria/expected-results.md), [expanded criteria and turns](criteria/expanded-expected-results.md), and [vendor-transition criteria and turn](criteria/vendor-expected-results.md) separately. Case 01 has two phases: the initial response must stop at the missing Decider; only then may a human provide its scripted fictional reply to continue. Case 02 should stop early without planning an exit. These are deliberately different paths, not a demonstration that must run every step.

For a teaching demo, the facilitator may read the criteria in advance. Label that as a rehearsal, not a blinded evaluation.

## Save and grade an actual run

Keep the transcript, model/version, date, mode, supplied files, tool use, human replies, individual artifacts, short readout, and criterion-by-criterion grades. Cite response passages for each grade. Keep new run records private until separately reviewed for publication. Do not call a fixture or an unexecuted criterion passed.

Current limits are in [Verification](VERIFICATION.md). These scenarios are teaching and evaluation material, not evidence of real customer outcomes.

The [October 27 behavioral report](reports/2026-10-27-loop-evaluation.md) records baseline failures, targeted skill corrections, and the final acceptance responses. It does not turn these authored examples into unseen holdout tests.

The [expanded evaluation report](reports/2026-10-27-expanded-evaluation.md) records four additional cases, failed criteria, targeted repeats, a three-turn Guided check, native Claude discovery, and a separate Codex comparison. Some criteria remain failing; independent human review has not occurred.

## Historical anchors and fiction boundary

Netflix announced the end of its shrinking DVD business and final shipments on September 29, 2023. [Netflix's own announcement](https://about.netflix.com/en/news/netflix-dvd-the-final-season).

Polaroid describes ending instant-film production in 2008, enthusiasts saving the last factory through the Impossible Project, and the brand's subsequent return. [Polaroid's own history](https://press.polaroid.com/about/).

Sources checked October 27, 2026. These anchors supply the situation, not the verdict. They do not establish that either real business was a zombie, quantify its economics, or reveal its internal decision process. Night Owl Disc Club and Second Exposure are invented products. Every figure, evidence record, owner, obligation, date, and approval in the cases is fictional; none should be attributed to Netflix or Polaroid. No private historical notes or source presentations are included.

Cases 03–06 are wholly fictional stress scenarios. They are not factual accounts of named historical businesses.

Case 07 adapts a practitioner-described pattern into wholly fictional evidence: retire a line outside the mission, and coordinate a transition and discount with another vendor. Its invented terms and integration results do not describe an actual agreement.

The [vendor-transition evaluation](reports/2026-10-27-vendor-transition.md) records the two-phase commercial bridge test, observed gaps and targeted instruction changes.
