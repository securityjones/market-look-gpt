# Chart Reference Guide

## Purpose

This document provides specific interpretation rules for charts used in Market Look analysis. When a chart is listed here, the GPT should follow these guidelines for interpretation and threshold-based conclusions.

For charts not listed in this guide, the GPT should use its general knowledge of technical analysis while adhering to the tone and output format requirements.

## SMA Interpretation Framework (All Ratio Charts)

This framework applies to all ratio charts (e.g., VOO:IJR, VOO:VEA, VOO:VWO, VOO:QQQ, VOO:IEF). Use these rules to interpret moving average relationships and derive posture implications.

### Understanding Ratio Charts

In a ratio chart like A:B (e.g., VOO:IJR):
- **Rising ratio** = A is outperforming B
- **Falling ratio** = B is outperforming A
- The SMAs (50-day and 200-day) show the trend of this relative performance

### SMA Crossover Signals

| Signal | What Happens | Interpretation |
|--------|--------------|----------------|
| **Golden Cross** | 50 SMA crosses *above* 200 SMA | Bullish for the numerator — potential sustained outperformance beginning |
| **Death Cross** | 50 SMA crosses *below* 200 SMA | Bearish for the numerator — potential sustained underperformance beginning |

These are lagging indicators that confirm *after* a move starts, but they often mark **regime changes** — sustained shifts in leadership that can last months.

### Price Position Relative to SMAs

| Position | Interpretation |
|----------|----------------|
| Price above both 50 & 200 SMA | Strong uptrend — clear momentum favoring the numerator |
| Price below both 50 & 200 SMA | Strong downtrend — sustained weakness in the numerator |
| Price between 50 & 200 SMA | Transitional — trend uncertain or potentially changing |
| Price bounces off SMA from above | SMA acting as support — trend intact |
| Price rejected at SMA from below | SMA acting as resistance — prior trend still dominant |

### Slope Analysis

| Slope Pattern | Interpretation |
|---------------|----------------|
| Both SMAs rising | Healthy uptrend — momentum building |
| Both SMAs falling | Sustained decline — weakness entrenched |
| SMAs flattening | Trend exhaustion — potential reversal ahead |
| 50 SMA rising, 200 SMA flat/falling | Early recovery — watch for confirmation |
| 50 SMA falling, 200 SMA flat/rising | Early deterioration — watch for breakdown |

### Signal Freshness (Monthly Reporting Context)

For monthly reports, distinguish between fresh signals and established conditions:

| Situation | Interpretation | Posture Implication |
|-----------|----------------|---------------------|
| Golden cross *this month* after downtrend | Fresh regime change signal | Consider shifting emphasis toward the numerator |
| Golden cross occurred months ago, still holding | Established trend, continuation | Continued emphasis on numerator remains supported |
| Golden cross this month but price falls back below SMAs | Failed signal / false start | Wait for confirmation before adjusting |
| Death cross *this month* after uptrend | Fresh reversal signal | Consider reducing emphasis on the numerator |
| Death cross occurred months ago, still holding | Established weakness | Reduced emphasis on numerator remains appropriate |

### Confirmation Criteria

A crossover signal is more reliable when:
- Price stays on the expected side of both SMAs after the cross
- Volume (if visible) supports the move
- The signal aligns with other charts in the analysis

A crossover signal is suspect when:
- Price immediately reverses back through the SMAs
- The cross happens in a choppy, sideways range
- Other charts show conflicting signals

### Posture Language (Tone-Guide Compliant)

When translating SMA signals into the "What Should We Do?" section, use measured language:

**For fresh bullish signals (golden cross, price breaking above SMAs):**
- "It may make sense to consider increasing exposure to [numerator] relative to [denominator]"
- "Early signs suggest [numerator] may be entering a period of relative strength"
- "This argues for openness to [numerator], while watching for confirmation"

**For fresh bearish signals (death cross, price breaking below SMAs):**
- "It may make sense to consider reducing emphasis on [numerator]"
- "The shift suggests [denominator] may be taking leadership"
- "Caution toward [numerator] appears warranted until conditions clarify"

**For established trends:**
- "Continued emphasis on [numerator/denominator] remains supported by the trend"
- "The pattern that has favored [X] over [Y] remains intact"

**For uncertain/transitional conditions:**
- "The trend is unclear — this argues for balance rather than strong emphasis either way"
- "Conditions are shifting but not yet decisive — patience is appropriate"

## Charts with Specific Interpretation Rules

### VIX (Volatility Index)

**What it measures:**
The market's expectation of near-term volatility, often called the "fear gauge." Higher readings indicate more uncertainty or stress; lower readings indicate calmer conditions.

**Key thresholds:**

| Level | Market Condition | Interpretation |
|-------|------------------|----------------|
| Below 12 | Extremely calm | Complacency risk — markets may be underpricing risk |
| 12–20 | Normal/calm | Healthy conditions — supportive for equities |
| 20–30 | Elevated | Uncertainty rising — some caution warranted |
| 30–40 | High stress | Significant fear — defensive posture appropriate |
| Above 40 | Panic/crisis | Extreme fear — often precedes contrarian opportunities |

**Trend matters as much as level:**

| Pattern | Interpretation |
|---------|----------------|
| Low and stable | Calm, supportive — but watch for complacency |
| Low but rising | Early warning — stress building, watch closely |
| Elevated but falling | Stress receding — constructive for risk assets |
| Spiking sharply | Active stress event — consider defensive moves |
| High but falling from spike | Fear exhausting — potential stabilization ahead |

**Month-to-month guidance:**
- A spike *this month* that has since receded = stress tested but resolved
- Sustained elevation over multiple months = persistent uncertainty
- Grinding lower over months = improving risk environment
- Breaking below a prior floor = new level of calm (watch for complacency)

**How to communicate:**
- Low VIX: "calmer conditions," "less day-to-day turbulence," "a quieter environment"
- High VIX: "elevated uncertainty," "more turbulent conditions," "investors are nervous"
- Falling VIX: "fear is receding," "conditions are settling," "stress is easing"
- Rising VIX: "uncertainty is building," "turbulence is increasing"
- Spike and retreat: "the market tested a stressful moment and stabilized"

### NAHL (New Highs vs New Lows)

**What it measures:**
The balance between stocks reaching new 52-week highs versus new 52-week lows.

**Key signal: The 13-day EMA only.** Daily readings are background noise — focus entirely on the smoothed 13-day EMA for interpretation and signal strength.

**Key thresholds (13-day EMA):**

| Level | Interpretation | Posture |
|-------|----------------|---------|
| Above +50 | Solid risk-on signal | Confidently invested in equities |
| Above 0 | Risk-on for equities | Normal equity exposure appropriate |
| Below 0 | Risk-off signal | Cautious; consider reducing exposure |
| Below -50 | Significant stress | Consider moving toward cash |

**Month-to-month guidance:**
- Crossing below zero from above = shift to cautious stance
- Crossing above zero from below = improving conditions, but confirm with other charts
- Sustained readings above +50 = strong confirmation to stay invested
- Sustained readings below -50 = widespread deterioration, consider defensive moves

**How to communicate:**
NAHL is a decision signal — communicate what it tells you to DO, not what the indicator shows:

| Situation | What to say |
|-----------|-------------|
| Above +50 | "The breadth signal confirms we should be confidently invested in stocks" |
| Above 0 | "The breadth signal supports staying invested in stocks" |
| Crossing above 0 | "The breadth signal has moved out of caution territory — it now supports being invested" |
| Crossing below 0 | "The breadth signal has flipped to caution — it argues for reducing stock exposure" |
| Below 0 | "The breadth signal is in cautious territory" |
| Below -50 | "The breadth signal is flashing a 3-alarm warning — consider moving some holdings to cash" |

**Do NOT** just describe what the indicator shows ("more highs than lows"). The reader needs to know what the signal *means for their posture*.

## Charts Using General Interpretation

*For the following charts, use the SMA Interpretation Framework above plus general technical analysis knowledge. Specific interpretation rules may be added later.*

### VOO:IJR (Large vs Small Cap Ratio)
- General: Rising = large caps outperforming small caps; Falling = small caps outperforming large caps
- **Plain language:** Describe as "large companies" vs "smaller companies"
- *Specific thresholds to be defined*

### VOO:QQQ (Broad Market vs Tech-Heavy)
- General: Rising = broad market outperforming tech-heavy stocks; Falling = tech-heavy stocks outperforming broad market
- **Plain language:** Describe as "the broad market" vs "tech-heavy stocks"
- **Do NOT use:** "concentrated," "concentration," "narrow leadership" — these are forbidden abstractions
- *Specific thresholds to be defined*

### VOO:IEF (Stocks vs Bonds)
- General: Rising = stocks outperforming bonds; Falling = bonds outperforming (flight to safety)
- Part of the "Stocks vs Safety" group — compare with VOO:IAU and VOO:BCI
- *Specific thresholds to be defined*

### VOO:IAU (Stocks vs Gold)
- General: Rising = stocks outperforming gold; Falling = gold outperforming (defensive/inflation hedge gaining)
- Part of the "Stocks vs Safety" group — compare with VOO:IEF and VOO:BCI
- **Plain language:** Describe as "stocks vs gold" or "gold as a safe haven"
- Gold often rises during uncertainty, inflation concerns, or loss of confidence in financial assets
- *Specific thresholds to be defined*

### VOO:BCI (Stocks vs Commodities)
- General: Rising = stocks outperforming commodities; Falling = commodities outperforming
- Part of the "Stocks vs Safety" group — compare with VOO:IEF and VOO:IAU
- **Plain language:** Describe as "stocks vs commodities" or "real assets"
- Commodities often rise during inflationary periods or supply-driven stress
- *Specific thresholds to be defined*

### VOO:VEA (US vs International Developed)
- General: Rising = US outperforming developed international; Falling = developed international outperforming US
- Part of the "US vs International" group — compare with VOO:VWO
- *Specific thresholds to be defined*

### VOO:VWO (US vs Emerging Markets)
- General: Rising = US outperforming emerging markets; Falling = emerging markets outperforming US
- Part of the "US vs International" group — compare with VOO:VEA
- Together, VOO:VEA and VOO:VWO answer the question "US or international?" — if both favor international, that's a clear signal; if mixed, explain which part of international is leading
- *Specific thresholds to be defined*

## Adding New Interpretations

When adding interpretation rules for a chart, include:

1. **What it measures** — Plain-language explanation
2. **Key thresholds** — Specific levels and what they mean
3. **Month-to-month guidance** — How to interpret changes between reports
4. **How to communicate** — Suggested phrasing for non-technical sections
