# Chart Reference Guide

## Purpose

This document provides specific interpretation rules for charts used in Market Look analysis. When a chart is listed here, the GPT should follow these guidelines for interpretation and threshold-based conclusions.

For charts not listed in this guide, the GPT should use its general knowledge of technical analysis while adhering to the tone and output format requirements.

## SMA Interpretation Framework (All Ratio Charts)

This framework applies to all ratio charts (e.g., IJR:VOO, VOO:VEA, VEA:VWO, QQQ:RSP, VOO:IEF). Use these rules to interpret moving average relationships and derive posture implications.

### Understanding Ratio Charts

In a ratio chart like A:B (e.g., IJR:VOO):
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
The balance between stocks reaching new 52-week highs versus new 52-week lows. The 13-day EMA (exponential moving average) smooths daily fluctuations.

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
- Sustained readings above +50 = healthy broad participation
- Sustained readings below -50 = widespread deterioration

**How to communicate:**
- Above 0: "more stocks reaching new highs than new lows"
- Below 0: "more stocks falling to new lows than reaching new highs"
- Crossing zero: "the balance has shifted" (describe direction)

## Charts Using General Interpretation

*For the following charts, use the SMA Interpretation Framework above plus general technical analysis knowledge. Specific interpretation rules may be added later.*

### IJR:VOO (Small vs Large Cap Ratio)
- General: Rising = small caps outperforming; Falling = large caps outperforming
- *Specific thresholds to be defined*

### QQQ:RSP (Concentration Proxy)
- General: Rising = narrow leadership (tech-heavy); Falling = broader participation
- *Specific thresholds to be defined*

### VOO:IEF (Stocks vs Bonds)
- General: Rising = stocks outperforming safer assets; Falling = flight to safety
- *Specific thresholds to be defined*

### VOO:VEA (US vs International Developed)
- General: Rising = US outperforming; Falling = international outperforming
- *Specific thresholds to be defined*

### VEA:VWO (Developed vs Emerging International)
- General: Rising = developed international outperforming; Falling = emerging markets outperforming
- *Specific thresholds to be defined*

## Adding New Interpretations

When adding interpretation rules for a chart, include:

1. **What it measures** — Plain-language explanation
2. **Key thresholds** — Specific levels and what they mean
3. **Month-to-month guidance** — How to interpret changes between reports
4. **How to communicate** — Suggested phrasing for non-technical sections
