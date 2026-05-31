# Benchmark Results: viral-content-ideation

**Skill:** viral-content-ideation
**Date:** 2026-06-01
**Evals:** 3
**Runs per configuration:** 1

---

## Pass Rate Comparison

| Configuration | Eval 1 | Eval 2 | Eval 3 | Mean |
|---|---|---|---|---|
| With skill | 6/6 (100%) | 6/6 (100%) | 6/6 (100%) | **100.0%** |
| Without skill | 1/6 (16.7%) | 2/6 (33.3%) | 4/6 (66.7%) | **38.9%** |
| **Delta** | +83.3% | +66.7% | +33.3% | **+61.1%** |

---

## Eval Summaries

### Eval 1: Rubber Duck Brainstorm (5 Concepts)
The largest performance gap. The skill's 3-angle expansion framework (competition/scale/constraint) and specific wow-factor requirements produce structurally distinct, high-quality concepts. The baseline generates generic stunt ideas without distinct angles, non-specific wow moments, and undifferentiated CTR scores.

### Eval 2: Creativity Saves Money — $5k Coding Video
Significant gap. The skill prompts a premise reframe (educational tutorial → Kids vs. Engineers competition) and explicitly applies the creativity-saves-money principle. The baseline provides budget-cutting logistics without changing the underlying concept, resulting in a cheaper but not more interesting video.

### Eval 3: 5-Dimension Rubric Evaluation
Smallest gap. The structured scoring format is partially inferrable without the skill. The baseline scores both ideas on all dimensions and makes a clear recommendation. Where it falls short: fails to identify the thumbnail problem as Idea A's structural flaw, and offers vague rather than specific improvement suggestions.

---

## Key Findings

1. **The framework provides the most value in generative tasks.** When asked to brainstorm, the skill's 3-angle expansion framework produces outputs that baseline cannot match — the difference between "ideas that come to mind" and "ideas systematically generated across fundamentally different angles."

2. **Naming principles matters.** Eval 2 fails for the baseline partly because it never names or invokes "creativity saves money" as the guiding principle. The skill makes this explicit, changing the problem frame from "how do I spend less?" to "what's the more interesting version?"

3. **Rubric scoring is more portable than generative frameworks.** Any LLM can apply a 5-dimension scoring rubric to sufficient depth — the skill's value in eval 3 comes from the depth of analysis (identifying the thumbnail as a structural flaw, setting the 20/25 production threshold) rather than the structure itself.

4. **Eval quality note:** Some expectations could be tightened. "Suggests improvements for the weaker idea" passes for vague advice in the baseline. Consider requiring 2+ concrete title/format/stakes changes to better discriminate. Similarly, "passes the 6-word simplicity test" needs clarification on whether the title itself or the underlying premise must fit 6 words.

---

## Conclusion

The skill improves pass rates by **+61.1 percentage points** (from 38.9% to 100.0%). The improvement is largest in open-ended brainstorming tasks where the framework provides structure, and smallest in evaluation tasks where scoring rubrics are partially self-evident. The skill delivers clear, consistent value across all three eval types.
