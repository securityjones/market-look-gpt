# Chart Reference Guide

## Purpose

This document provides specific interpretation rules for charts used in Market Look analysis. When a chart is listed here, the GPT should follow these guidelines for interpretation and threshold-based conclusions.

For charts not listed in this guide, the GPT should use its general knowledge of technical analysis while adhering to the tone and output format requirements.

---

## Ratio Chart Fundamentals

**This section applies to all ratio charts:** VOO:IEF, VOO:IAU, VOO:BCI, VOO:VEA, VOO:VWO, VOO:IJR, VOO:QQQ. Master this before interpreting any ratio chart.

### What a Ratio Chart Shows

A ratio chart like A:B (e.g., VOO:IJR) displays A divided by B. It shows **relative performance** between two assets — not the absolute price of either one.

- **Rising ratio** → the numerator (first symbol) is outperforming the denominator (second symbol)
- **Falling ratio** → the denominator (second symbol) is outperforming the numerator (first symbol)
- **Flat ratio** → roughly equal performance between the two

### Terminology

| Term | Meaning |
|------|---------|
| **Numerator** | The first symbol (before the colon). In VOO:IJR, VOO is the numerator. |
| **Denominator** | The second symbol (after the colon). In VOO:IJR, IJR is the denominator. |
| **Ratio** | The value shown on the chart. Say "ratio" not "price" when describing ratio charts. |

### What to Observe (in this order)

1. **Recent bars vs one month ago** — Where is the ratio now compared to 4-5 bars left? Rising, falling, or flat?
2. **Ratio position vs MAs** — Is the ratio above or below the 10-week (short) and 40-week (long) moving averages?
3. **MA relationship** — Is the short MA above or below the long MA?
4. **MA crossovers** — Did a golden cross (short crosses above long) or death cross (short crosses below long) occur? If so, when?
   - **Within the last 4-5 bars** = this month; a fresh signal that may need confirmation
   - **Within the last 12-13 bars** = past few months; an established signal — check whether the most recent 4-5 bars are confirming (continuing in the crossover's direction) or reverting (moving back toward the prior trend)
   - **Older than ~13 bars** = well-established; describe as the prevailing trend rather than a recent event
5. **MA slope** — Are both MAs rising, falling, flattening, or mixed?

### Interpretation Rule — Do Not Invert

**⚠️ CRITICAL:** Your conclusion MUST match the ratio's direction. When the ratio is falling or below the MAs, the **DENOMINATOR is winning**, not the numerator.

| Chart | When ratio is FALLING or below MAs | Winner |
|-------|-----------------------------------|--------|
| VOO:IJR | Small caps beating large caps | IJR (small caps) |
| VOO:VEA | International beating US | VEA (international) |
| VOO:VWO | Emerging markets beating US | VWO (emerging) |
| VOO:IEF | Bonds beating stocks | IEF (bonds) |
| VOO:IAU | Gold beating stocks | IAU (gold) |
| VOO:BCI | Commodities beating stocks | BCI (commodities) |
| VOO:QQQ | Tech beating broad market | QQQ (tech) |

**Before writing any interpretation, ask yourself:** "Which side is winning based on what I observed?" Then verify your conclusion matches.

### Common Error to Avoid

❌ **Wrong:** "The ratio is below both MAs and falling. Large caps are still outperforming small caps."

✅ **Correct:** "The ratio is below both MAs and falling. Small caps are outperforming large caps."

The first example inverts the interpretation — it describes small caps winning but concludes large caps are ahead. This is the most common error. Always check that your conclusion matches your observation.

---

## SMA Interpretation Framework (All Ratio Charts)

This framework builds on the Ratio Chart Fundamentals above. Use these rules to interpret moving average relationships and derive posture implications.

### SMA Crossover Signals

| Signal | What Happens | Interpretation |
|--------|--------------|----------------|
| **Golden Cross** | 50 SMA crosses *above* 200 SMA | Bullish for the numerator — potential sustained outperformance beginning |
| **Death Cross** | 50 SMA crosses *below* 200 SMA | Bearish for the numerator — potential sustained underperformance beginning |

These are lagging indicators that confirm *after* a move starts, but they often mark **regime changes** — sustained shifts in leadership that can last months.

### Ratio Position Relative to SMAs

| Position | Interpretation |
|----------|----------------|
| Ratio above both short & long MA | Strong uptrend — clear momentum favoring the numerator |
| Ratio below both short & long MA | Strong downtrend — denominator is outperforming |
| Ratio between short & long MA | Transitional — trend uncertain or potentially changing |
| Ratio bounces off MA from above | MA acting as support — trend intact |
| Ratio rejected at MA from below | MA acting as resistance — prior trend still dominant |

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
| Golden cross this month but ratio falls back below MAs | Failed signal / false start | Wait for confirmation before adjusting |
| Death cross *this month* after uptrend | Fresh reversal signal | Consider reducing emphasis on the numerator |
| Death cross occurred months ago, still holding | Established weakness | Reduced emphasis on numerator remains appropriate |

### Confirmation Criteria

A crossover signal is more reliable when:
- Ratio stays on the expected side of both MAs after the cross
- Volume (if visible) supports the move
- The signal aligns with other charts in the analysis

A crossover signal is suspect when:
- Ratio immediately reverses back through the MAs
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

**This is a breadth indicator, NOT a ratio chart.** Do not apply ratio chart rules (no numerator/denominator, no "bars vs MAs" analysis, no crossover signals).

**What it measures:**
The balance between stocks reaching new 52-week highs versus new 52-week lows. It is the count of daily high minus the count of lows.

**Chart elements — two lines, one signal:**
- **13-day EMA (solid line)** — THE signal. Always focus on this. It's smoothed by design.
- **Daily readings (dotted line)** — Ignore completely unless the emergency threshold triggers (see below).

**What to observe:**
1. Current EMA value
2. Which threshold zone it's in (+50, 0, -50)
3. EMA direction: rising, falling, or flat over recent weeks
4. Recent threshold crossings: did it cross 0, +50, or -50 within the last 1-2 months?

**Do NOT observe or describe:**
- The dotted daily line (unless emergency)
- "Choppiness" or "swings" — that describes daily noise, not the smoothed EMA
- "Bars vs moving averages" — that's for ratio charts, not NAHL
- Comparisons to prior peaks that aren't recent (see recency rules below)

**Key thresholds (13-day EMA):**

| Level | Interpretation | Posture |
|-------|----------------|---------|
| Above +50 | Solid risk-on signal | Confidently invested in equities |
| Above 0 | Risk-on for equities | Normal equity exposure appropriate |
| Below 0 | Risk-off signal | Cautious; consider reducing exposure |
| Below -50 | Significant stress | Consider moving toward cash |

**Recency and comparisons to prior readings — when it's relevant:**

Threshold crossings reset the narrative anchor. Apply these rules:

- **"Recent"** for NAHL means 1-2 months (roughly 4-8 weeks)
- **If a threshold was crossed since the prior extreme:** The threshold crossing becomes the new story anchor, not the prior high/low
  - Example: EMA hit +80 in September, dipped near zero in November, now at +62 → The story is "recovered from November's dip to solidly above +50" — NOT "off from September highs"
- **If no threshold was crossed since the prior extreme AND it was within 1-2 months:** Referencing that prior reading is valid
  - Example: EMA hit +80 three weeks ago, now at +62 with no threshold crossing → "Still solid above +50, but pulling back a bit from recent highs"

**You CAN reference older readings** if you label them correctly:
- ✅ "hasn't reached the high signals from late last year"
- ✅ "below where it was several months ago"
- ✅ "not as strong as during the summer peak"

**Do NOT mislabel old readings as "recent":**
- ❌ "eased from recent highs" — when the high was 3+ months ago
- ❌ "cooled from higher readings" — implies recent decline when the decline happened months ago
- ❌ "off from recent highs" — same issue
- ❌ "pulled back a bit from recent highs" — same issue

The key rule: **Don't call something "recent" if it wasn't.** Acknowledging older context with accurate time references is fine.

**Emergency signal (rare):**
If the dotted daily line drops below -500, mention this as a severe stress warning — this is the only time to reference the dotted line. Otherwise, ignore it completely.

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

## Ratio Charts — Specific Notes

*All ratio charts follow the Ratio Chart Fundamentals and SMA Interpretation Framework above. This section provides chart-specific notes only.*

### VOO:IJR (Large vs Small Cap)
- **Numerator:** VOO (S&P 500 large caps)
- **Denominator:** IJR (S&P 600 small caps)
- **Plain language:** "large companies" vs "smaller companies"
- **Remember:** Ratio falling or below MAs = **small caps winning**

### VOO:QQQ (Broad Market vs Tech-Heavy)
- **Numerator:** VOO (S&P 500 broad market)
- **Denominator:** QQQ (Nasdaq-100 tech-heavy)
- **Plain language:** "the broad market" vs "tech-heavy stocks"
- **Remember:** Ratio falling or below MAs = **tech winning**
- **Do NOT use:** "concentrated," "concentration," "narrow leadership" — forbidden abstractions

### VOO:IEF (Stocks vs Bonds)
- **Numerator:** VOO (stocks)
- **Denominator:** IEF (intermediate Treasury bonds)
- **Plain language:** "stocks" vs "bonds"
- **Remember:** Ratio falling or below MAs = **bonds winning** (flight to safety)
- Part of the "Stocks vs Safety" group — compare with VOO:IAU and VOO:BCI

### VOO:IAU (Stocks vs Gold)
- **Numerator:** VOO (stocks)
- **Denominator:** IAU (gold)
- **Plain language:** "stocks" vs "gold"
- **Remember:** Ratio falling or below MAs = **gold winning** (defensive/inflation hedge gaining)
- Part of the "Stocks vs Safety" group — compare with VOO:IEF and VOO:BCI
- Gold often rises during uncertainty, inflation concerns, or loss of confidence in financial assets

### VOO:BCI (Stocks vs Commodities)
- **Numerator:** VOO (stocks)
- **Denominator:** BCI (broad commodities)
- **Plain language:** "stocks" vs "commodities" or "real assets"
- **Remember:** Ratio falling or below MAs = **commodities winning**
- Part of the "Stocks vs Safety" group — compare with VOO:IEF and VOO:IAU
- Commodities often rise during inflationary periods or supply-driven stress

### VOO:VEA (US vs International Developed)
- **Numerator:** VOO (US stocks)
- **Denominator:** VEA (developed international stocks)
- **Plain language:** "U.S. stocks" vs "stocks from other wealthy countries"
- **Remember:** Ratio falling or below MAs = **international developed winning**
- Part of the "US vs International" group — compare with VOO:VWO

### VOO:VWO (US vs Emerging Markets)
- **Numerator:** VOO (US stocks)
- **Denominator:** VWO (emerging market stocks)
- **Plain language:** "U.S. stocks" vs "emerging market stocks"
- **Remember:** Ratio falling or below MAs = **emerging markets winning**
- Part of the "US vs International" group — compare with VOO:VEA
- Together, VOO:VEA and VOO:VWO answer "US or international?" — if both favor international, that's a clear signal; if mixed, explain which part of international is leading

## Adding New Interpretations

When adding interpretation rules for a chart, include:

1. **What it measures** — Plain-language explanation
2. **Key thresholds** — Specific levels and what they mean
3. **Month-to-month guidance** — How to interpret changes between reports
4. **How to communicate** — Suggested phrasing for non-technical sections
