# Screenshot Reference Guide

## Purpose

This document provides interpretation rules for portfolio screenshots used in Portfolio Look analysis. It defines where to find key information, how to extract it accurately, and common pitfalls to avoid.

## Screenshot Format (allocatesmartly.com style)

Portfolio screenshots from allocatesmartly.com typically contain:

```
┌─────────────────────────────────────────────────────────────────┐
│  Portfolio Name (top left)                                      │
│                                                                 │
│  ┌─────────────────────────────────┐  ┌──────────────────────┐ │
│  │                                 │  │ Current Holdings     │ │
│  │    Performance Chart            │  │ ────────────────     │ │
│  │    (portfolio vs benchmark)     │  │ ETF1  XX.X%          │ │
│  │                                 │  │ ETF2  XX.X%          │ │
│  │    1-year timeframe             │  │ ETF3  XX.X%          │ │
│  │                                 │  │ ...                  │ │
│  │                                 │  ├──────────────────────┤ │
│  │                                 │  │ Recent Returns       │ │
│  │                                 │  │ ────────────────     │ │
│  │                                 │  │ MTD: +X.XX%          │ │
│  │                                 │  │ YTD: +X.XX%          │ │
│  │                                 │  │ 1-Yr: +X.XX%         │ │
│  └─────────────────────────────────┘  └──────────────────────┘ │
└─────────────────────────────────────────────────────────────────┘
```

### Key locations:

| Element | Where to find it |
|---------|------------------|
| Portfolio name | Top left corner |
| Performance chart | Center/left main area |
| Current holdings & weights | Right panel, upper section |
| MTD (Month-to-Date) return | Right panel, below holdings |
| Benchmark comparison line | On the performance chart (typically gray/secondary line) |

---

## Extracting Key Data

### Portfolio Name
- Found in the top left of the screenshot
- Use this name throughout the output (e.g., "OptimHybrid," "LessBold")
- Do not rename or abbreviate

### Month-to-Date (MTD) Return
- Found in the returns section of the right panel
- Usually labeled "MTD" or "Month-to-Date"
- Extract the exact percentage (e.g., "+5.80%")
- Include the sign (+ or -)

### Holdings and Weights
- Listed in the right panel with percentages
- Format is typically: `TICKER  XX.X%`
- Extract all holdings and their weights
- Note which are equities, bonds, cash, or other (gold, commodities)

---

## ETF Lookup Requirement (CRITICAL)

**Do NOT trust the shorthand descriptions on screenshots.**

Screenshots often show abbreviated or misleading labels. You MUST use your knowledge (or web search if needed) to understand what each ETF actually tracks before categorizing it.

### Examples of misleading labels:

| Screenshot shows | Actual holding |
|------------------|----------------|
| "IEMG - Emerging market equities" | MSCI Emerging Markets index — international emerging markets, NOT U.S. |
| "IEF - Treasuries" | Intermediate-term U.S. Treasury bonds (7-10 year) |
| "IWM - Small cap" | U.S. small-cap stocks (Russell 2000) |
| "SCZ - Small cap" | International small-cap stocks (NOT U.S.) |

### Why this matters:
- Positioning analysis depends on understanding geographic and asset class exposure
- Confusing "emerging market equities" with U.S. equities would produce wrong conclusions
- The Market Look connection requires accurate categorization

### How to handle ETF lookup:

1. **First:** For each ETF ticker on the screenshot, recall or look up what index it tracks and what it actually holds
2. **Then:** Categorize it into one of the categories below based on what you learned

The categorization table below is a reference for common ETFs — but if you encounter an ETF not listed, look it up rather than guessing.

### ETF categorization (common examples):

| Category | Examples |
|----------|----------|
| **U.S. Large Cap** | VOO, SPY, IVV, RSP |
| **U.S. Small Cap** | IWM, IJR, VB |
| **U.S. Tech-Heavy** | QQQ, QQQM, VGT |
| **International Developed** | IEFA, VEA, EFA |
| **International Developed (Single Country)** | EWJ (Japan), EWS (Singapore) |
| **International Small Cap** | SCZ, VSS |
| **Emerging Markets** | IEMG, VWO, EEM |
| **Emerging Markets (Single Country)** | EWZ (Brazil) |
| **U.S. Bonds (Intermediate)** | IEF, AGG, BND |
| **U.S. Bonds (Long-Term)** | TLT, VGLT |
| **International Bonds** | BNDX, IAGG |
| **Cash/Short-term** | Cash, SHV, BIL |
| **Commodities** | BCI, PDBC, DBC |
| **Gold** | GLD, IAU |
| **Real Estate (REITs)** | SCHH |

---

## Reading the Performance Chart

### What to observe:

1. **Relative position now:** Is the portfolio line above or below the benchmark at the right edge?

2. **12-month path:** Trace the portfolio line from left to right:
   - Did it start above or below the benchmark?
   - When did it diverge (pull away)?
   - When did it converge (come back together)?
   - Were there notable crossovers?

3. **Recent trend:** Focus on the last 1-3 months:
   - Is the gap widening or narrowing?
   - Is the portfolio line rising, falling, or flat?

### Describing the visual narrative:

**Good descriptions:**
- "spent much of the year running below the benchmark line"
- "started closing the gap in the back half of the year"
- "caught up and finished above the benchmark with a sharp move higher"
- "the lines tracked closely until Q3, then diverged"

**Bad descriptions:**
- "performed well" (too vague)
- "beat the benchmark" (only describes the endpoint, not the journey)
- Making up specific dates or events not visible on the chart

### Honesty about limitations:
- If you can't clearly see something on the chart, say so
- Don't invent narrative the chart doesn't support
- Example: "The chart alone can't prove which sleeve drove this month's jump"

---

## Benchmark Screenshots

The benchmark screenshot (typically 60/40) uses the same format.

### What to extract:
- Benchmark name (e.g., "60/40 Benchmark")
- MTD return percentage
- The benchmark line is the comparison reference

### Calculating the delta:
- Portfolio MTD minus Benchmark MTD = outperformance/underperformance
- Example: +5.80% - +0.56% = +5.24 percentage points ahead
- Express in plain language: "ahead by about 5.24 percentage points"

---

## Categorizing Portfolio Positioning

After extracting holdings, summarize the portfolio's positioning using this hierarchy. This structure maps directly to the Market Look themes, making it easy to compare alignment.

### Top-Level Splits (always state with approximate percentages):

**1. Stocks vs Safety**
- Stocks = all equity ETFs (U.S. + international)
- Safety = bonds + cash + gold/commodities combined
- Example: "about 75% stocks and 25% safety (bonds, cash, gold)"

**2. U.S. vs International (within stocks)**
- Calculate the split within the stock portion
- Example: "Within stocks, about 25% U.S. and 75% international"

**Important:** IEFA, VEA, EFA are international developed stocks — they count toward international, not U.S.

### Second-Level Splits (mention if meaningful exposure exists):

**3. Developed vs Emerging (within international)**
- If the portfolio has both developed (IEFA, VEA) and emerging (IEMG, VWO), note the balance
- Example: "The international exposure is mostly developed markets (IEFA), with a smaller emerging-markets slice (IEMG)"

**4. Small vs Large (if notable small-cap exposure)**
- If the portfolio holds small-cap ETFs (IWM, IJR, SCZ), mention it
- Example: "includes meaningful small-cap exposure through IWM and SCZ"

### Why This Structure

These four dimensions map directly to Market Look themes:

| Portfolio Slice | Market Look Theme |
|-----------------|-------------------|
| Stocks vs Safety | "Stocks doing better than bonds" / risk-on vs risk-off |
| U.S. vs International | "U.S. vs international" |
| Developed vs Emerging | "Developed vs emerging" |
| Small vs Large | "Smaller companies perking up" |

This makes it easy to connect positioning to the Market Look: state the portfolio's tilt, then note whether it aligns or conflicts with what the Market Look observed.

### Example positioning summary:

> "LessBold is about 75% stocks and 25% safety (12% Treasury bonds, 13% cash). Within stocks, it's heavily international — roughly 70% international and 30% U.S. The international exposure is led by IEFA (40.8%) for developed markets, with a smaller slice in IEMG (9.8%) for emerging markets plus single-country positions in Brazil (EWZ) and Singapore (EWS). It also has meaningful small-cap exposure through IWM (9.8%) on the U.S. side."

Note how this flows: stocks vs safety → U.S. vs international → developed vs emerging → small vs large. Each layer sets up a potential alignment or conflict with the Market Look.

---

## Common Pitfalls

| Pitfall | How to avoid |
|---------|--------------|
| Trusting ETF labels on screenshot | Always look up what the ETF actually holds |
| Confusing international with U.S. | Check each ETF's underlying index |
| Inventing chart narrative | Only describe what you can see |
| Missing the MTD numbers | Always extract exact percentages from both screenshots |
| Forgetting to calculate delta | State outperformance/underperformance explicitly |
| Vague positioning descriptions | Include percentages and specific ETF names |
