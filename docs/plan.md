# Project Plan

## Objective

Develop **Market Look GPT** — a custom GPT that analyzes stock chart images and produces structured monthly market analysis reports for Jeff's Substack.

## Phases

### Phase 1: Foundation ✅
- [x] Define project structure
- [x] Gather sample charts (7 charts covering volatility, breadth, ratios)
- [x] Document tone and style requirements
- [x] Document output format requirements
- [x] Create chart interpretation reference guide
  - [x] SMA framework for all ratio charts
  - [x] VIX thresholds and patterns
  - [x] NAHL interpretation rules
- [x] Collect aspirational output example

### Phase 2: GPT Configuration ✅
- [x] Draft system instructions
- [x] Create conversation starters
- [x] Compile knowledge files for upload
- [x] Deploy V1 to OpenAI Custom GPT

### Phase 3: Testing & Iteration ✅
- [x] Test V1 with sample charts
- [x] Compare outputs to aspirational sample
- [x] Identify issues (chart interpretation, ordering, tone)
- [x] Refine instructions based on results (V2-V5)
- [x] Adjust chart interpretation rules as needed
- [x] Discover model requirement (thinking mode essential)
- [x] Validate with thinking model

### Phase 4: Deployment ✅
- [x] Finalize GPT configuration
- [x] Deploy Market Look GPT to OpenAI
- [x] Document usage guidelines

### Phase 5: Portfolio Look Capability ✅
- [x] Define portfolio analysis requirements
- [x] Design output format for portfolio reports (portlook-output-guide.md)
- [x] Create knowledge file for screenshot interpretation (screenshot-reference-guide.md)
- [x] Update instructions.md with Task 2 logic
- [x] Test with sample portfolio data (OptimHybrid, LessBold, Permanent Portfolio)
- [x] Iterate and refine (ETF attribution, positioning hierarchy, MTD preference)
- [ ] Deploy updated GPT to OpenAI
- [ ] Final validation with production use

### Phase 6: TAA Recommendation Assessment 🔜 (Next)
- [ ] Add optional input: TAA recommended changes (e.g., "Move 10% from VOO to BCI")
- [ ] Design output element assessing how proposed changes align with Market Look themes
- [ ] Update portlook-output-guide.md with new paragraph structure
- [ ] Update instructions.md with TAA input handling
- [ ] Test with sample TAA recommendations
- [ ] Iterate and refine

### Phase 7: Help/Usage Task 🔜
- [ ] Add Task 3: Help — triggered by "How do I use this?" or similar
- [ ] Define fixed output with:
  - Permalinks to chart image sources (StockCharts, TradingView, etc.)
  - Step-by-step instructions for Market Look
  - Step-by-step instructions for Portfolio Look
  - What inputs are required for each task
- [ ] Add to instructions.md (minimal thinking needed — mostly static output)

### Phase 8: Expanded Market Look Charts 🔜
- [ ] Add VOO:IAU ratio chart (stocks vs gold)
- [ ] Add VOO:BCI ratio chart (stocks vs commodities)
- [ ] Update chart-reference-guide.md with interpretation rules for new charts
- [ ] Update output-format-guide.md chart ordering
- [ ] Test with expanded chart set

### Phase 9: Flexible Chart Inputs 🔜
- [ ] Allow Market Look to work with subset of charts (not all 7 required)
- [ ] Update instructions.md to handle variable chart counts
- [ ] Test with partial chart sets (e.g., skip IAU if not relevant to portfolio)
- [ ] Ensure output adapts gracefully to available charts

## Model Requirement

⚠️ **Market Look GPT requires a thinking-enabled model.**

**Recommended:** ChatGPT 5.2 Thinking (tested and confirmed working)

Non-thinking models (ChatGPT 5.2 standard) fail at chart interpretation — they guess or assume rather than accurately reading visual data. Testing showed:
- Non-thinking (5.2): Missed crossovers, inverted MA relationships, wrong signal strength
- Thinking (5.1, 5.2): Accurate chart reading, correct crossover detection, proper signal mapping

## Success Criteria

- Output matches desired format (3 sections, correct structure)
- Tone is conversational, humble, non-prescriptive
- Technical language only in Detailed Chart Analysis
- Plain language accessible to non-investors in Executive Summary and What Should We Do?
- Signal strength ratings applied consistently
- Chart interpretations follow documented rules
- Posture guidance without trade recommendations

## Knowledge Files

| File | Purpose | Status |
|------|---------|--------|
| tone-and-style-guide.md | Voice, editorial rules, forbidden words | ✅ V7 (shared) |
| output-format-guide.md | Market Look report structure, plain-language rules | ✅ V7 |
| chart-reference-guide.md | Market chart interpretation rules (AUTHORITATIVE) | ✅ V2 |
| portlook-output-guide.md | Portfolio Look report structure | ✅ V1 |
| screenshot-reference-guide.md | Portfolio screenshot interpretation (AUTHORITATIVE) | ✅ V1 |

## GPT Configuration

| File | Purpose | Status |
|------|---------|--------|
| instructions.md | System instructions with task routing | ✅ V7 |
| conversation-starters.md | User prompts | ✅ V1 |
