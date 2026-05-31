# Benchmark: youtube-production-mindset
**Date:** 2026-06-01 | **Evals:** 3 | **Runs per config:** 1

## Pass Rate Summary

| Configuration | Eval 1 | Eval 2 | Eval 3 | Mean |
|---|---|---|---|---|
| with_skill | 7/7 (100%) | 7/7 (100%) | 6/6 (100%) | **100%** |
| without_skill | 3/7 (43%) | 3/7 (43%) | 3/6 (50%) | **45.2%** |
| **Delta** | +57% | +57% | +50% | **+54.8pp** |

## What the Skill Adds

The baseline model produces sound generic production advice and correctly identifies the main critical components. Where it consistently fails is in the *specific, opinionated mechanics* the skill encodes:

| Expectation | With Skill | Without Skill |
|---|---|---|
| Daily check-ins (not every 2-3 days) | PASS | FAIL |
| "Dump-and-forget" pattern named explicitly | PASS | FAIL |
| Video updates over photos for contractors | PASS | PASS (weakly) |
| Backup day negotiated into same contract | PASS | FAIL |
| Standard shipping warning for critical props | PASS | FAIL |
| "Can this failure become content?" principle | PASS | FAIL |
| Producer — not contractor — owns outcome | PASS | FAIL |
| Ask why there was no backup plan | PASS | FAIL |
| Do not skip scene without exhausting alternatives | PASS | FAIL |

## Eval Improvement Suggestions

- **Eval 2, "dump-and-forget":** Assertion checks naming rather than mechanism. Consider requiring the response to explain *why* dump-and-forget fails (no visibility into problems), not just use the phrase.
- **Eval 3:** No assertion checks whether the response recommends capturing the failure on camera immediately (a key skill behavior). Consider adding this.
- **Eval 1, daily check-ins:** The phrase "or equivalent tracking" weakens the assertion. Tighten to require daily cadence explicitly.

## Conclusion

The skill demonstrates strong, consistent lift (+54.8pp). Every with_skill run was perfect. The improvements are concentrated in behavioral specifics rather than conceptual coverage — exactly what a production mindset skill should add.
