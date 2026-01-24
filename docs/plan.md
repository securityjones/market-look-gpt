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

### Phase 3: Testing & Iteration 🔄 (In Progress)
- [x] Test V1 with sample charts
- [x] Compare outputs to aspirational sample
- [x] Identify issues (chart interpretation, ordering, tone)
- [x] Refine instructions based on results (V2)
- [x] Adjust chart interpretation rules as needed
- [ ] Test V2 with sample charts
- [ ] Iterate until output meets success criteria

### Phase 4: Deployment
- [ ] Finalize GPT configuration
- [ ] Deploy to OpenAI
- [ ] Document usage guidelines

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
| tone-and-style-guide.md | Voice, editorial rules | ✅ V2 (added observable vs analytical, Jeff's Mother test) |
| output-format-guide.md | Report structure | ✅ V2 (added chart ordering, good/bad examples) |
| chart-reference-guide.md | Interpretation rules | ✅ V2 (marked authoritative) |

## GPT Configuration

| File | Purpose | Status |
|------|---------|--------|
| instructions.md | System instructions with task routing | ✅ V2 |
| conversation-starters.md | User prompts | ✅ V1 |
