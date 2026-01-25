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

### Phase 5: Portfolio Analysis Capability 🔜 (Next)
- [ ] Define portfolio analysis requirements
- [ ] Design output format for portfolio reports
- [ ] Create knowledge file for portfolio interpretation
- [ ] Update instructions.md with Task 2 logic
- [ ] Test with sample portfolio data
- [ ] Iterate and refine

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
| tone-and-style-guide.md | Voice, editorial rules, forbidden words | ✅ V7 |
| output-format-guide.md | Report structure, plain-language rules | ✅ V7 |
| chart-reference-guide.md | Interpretation rules (AUTHORITATIVE) | ✅ V2 |

## GPT Configuration

| File | Purpose | Status |
|------|---------|--------|
| instructions.md | System instructions with task routing | ✅ V7 |
| conversation-starters.md | User prompts | ✅ V1 |
