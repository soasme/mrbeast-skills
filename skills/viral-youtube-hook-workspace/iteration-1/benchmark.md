# Benchmark Report: viral-youtube-hook
**Date:** 2026-06-01  
**Evals run:** 1, 2, 3  
**Runs per configuration:** 1

---

## Summary Table

| Eval | Description | with_skill | without_skill | Delta |
|------|-------------|-----------|---------------|-------|
| 1 | Write first 60 seconds for underground survival video | 5/5 (100%) | 2/5 (40%) | +60% |
| 2 | Critique a retention-killing video opening | 5/5 (100%) | 4/5 (80%) | +20% |
| 3 | Plan hook-to-minutes-1-3 transition with crazy progression | 5/5 (100%) | 2/5 (40%) | +60% |
| **Mean** | | **100%** | **53.3%** | **+46.7%** |

---

## Per-Eval Breakdown

### Eval 1 — Write First 60 Seconds (Underground Survival)

**with_skill: 5/5 PASS**
- Opened mid-action inside the chamber (thumbnail confirmed in ~2 seconds)
- Zero filler warmup — first line: "I'm already underground"
- Stakes locked by second 55 (rules, hours, water supply, check-in protocol)
- Rich visual direction throughout (camera angles, dramatic lighting, clock graphic)
- Transition Signal section explicitly described (time-lapse, emotional re-engagement)

**without_skill: 2/5 PASS**
- FAILED: Opened outside the chamber ("standing next to a freshly dug hole") — thumbnail not confirmed
- FAILED: Used filler warmup ("Hey guys! What is up, today's video is absolutely insane")
- PASSED: Stakes were mentioned (100 hours, no leaving early)
- PASSED: Some visual instructions present (ladder, chamber from above)
- FAILED: No transition to execution phase described — plan ends at "countdown starts"

---

### Eval 2 — Critique a Retention-Killing Opening

**with_skill: 5/5 PASS**
- Identified all 5 retention problems with named principles from SKILL.md
- Flagged visual non-confirmation (ball pit never shown) as distinct from verbal delay
- Included a full scripted rewrite with dialogue, visual directions, and timing
- Summary table with mistake, timing, and retention impact rating

**without_skill: 4/5 PASS**
- Identified 4/5 problems correctly (warmup, subscribe ask, sponsor, filler)
- FAILED: Treated the ball pit absence as a verbal timing issue ("doesn't come until 25–30 seconds in verbally") rather than a thumbnail visual confirmation failure
- Recommendations were bullet-point suggestions, not a scripted rewrite

---

### Eval 3 — Hook-to-Minutes-1-3 Transition (Slip N Slide)

**with_skill: 5/5 PASS**
- Thumbnail confirmed within 8 seconds (drone shot of full 500-foot slide)
- Crazy progression applied: 3 rounds compressed in first 90 seconds, speed escalation, obstacle reveal
- Three named emotional anchor characters introduced by minute 2:30
- Concrete re-engagement spectacle at minute 3 (obstacle barrier reveal)
- Execution begins before 1-minute mark (first contestant launches at ~50 seconds)

**without_skill: 2/5 PASS**
- PASSED: Drone shot of full slide mentioned in opening
- FAILED: Crazy progression not applied — plan uses "briefly introduce", "establish rules" framing; ends minute 3 on "conditions are explained"
- PASSED: Emotional investment addressed (characters to root for)
- FAILED: Re-engagement spectacle is vague ("maybe obstacles, maybe faster, maybe slippery")
- FAILED: Plan avoids execution — ends on setup/explanation framing rather than action

---

## Key Findings

**The skill creates the largest improvement on tasks that require proactive structure** — specifically: starting mid-action (not setup), the four-beat output format (Opening Beat / Hook Sequence / Premise Lock / Transition Signal), and the "crazy progression" concept for minutes 1–3. These are not intuitions a general-knowledge baseline applies consistently.

**The skill creates the smallest improvement on critique tasks** (Eval 2, +20%) because identifying obvious retention mistakes (warmup, sponsor, subscribe ask) is partially accessible from general YouTube knowledge. However, the skill adds meaningful quality by providing a scripted rewrite and correctly diagnosing the visual confirmation failure vs. a verbal timing issue.

**The most discriminating single assertion across all evals** was Eval 1 Expectation 1: the baseline opened the video OUTSIDE the chamber, not inside it — a direct contradiction of the thumbnail-matching principle that is the skill's core teaching.

**Output depth:** with_skill responses averaged ~4,390 characters vs ~1,716 characters for baseline (2.5x more detailed). This gap is not captured by pass/fail scores but represents meaningful quality improvement.

---

## Recommendations for Eval Improvement

1. **Eval 1:** Add an assertion for the SKILL.md four-beat format (Opening Beat, Hook Sequence, Premise Lock, Transition Signal) — this is the skill's primary structural output and nothing currently checks for it.
2. **Eval 2:** Add an assertion verifying the rewrite itself avoids the same mistakes it critiques (e.g., "the rewrite does not contain a warmup greeting or subscribe ask").
3. **Eval 3:** Make the re-engagement spectacle assertion more precise — require the spectacle to visually change the nature of the challenge, not just vaguely raise stakes.
