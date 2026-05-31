# Brand Deal Integration Skill — Benchmark Results
## Iteration 1

**Date:** 2026-06-01
**Evals run:** 3 (IDs: 1, 2, 3)
**Expectations per eval:** 6

---

## Pass Rate Summary

| Configuration | Eval 1 | Eval 2 | Eval 3 | Mean |
|---|---|---|---|---|
| With Skill | 6/6 (100%) | 6/6 (100%) | 6/6 (100%) | **100%** |
| Without Skill | 3/6 (50%) | 3/6 (50%) | 3/6 (50%) | **50%** |
| **Delta** | +50% | +50% | +50% | **+50%** |

---

## What the Skill Fixes

**Placement precision** — The baseline offered "minutes 2–3" as a valid placement option in eval 3. The skill-guided response strictly enforced the 6+ minute rule with explicit reasoning (viewer investment, retention graph behavior).

**Script craft** — The baseline reliably removed the forbidden "brought to you by" opener but then fell back into marketing-copy patterns: feature lists, stat-quoting without context, scripted-sounding delivery. The skill-guided responses wrote genuinely conversational delivery with first-person uncertainty and story-tied context.

**Visual integration** — The baseline mentioned visuals in tips sections but did not script them into the delivery. The skill-guided responses scripted visual stage directions directly into the segment (packet opening, phone screen, contestant reactions).

**Runtime targeting** — The baseline never stated a runtime target. The skill-guided responses explicitly recommended 45-second segments within the 60-second ceiling.

---

## Consistent Baseline Failures (appeared in all 3 evals)

1. Placement too early (or early option offered as equal alternative)
2. Scripted tone despite conversational intent
3. Missing runtime recommendation
4. Visual bit mentioned but not scripted into delivery

---

## Eval Quality Notes

- Eval 1 & 3 assertions are tight and discriminating — they correctly failed the baseline on placement and craft.
- Eval 2 has one potentially weak assertion ("clearly more entertaining") — subjective and hard to fail even for mediocre rewrites.
- No assertion across all 3 evals checks for the forbidden "This video is brought to you by" opener in the *written script* (as opposed to testing the rewrite task in eval 2). Eval 1 and 3 scripts could technically open with it and still pass.

---

## Conclusion

The skill delivers a **+50 percentage point improvement** over the baseline across all three evals. The gains are consistent and attributable to specific, verifiable behaviors the skill encodes: placement rules, anti-patterns, and scripting conventions that general-purpose models do not apply by default.
