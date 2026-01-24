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
- [ ] Update GPT with V2 files
- [ ] Re-run test with sample charts
- [ ] Compare V2 output to aspirational
- [ ] Further iterate as needed
