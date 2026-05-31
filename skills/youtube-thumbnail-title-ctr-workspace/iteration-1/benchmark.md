# Benchmark Summary — youtube-thumbnail-title-ctr
**Date:** 2026-06-01
**Evals run:** 1, 2, 3
**Runs per configuration:** 1

## Pass Rates

| Configuration | Eval 1 | Eval 2 | Eval 3 | Mean |
|---|---|---|---|---|
| with_skill | 5/5 (1.0) | 5/5 (1.0) | 5/5 (1.0) | **1.0** |
| without_skill | 5/5 (1.0) | 5/5 (1.0) | 5/5 (1.0) | **1.0** |
| Delta | 0.0 | 0.0 | 0.0 | **+0.0** |

## Key Findings

Both configurations achieved perfect pass rates (15/15 expectations). The skill does not show a measurable lift on these evals using the current expectation set.

**Qualitative differences (not captured by current evals):**
- with_skill responses used explicit framework terminology from the SKILL.md (extremity rule, open loop principle, thumbnail/title contract, production implications checklist)
- with_skill responses were more structured and complete, averaging ~3,670 chars vs ~2,630 chars for without_skill
- with_skill responses more explicitly grounded reasoning in named principles, while without_skill relied on general YouTube knowledge

## Eval Quality Note

The current expectations test high-level CTR concepts that a capable baseline model can satisfy without skill guidance. To make evals more discriminating, consider adding assertions for:
- Production implications mentioned in the response
- Use of skill-specific framework names (open loop, extremity rule, thumbnail contract)
- CTR self-test checklist applied
- Flagging which title is most accurate to content (skill-specific requirement)
