# Progress Log

## January 24, 2026

### Session 1 — Foundation Complete

**Project Setup:**
- ✅ Created project folder structure
- ✅ Initialized documentation (plan.md, progress.md)
- ✅ Created .gitignore

**Knowledge Files Created:**
- ✅ tone-and-style-guide.md — Voice, tone, editorial rules
  - Conversational "we" framing
  - Plain language requirement (no jargon in Exec Summary / What Should We Do)
  - Non-prescriptive posture guidance
  - End with humility, not closure

- ✅ output-format-guide.md — Report structure
  - 3 sections: Executive Summary, What Should We Do?, Detailed Chart Analysis
  - Executive Summary = exactly 3 paragraphs
  - Signal strength ratings (Weak/Moderate/Strong) in chart analysis
  - No "Bottom Line" or "What to Watch" sections

- ✅ chart-reference-guide.md — Interpretation rules
  - SMA Framework for all ratio charts (crossovers, price position, slope, signal freshness)
  - VIX thresholds and trend patterns
  - NAHL interpretation with +50/0/-50 levels
  - Posture language templates

**Sample Files:**
- ✅ 7 chart PNGs added to samples/charts/
- ✅ market-look-aspirational.md created from original docx

**Decisions Made:**
- GPT name: "Market Look GPT"
- Dynamic chart coverage (analyze all charts provided)
- Technical language OK in Detailed Chart Analysis only
- Signal strength ratings included per chart

**Next Steps:**
- [x] Delete original .docx files (now converted to .md)
- [x] Initialize git repo
- [x] Stage and push to GitHub
- [x] Begin Phase 2: Draft GPT system instructions

---

### Session 2 — V1 Testing & Revisions

**GPT Configuration Created:**
- ✅ instructions.md — System instructions with task routing
- ✅ conversation-starters.md — Two starters (Market Look, Portfolio placeholder)

**V1 Deployed to OpenAI Custom GPT:**
- Uploaded 3 knowledge files
- Configured instructions and conversation starters
- Tested with 7 sample charts

**V1 Output Review — Issues Identified:**

| Issue | Section Affected |
|-------|------------------|
| Output wrapped in markdown code block | Output format |
| Chart order incorrect | Detailed Chart Analysis |
| Ended with summary paragraph | Detailed Chart Analysis |
| Para 3 didn't walk through each chart | Executive Summary |
| "What Should We Do" too generic | What Should We Do |
| Abstraction ban violations | Throughout |
| Analytical language instead of observable | Para 1, Para 2 |
| Missed IJR:VOO golden cross | Chart interpretation |
| Missed NAHL +50 threshold (called Moderate, should be Strong) | Chart interpretation |
| Missed VOO:VEA death cross (called "in transition") | Chart interpretation |
| Wrong signal strength ratings | Multiple charts |

**V2 Revisions Applied:**

*output-format-guide.md:*
- Added explicit chart ordering (VIX → VOO:IEF → NAHL → IJR:VOO → QQQ:RSP → VOO:VEA → VEA:VWO)
- Para 3 now requires chart-by-chart walkthrough in order
- Para 2 must ground context in chart evidence, not abstract "mood"
- "What Should We Do" must link each suggestion to specific chart signal
- Added good/bad examples for "What Should We Do"
- Added "Do not end with summary paragraph" rule

*tone-and-style-guide.md:*
- Added "Jeff's Mother" test
- Added "Observable vs Analytical" comparison table with examples
- Clarified abstraction ban with more examples

*instructions.md:*
- Marked chart-reference-guide as AUTHORITATIVE
- Added explicit override: our guide > generic TA knowledge
- Added MUST-do checklist for ratio charts (price position, MA crossovers, signal freshness)
- Added anti-weasel clause: don't say "in transition" if signal is clear
- Added explicit NAHL threshold reminder (+50 = Strong)
- Fixed output format to prohibit code blocks/backticks

**Next Steps:**
- [x] Update GPT with V2 files
- [x] Re-run test with sample charts
- [x] Iterate through V3, V4, V5

---

### Session 2 (continued) — V2-V5 Testing & Model Discovery

**V2-V4 Testing (ChatGPT 5.2 / non-thinking model):**

Despite progressive refinements to instructions and knowledge files, the non-thinking model consistently failed at chart interpretation:

| Chart | Actual Signal | 5.2 Output |
|-------|---------------|---------------|
| IJR:VOO | Price above both MAs, golden cross | "Below both MAs, no change" |
| VOO:VEA | Price below both MAs, death cross | "U.S. still ahead" |
| NAHL | 13 EMA at +63, above +50 | "Above zero, Moderate" (should be Strong) |

**V3 Revisions:**
- Added requirement to state observable values before interpreting
- Added "compare current to one month ago" step
- Fixed QQQ:RSP language (no "concentrated")
- Strengthened crossover = regime change rule

**V4 Revisions:**
- Clarified Executive Summary paragraph purposes (non-overlapping)
- "What Should We Do?" now requires ONE paragraph
- Added signal-to-posture mapping for all chart types
- Ratio values deemed meaningless — only MA relationships matter
- NAHL: focus on 13-day EMA only

**V5 Revisions:**
- Compressed instructions.md to under 8,000 characters
- Moved detailed chart rules to chart-reference-guide.md (single source of truth)
- Instructions now point to knowledge files rather than duplicating rules

**Key Discovery: Thinking Model Required**

Tested with ChatGPT 5.2 (non-thinking) vs 5.1 Thinking:

| Aspect | Non-Thinking (5.2) | Thinking (5.1) |
|--------|--------------|----------|
| Chart reading accuracy | ❌ Frequently wrong | ✅ Correct |
| Crossover detection | ❌ Missed | ✅ Identified |
| MA relationship | ❌ Often inverted | ✅ Accurate |
| Signal strength | ❌ Inconsistent | ✅ Matched our criteria |
| Following knowledge files | ⚠️ Partial | ✅ Rigorous |

**Root cause:** Non-thinking models appear to guess or rely on assumptions rather than actually reading the chart images. Thinking models reason step-by-step and accurately observe visual data.

**V6 — ChatGPT 5.2 Thinking Test (Final)**

Tested with ChatGPT 5.2 Thinking model:
- ✅ Chart reading accurate across all 7 charts
- ✅ Executive Summary structure correct (3 paragraphs, non-overlapping purposes)
- ✅ "What Should We Do?" = one paragraph, linked to chart evidence
- ✅ Detailed Chart Analysis follows correct order
- ✅ Signal strength ratings appropriate
- ✅ Knowledge file compliance throughout

**Decision:** Deploy with ChatGPT 5.2 Thinking as the standard model.

**V7 Revisions — Plain Language Polish**

After V6 testing, identified that Exec Summary Para 1/2 and "What Should We Do?" still had technical language leakage (ticker symbols, MA jargon).

*output-format-guide.md:*
- Added explicit plain-language rules for Para 1 (no tickers, no MA language, use "stocks" not "equities")
- Added accuracy requirement for Para 2 (must match chart evidence, not fabricate context)
- Added explicit note that Para 3 DOES allow technical language
- Added plain-language rules for "What Should We Do?" (no tickers, no MA jargon, must pass Jeff's Mother test)
- Added translation examples for common technical phrases

*tone-and-style-guide.md:*
- Added "equities" to forbidden words list (use "stocks" instead)

**V7 Test Output:**
- Tested with ChatGPT 5.2 Thinking
- Para 1 and 2 now plain language ✅
- Para 3 retains technical detail ✅
- "What Should We Do?" plain language ✅
- Saved to samples/outputs/market-look-v7-test.md

**Current Status:**
- ✅ All knowledge files finalized (V7)
- ✅ Instructions finalized
- ✅ Model requirement documented (5.2 Thinking)
- ✅ V7 test output saved
- ✅ Market Look GPT deployed

**Next Phase: Portfolio Analysis**
- Task 2 currently returns placeholder: "Future portfolio analysis tbd."
- Goal: Generate monthly portfolio reports comparing user's portfolio to benchmarks
- Will require new knowledge files and output format design
