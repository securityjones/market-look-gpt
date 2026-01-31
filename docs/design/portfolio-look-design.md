# Portfolio Look — Design Document

## Overview

Portfolio Look is the second capability for Market Look GPT. It produces monthly portfolio update reports that complement the Market Look reports.

## Workflow Context

The two capabilities are used sequentially to produce two related Substack articles:

```
┌─────────────────────────────────────────────────────────────────┐
│  Step 1: Market Look                                            │
│  ────────────────────                                           │
│  Input:  9 market charts                                        │
│  Output: Market Look report                                     │
│  Action: Publish as Substack Article #1                         │
└─────────────────────────────────────────────────────────────────┘
                              │
                              ▼
┌─────────────────────────────────────────────────────────────────┐
│  Step 2: Portfolio Look                                         │
│  ──────────────────────                                         │
│  Input:  Published Market Look text + 2 portfolio screenshots   │
│  Output: Portfolio update report                                │
│  Action: Publish as Substack Article #2                         │
└─────────────────────────────────────────────────────────────────┘
```

**Key implication:** When the Portfolio Look output references the Market Look, it should do so as a *published article* that readers may have already read — not as internal analysis.

## Inputs

### 1. Market Look Article (Text)
- The full text of the published Market Look report
- Pasted into the prompt by the user
- Treated as a reference document the reader may have seen

### 2. Portfolio Screenshot
- Screenshot from allocatesmartly.com (or similar)
- Contains:
  - Portfolio name (top left)
  - Performance chart vs 60/40 benchmark (1-year timeframe, bottom left)
  - **New recommended allocations** with ± change indicators (right panel)
  - Recent returns including MTD (bottom right)

**Important:** The allocations shown are NEW recommendations, not current holdings. To get current/past allocation: Displayed − Change.

### 3. Benchmark Screenshot
- Screenshot in the same format as the portfolio
- Typically a 60/40 benchmark for comparison
- Same timeframe and format for apples-to-apples comparison

## Output Structure

**Length:** Opening + 3 sections (approximately 300-400 words)

The output has two parts with clean section headers:

### Part 1 — How We Did (Backward-Looking)

**Opening framing sentence** — References Market Look, sets up both performance review and changes assessment

**How we did (Performance Summary)**
- State portfolio's MTD % from the chart
- State benchmark's MTD %
- Compare: outperformed/underperformed by how much (plain language)
- Describe 12-month visual narrative from the chart

**Why it happened (Attribution & Market Look Reflection)**
- Describe current/past positioning (calculated from Displayed − Change)
- Look up ETF MTD performance to explain what drove gains/losses
- Connect performance to Market Look themes: did our tilts help or hurt?

### Part 2 — What's Changing (Forward-Looking)

**Recommended adjustments (Changes Assessment)**
- Summarize key recommended changes (what's going up/down)
- Assess whether changes align with or conflict with Market Look signals
- Plain-language analysis (not advice on whether to follow)

**Section headers:** Use "**How we did**", "**Why it happened**", "**Recommended adjustments**" as bold text on their own line. No parenthetical explanations.

## Key Requirements

### Portfolio Context: TAA Strategies

The portfolios analyzed are Tactical Asset Allocation (TAA) strategies — rules-based approaches that Jeff follows mechanically with month-end adjustments. Key characteristics:
- Mechanical execution (strategy dictates allocation)
- Month-end rebalancing
- Typical TAA tradeoff: may lag in strong bull markets as cost of avoiding big drawdowns

This is background context, not required commentary.

### ETF Lookup
The GPT must look up what ETFs actually hold, not rely on shorthand labels.

**Example:**
- Screenshot says "IEMG - Emerging market equities"
- Actual: IEMG tracks the MSCI Emerging Markets index (international emerging-market stocks, NOT U.S.)

**Critical terminology:** Always say "international emerging-market stocks" — never just "emerging markets." This ensures EM is correctly counted as part of international exposure.

### Market Look Reference Style
Because the Market Look is a published article, references should sound like cross-references between articles:

**Good:**
- "As I noted in this month's Market Look..."
- "The Market Look I published earlier this month pointed out that..."
- "This month's Market Look highlighted..."
- "If you read the Market Look, you'll recall..."

**Bad:**
- "Based on the analysis above..."
- "According to the Market Look report provided..."
- "The pasted Market Look says..."

The Portfolio Look should feel like a **companion piece** to Article 1.

### Style Constraints
- Plain English, newsletter tone
- No predictions, no trade instructions, no price targets
- If the chart/report doesn't support a claim, say so
- Use the portfolio name from the screenshot (e.g., "OptimHybrid")

## What to Include (Only What Inputs Support)

| Element | Source | Required |
|---------|--------|----------|
| Portfolio MTD % | Portfolio screenshot | ✅ |
| Benchmark MTD % | Benchmark screenshot | ✅ |
| MTD comparison (delta) | Calculated | ✅ |
| 12-month narrative | Portfolio chart visual | ✅ |
| Current holdings/weights | Portfolio screenshot | ✅ |
| Biggest weights called out | Portfolio screenshot | ✅ |
| Cash/bonds vs equities mix | Portfolio screenshot | ✅ |
| Market Look theme alignment | Market Look text + positioning | ✅ |
| What aligns / what's at odds | Analysis | ✅ |

## What NOT to Include

- Trade recommendations
- Price targets
- Timing suggestions
- Claims not supported by the inputs
- Predictions about future performance

## Aspirational Output Example

> OptimHybrid is having a strong month so far: it's up +5.80% Month-to-Date, versus the 60/40 benchmark's +0.56%, so it's ahead by about 5.24 percentage points. Over the last 12 months on the chart (Jan 2025 – Jan 2026), OptimHybrid spent much of the year running below the benchmark line after the early-year dip, then started closing the gap in the back half of the year, and finally caught up and finished above the benchmark with a sharp move higher right at the end of the period.
>
> Positioning helps explain why this portfolio may behave differently than a plain 60/40. OptimHybrid is equity-heavy and globally tilted, led by IEMG (33.3%) for emerging-markets stocks and IEFA (13.3%) for developed international stocks, plus meaningful small-cap exposure (IWM 10% in U.S. small caps and SCZ 10% in international small caps). On the "defensive/real asset" side it holds 10% cash, 6.1% gold (GLD), and only 1.7% in intermediate Treasuries (IEF). That mix broadly lines up with this month's Market Look's "stocks over bonds" backdrop (very little bond exposure here), and it also leans into the report's note that small caps may be starting to improve (IWM/SCZ). Where it's less aligned is the report's point that developed international has been beating emerging markets lately – OptimHybrid's single biggest weight is emerging markets, even though it also carries a sizable developed-international sleeve (IEFA plus Europe/Japan). The chart alone can't prove which sleeve drove this month's jump, but the result is clear: the portfolio's current tilts have translated into a big Month-to-Date lead over the benchmark.

## Article Framing

The Portfolio Look is explicitly a **companion piece** to the Market Look article. The output should:

- Open with a framing sentence that references the Market Look and suggests readers check it out
- Assume the Market Look exists as a published article (with an embedded link the user will add)
- Not repeat the Market Look's analysis — just reference its conclusions when connecting to portfolio positioning

**Example opening framing:**
> "Today we want to look at our portfolio to see how it did for the past month and also how it is positioned relative to this month's Market Look."

The user will add the embedded link to "Market Look" when publishing. The GPT output should write in a way that makes this natural.

## Open Questions

1. **Multiple portfolios:** If the user provides multiple portfolio screenshots, should we produce separate sections or one combined analysis?

2. **Naming:** Should this be called "Portfolio Look" to parallel "Market Look," or something else like "Portfolio Update"?

## Implementation Checklist

- [ ] Create portfolio-reference-guide.md (knowledge file)
- [ ] Design output-format additions for Portfolio Look
- [ ] Update instructions.md Task 2 with real logic
- [ ] Update conversation starters if needed
- [ ] Test with OptimHybrid + benchmark screenshots
- [ ] Test with LessBold + benchmark screenshots
- [ ] Iterate based on output quality
- [ ] Document any model requirements (thinking mode?)

## Sample Charts Available

| File | Purpose |
|------|---------|
| samples/portcharts/benchmark-012426.png | 60/40 benchmark reference |
| samples/portcharts/optimhybrid-012426.png | OptimHybrid portfolio |
| samples/portcharts/lessbold-012426.png | LessBold portfolio |
