# Benchmark Results: youtube-video-formats

**Date:** 2026-06-01  
**Evals run:** 1, 2, 3  
**Runs per configuration:** 1

---

## Pass Rate Summary

| Configuration | Eval 1 | Eval 2 | Eval 3 | Mean |
|---|---|---|---|---|
| With skill    | 5/5 (1.00) | 5/5 (1.00) | 5/5 (1.00) | **1.00** |
| Without skill | 4/5 (0.80) | 3/5 (0.60) | 5/5 (1.00) | **0.80** |
| Delta         | +0.20 | +0.40 | 0.00 | **+0.20** |

---

## Per-Eval Results

### Eval 1: Extreme hot sauce stair-stepping format

**With skill (5/5 PASS):**
- Named the stair-stepping format explicitly
- Provided escalation table with Scoville ratings
- Critical Rule section: final sauce must be last, never tease it
- Entertainment ideas: guests, reaction challenges, heat indicators
- Detailed Finale/Payoff section with specific mechanics

**Without skill (4/5 PASS — 1 fail):**
- FAIL: Never used "stair-stepping" by name; described "progressive escalation" generically
- PASS: Escalation principle present
- PASS: Most extreme sauce saved for end
- PASS: Entertainment ideas (guests, timer challenge)
- PASS: Finale section with payoff structure

### Eval 2: Last-to-leave format fatigue diagnosis

**With skill (5/5 PASS):**
- Named format fatigue/saturation explicitly
- Stated the 2-3 format rotation rule precisely
- Provided rest option AND innovation twist options
- Articulated the viewer stated-preference paradox
- Multiple concrete innovation examples including combined format

**Without skill (3/5 PASS — 2 fails):**
- PASS: Format fatigue concept identified
- FAIL: Recommended calendar spacing (quarterly) not format-rotation rule
- PASS: Rest and twist options mentioned
- FAIL: Did not address the viewer stated-preference paradox
- PASS: Concrete setting changes and social mechanic ideas

### Eval 3: Chef kitchen swap format design

**With skill (5/5 PASS):**
- Open-loop question: "Who performs worse?" established in 60-second hook
- Explicit two parallel tracks converging at 70% mark
- Detailed blind taste test with multi-step reveal sequence
- Both tracks include explicit early failure beats
- Multiple warnings against revealing outcome early

**Without skill (5/5 PASS):**
- Open-loop competition question present
- Parallel tracks via cross-cutting mentioned (though organized day-by-day)
- Blind taste test payoff with external judges specified
- Both kitchens failing explicitly covered
- "Protect the ending" principle stated

**Note:** Eval 3 shows no pass-rate separation, but the without-skill response fell into the day-by-day vlog structure the skill explicitly warns against. The evals don't catch this difference.

---

## Key Findings

1. **Largest gap: Eval 2** — The skill's two most distinctive insights (format rotation rule and viewer paradox) are not naturally reproduced by a capable baseline model. This is where the skill provides unique value.

2. **Moderate gap: Eval 1** — The skill provides named format terminology and more precise structural mechanics. Baseline handles the general escalation principle well but lacks the specific framework.

3. **No gap: Eval 3** — The eval expectations are satisfiable by a good general response. The skill adds qualitative improvements (explicit parallel track framing, named format classification) that no assertion checks.

4. **Eval improvement opportunity:** Add an assertion to Eval 3 checking that the response explicitly warns against chronological day-by-day vlog structure.

---

## Overall Verdict

**With skill: 1.00 mean pass rate | Without skill: 0.80 mean pass rate | Delta: +0.20**

The skill improves performance, most significantly on format-specific rule application (rotation rules, format naming) and counterintuitive insights (viewer preference paradox). General open-loop and payoff design principles are already well-covered by baseline.
