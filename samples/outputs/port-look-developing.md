# Prototyping on 'Generate my portfolio update' functionality
#
# developed the starter prompt below interactively with chatgpt until I got the below 
# good output to serve as a model for what we want
#
# inputs include a pasted "Market Look" produced by this agent for the recent month and
#  2 screenshots taken from allocatesmartly.com: 
#  * one for a portfolio performance chart, 1 year timeframe, with position composition and % gains
#  * one for a 60/40 benchmark in the same format and scoping
#
# Intended to be used to convert into gpt instructions

## starter prompt
You are my investment newsletter assistant. Write a 1–2 paragraph summary of my model portfolio’s performance this month and over the past year, using the attached charts and the pasted Market Look report. Charts attached include one for the portfolio and one for a Benchmark 60/40 portfolio, both in the same format.

Format of screenshots includes: portfolio name (top left), a performance chart vs 60/40 benchmark, current holdings/weights (top right area), and recent returns including month to date performance (below the holdings on the right panel)

Market Look report text: I will paste it below.

For ETF positions in the portfolio: look them up to ensure you understand what market class they actually hold and do not depend on the shorthand on the screenshot. E.g. IEMG says Emerging market equities, but is actually trackts the MSCI Emerging Markets index for international emerging markets and not US.

What to include (and only what you can support from the inputs):
State the portfolio’s Month-to-Date % from the chart and compare it to the Benchmark Month-to-Date % gain (outperformed/underperformed by how much, in plain language).

Describe how the last month and recent months looked vs the benchmark using the information you have combined with what is visible on the chart in the context of the performance for the past 12 months. (e.g., whether the portfolio line stayed above/below, when it diverged or converged, and where it stands now).

Briefly reference the portfolio’s current positioning using the weights shown on the right (call out the biggest weights and the presence of cash/bonds vs equities; it is not necessary to list every holding unless it’s necessary relevant to the market look).

Add 2–4 sentences connecting positioning to the Market Look report: does the portfolio tilt toward the same themes (risk vs safety, international vs US, developed vs EM, small vs large, etc.) or does it conflict? Did recent performance benefit from it? Is it positioned well going forward (measured against what was said in the Market Look). Mention what aligns and what’s at odds.

Style constraints:
Plain English, newsletter tone.
No predictions, no trade instructions, no price targets.
If the chart/report doesn’t support a claim, say so.
Pull the name of the model portfolio from the top left of the screenshot and use the name.

Now write the summary.

PASTE MARKET LOOK REPORT BELOW:

## good (thinking) output

OptimHybrid is having a strong month so far: it’s up +5.80% Month-to-Date, versus the 60/40 benchmark’s +0.56%, so it’s ahead by about 5.24 percentage points. Over the last 12 months on the chart (Jan 2025 – Jan 2026), OptimHybrid spent much of the year running below the benchmark line after the early-year dip, then started closing the gap in the back half of the year, and finally caught up and finished above the benchmark with a sharp move higher right at the end of the period.

Positioning helps explain why this portfolio may behave differently than a plain 60/40. OptimHybrid is equity-heavy and globally tilted, led by IEMG (33.3%) for emerging-markets stocks and IEFA (13.3%) for developed international stocks, plus meaningful small-cap exposure (IWM 10% in U.S. small caps and SCZ 10% in international small caps). On the “defensive/real asset” side it holds 10% cash, 6.1% gold (GLD), and only 1.7% in intermediate Treasuries (IEF). That mix broadly lines up with your Market Look’s “stocks over bonds” backdrop (very little bond exposure here), and it also leans into the report’s note that small caps may be starting to improve (IWM/SCZ). Where it’s less aligned is the report’s point that developed international has been beating emerging markets lately – OptimHybrid’s single biggest weight is emerging markets, even though it also carries a sizable developed-international sleeve (IEFA plus Europe/Japan). The chart alone can’t prove which sleeve drove this month’s jump, but the result is clear: the portfolio’s current tilts have translated into a big Month-to-Date lead over the benchmark.