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

---

## January 25, 2026

### Session 1 — Portfolio Look Design & Implementation

**Context gathered:**
- User provided sample portfolio screenshots in samples/portcharts/:
  - benchmark-012426.png (60/40 benchmark)
  - optimhybrid-012426.png (OptimHybrid portfolio)
  - lessbold-012426.png (LessBold portfolio)
- User provided developmental prototype in samples/outputs/port-look-developing.md
- Prototype includes working starter prompt and aspirational output

**Key design decisions:**

1. **Workflow:** Portfolio Look is a companion piece to Market Look
   - Market Look → publish as Substack Article #1
   - Portfolio Look uses published Market Look text as input → publish as Article #2
   - References to Market Look should read like cross-references between articles

2. **Knowledge file architecture:** Parallel to Market Look
   - tone-and-style-guide.md — Shared
   - portlook-output-guide.md — New (output structure)
   - screenshot-reference-guide.md — New (screenshot interpretation, AUTHORITATIVE)

3. **Output structure:** Opening + 2 paragraphs
   - Opening framing sentence referencing Market Look
   - Paragraph 1: Performance summary (MTD comparison, 12-month visual narrative)
   - Paragraph 2: Positioning & Market Look connection

4. **ETF lookup requirement:** Must look up what ETFs actually hold, not trust screenshot labels

**Files created:**

- ✅ docs/design/portfolio-look-design.md — Design document
- ✅ knowledge/reference/portlook-output-guide.md — Output format guide (V1)
- ✅ knowledge/reference/screenshot-reference-guide.md — Screenshot interpretation guide (V1)

**Files updated:**

- ✅ gpt-config/instructions.md — Added Task 2 logic, expanded knowledge file references
- ✅ docs/plan.md — Updated Phase 5 status and knowledge file table

**Next steps:**
- [ ] Test with OptimHybrid + benchmark screenshots
- [ ] Test with LessBold + benchmark screenshots
- [ ] Iterate based on output quality
- [ ] Deploy updated GPT to OpenAI

---

### Session 1 (continued) — Testing & Iteration

**Testing completed:**

Tested Portfolio Look with three portfolios:
1. **OptimHybrid** — Stock-heavy, international-tilted, aligns with Market Look themes
2. **LessBold** — Balanced, developed-international heavy
3. **Harry Browne's Permanent Portfolio** — Defensive 25/25/25/25 split, conflicts with Market Look themes

**Issues identified and fixed:**

| Issue | Fix |
|-------|-----|
| Task triggers too literal ("Generate my portfolio update" only) | Made triggers flexible — accepts variations like "port look," "how did my portfolio do" |
| IEFA not treated as part of international allocation | Added explicit note that IEFA/VEA/EFA count toward international |
| Positioning categories didn't map to Market Look themes | Restructured to: Stocks vs Safety → U.S. vs International → Developed vs EM → Small vs Large |
| Couldn't tell which holdings drove gains/losses | Added new Paragraph 2 for ETF attribution (look up individual ETF MTD) |
| ETF lookup vs categorization confusing | Clarified: look up what ETF holds first, then use categorization table |
| Missing common ETFs in reference | Added: QQQM, VGLT, IAU, PDBC, BCI, SCHH, EWJ, EWS, EWZ |
| YTD vs MTD inconsistency | Added note to prefer MTD terminology for consistency |

**Output structure finalized:**

1. **Opening** — References Market Look as published article
2. **Paragraph 1** — Performance summary (MTD comparison, 12-month chart narrative)
3. **Paragraph 2** — ETF attribution (which holdings drove gains/losses)
4. **Paragraph 3** — Positioning & Market Look connection (stocks vs safety, U.S. vs intl, alignment/conflicts)

**Key design decisions:**

- Portfolio Look is a **companion piece** to Market Look (readers may have read both)
- Market Look should be referenced as a published article, not "the analysis above"
- Benchmark screenshot may be optional — GPT can look up VBINX or calculate SPY/IEF weighted average
- ETF MTD lookup is required for attribution paragraph

**Files updated during iteration:**

- instructions.md — Flexible triggers, added ETF MTD lookup step, updated validation checklist
- portlook-output-guide.md — Added Paragraph 2 (ETF attribution), MTD preference
- screenshot-reference-guide.md — Positioning hierarchy, ETF lookup clarification, expanded ETF examples

**Test output quality:** Good. All three portfolios produced usable outputs with correct:
- MTD comparison and delta calculation
- 12-month chart narrative
- ETF attribution explaining gains/losses
- Market Look theme alignment/conflict analysis

**Current status:**
- ✅ Portfolio Look design complete
- ✅ Knowledge files created and refined
- ✅ Instructions updated
- ✅ Testing passed (3 portfolios)
- ⏳ Ready for deployment to OpenAI

---

## January 26, 2026

### Session 1 — Phase 8: Expanded Market Look Charts ✅

**Objective:** Add VOO:IAU (stocks vs gold) and VOO:BCI (stocks vs commodities) to Market Look capability.

**Chart hierarchy redesign:**

Reorganized chart ordering into a logical 3-tier hierarchy:

| Tier | Purpose | Charts |
|------|---------|--------|
| Tier 1 — Macro Conditions | Overall market stress/health | VIX, NAHL |
| Tier 2 — Big Allocation Questions | Stocks vs safety, US vs intl | VOO:IEF, VOO:IAU, VOO:BCI (group), VOO:VEA, VOO:VWO (group) |
| Tier 3 — Drilling Down | Within-category comparisons | VOO:IJR, VOO:QQQ (within US) |

**Chart changes:**
- Added VOO:IAU (stocks vs gold)
- Added VOO:BCI (stocks vs commodities)
- Swapped VEA:VWO → VOO:VWO (direct US vs EM comparison, cleaner story)
- Swapped IJR:VOO → VOO:IJR (consistent VOO: prefix, inverted interpretation)
- Swapped QQQ:RSP → VOO:QQQ (consistent VOO: prefix, inverted interpretation)

**Final chart lineup (9 charts):**
1. $VIX — Volatility Index
2. $NAHL — New Highs vs New Lows
3. VOO:IEF — Stocks vs Bonds
4. VOO:IAU — Stocks vs Gold
5. VOO:BCI — Stocks vs Commodities
6. VOO:VEA — US vs International Developed
7. VOO:VWO — US vs Emerging Markets
8. VOO:IJR — Large vs Small Cap
9. VOO:QQQ — Broad Market vs Tech-Heavy

**Paragraph 3 improvements (multiple iterations):**
- Issue: GPT was writing checklist-style with parenthetical translations
- Fix: Added explicit "observation vs interpretation" guidance
- Fix: Added full aspirational example showing narrative style
- Fix: Changed "technical language allowed" to "permitted but not required"
- Fix: Added "DO NOT write like this" example showing the bad pattern
- Result: GPT now writes flowing narrative interpretation, not data dumps

**NAHL communication fix:**
- Issue: GPT was describing indicator ("more highs than lows")
- Fix: NAHL is a decision signal — communicate what it tells you to DO
- New guidance: "above +50 = confirms we should be confidently invested in stocks"

**Optional "lesson of the month" closer:**
- Added option to end Paragraph 3 with investing principle the data illustrates
- Backward-looking reflection, not forward action guidance
- Only when earned from the data

**Chart permalinks added:**
- Each chart in Detailed Chart Analysis now starts with `[Link to chart](permalink)`
- All 9 StockCharts permalinks documented in output-format-guide.md

**Files updated:**
- output-format-guide.md → V8 (major revisions)
- chart-reference-guide.md → V8 (new charts, updated examples)

**Test output saved:**
- samples/outputs/market-look-v8-test.md

**Legacy cleanup:**
- Removed all references to old chart names (IJR:VOO, QQQ:RSP, VEA:VWO)
- Updated examples throughout both knowledge files

**Status:** Phase 8 complete. Ready for deployment when ChatGPT upload limits reset.

---

## January 27-28, 2026

### Session — Phase 9: Flexible Chart Inputs & Ratio/NAHL Guidance Overhaul

**Flexible chart requirements implemented:**
- 3 minimum required charts: NAHL, VOO:IEF, VOO:VEA
- 6 optional charts: VIX, VOO:IAU, VOO:BCI, VOO:VWO, VOO:IJR, VOO:QQQ
- GPT stops and requests missing required charts; generates complete report with partial optional set
- Input formats: individual images (PNG/JPG) or multi-page PDF (ZIP not supported)

**Ratio Chart Fundamentals section added to chart-reference-guide.md:**
- Clear terminology: numerator, denominator, "ratio" not "price"
- 5-step observation checklist with MA crossover timing guidance (4-5 bars = this month, 12-13 bars = established)
- "Do Not Invert" rule with explicit table showing winner when ratio falls
- Common error example (VOO:IJR inversion)

**NAHL guidance overhauled:**
- Explicit: "This is a breadth indicator, NOT a ratio chart"
- Two elements, one signal: 13-day EMA only; ignore dotted daily line unless emergency (-500)
- Recency rules: don't call old readings "recent"; threshold crossings reset narrative anchor
- Do NOT say: "eased from recent highs," "cooled from higher readings" (unless actually recent)
- CAN reference older readings with accurate time labels: "hasn't reached the high signals from late last year"

**Output format updates:**
- Chart link now comes after header, not before
- "Ratio" terminology throughout
- Reference to chart-reference-guide for interpretation rules

**Testing:**
- V9: 4-chart and 9-chart tests (identified NAHL and ratio inversion issues)
- V10: 4-chart and 9-chart tests (NAHL and ratio interpretation correct)

**Test outputs saved:**
- samples/outputs/market-look-v9-4chart-test.md
- samples/outputs/market-look-v9-allcharts-test.md
- samples/outputs/market-look-v10-4chart-test.md
- samples/outputs/market-look-v10-allcharts-test.md

**Files updated:**
- instructions.md → flexible chart requirements, input format changes
- chart-reference-guide.md → Ratio Chart Fundamentals, NAHL overhaul, terminology fixes
- output-format-guide.md → chart link position, ratio terminology
- plan.md → Phase 9 complete
- README.md → Phase 9 complete

**Status:** Phase 9 complete. V10 is stable and ready for production use.
