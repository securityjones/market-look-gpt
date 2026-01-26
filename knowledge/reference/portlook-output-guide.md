# Portfolio Look Output Format Guide

## Purpose

This document defines the required structure, content, and presentation for Jeff's monthly portfolio update posts.

The Portfolio Look is a **companion piece** to the Market Look article. It analyzes portfolio performance and positioning, then connects both to the themes from the published Market Look.

This guide governs what the reader sees.

## Article Framing

The Portfolio Look should open with a framing sentence that:
- References the Market Look as a published article
- Sets up the purpose: reviewing portfolio performance and positioning
- Makes it natural for Jeff to add an embedded link to "Market Look" when publishing

**Example opening:**
> "Today we want to look at our portfolio to see how it did for the past month and also how it is positioned relative to this month's Market Look."

The GPT should write this framing naturally — Jeff will add the hyperlink when publishing.

## Required Inputs

The Portfolio Look requires three inputs:

1. **Market Look article text** — The published Market Look, pasted by the user
2. **Portfolio screenshot** — From allocatesmartly.com or similar
3. **Benchmark screenshot** — Typically 60/40, same format as portfolio

## Output Structure

The output consists of:
1. **Opening framing sentence** (references Market Look)
2. **Paragraph 1** — Performance summary (MTD comparison, 12-month chart narrative)
3. **Paragraph 2** — ETF attribution (which holdings drove gains/losses)
4. **Paragraph 3** — Positioning and Market Look connection

Total length: Opening + 3 paragraphs (approximately 250-350 words total)

---

## Opening Framing Sentence

One sentence that:
- Tells the reader what we're doing (reviewing the portfolio)
- References this month's Market Look
- Sets up both performance review and positioning analysis

**Good examples:**
- "Today we want to look at our portfolio to see how it did for the past month and also how it is positioned relative to this month's Market Look."
- "Let's check in on the portfolio — how did it do this month, and how does its positioning line up with what we covered in the Market Look?"

---

## Paragraph 1 — Performance Summary

This paragraph covers **what happened** — the numbers and the visual story from the chart.

### Required elements:

1. **Portfolio MTD %** — State the exact number from the screenshot
2. **Benchmark MTD %** — State the exact number from the screenshot
3. **Comparison** — Outperformed or underperformed, by how much, in plain language
4. **12-month visual narrative** — Describe the chart story:
   - Did the portfolio line stay above or below the benchmark?
   - When did it diverge or converge?
   - Where does it stand now relative to where it's been?

### Example:

> "OptimHybrid is having a strong month so far: it's up +5.80% Month-to-Date, versus the 60/40 benchmark's +0.56%, so it's ahead by about 5.24 percentage points. Over the last 12 months on the chart (Jan 2025 – Jan 2026), OptimHybrid spent much of the year running below the benchmark line after the early-year dip, then started closing the gap in the back half of the year, and finally caught up and finished above the benchmark with a sharp move higher right at the end of the period."

### Key rules:
- Use the portfolio name from the screenshot (e.g., "OptimHybrid")
- State actual numbers, not vague comparisons
- Describe what you can SEE on the chart — don't invent narrative the chart doesn't show
- Plain language throughout

---

## Paragraph 2 — ETF Attribution

This paragraph explains **where the gains or losses came from** by looking up individual ETF performance.

### Required action:

Look up the Month-to-Date performance for each significant ETF in the portfolio. Then report which holdings contributed most to the portfolio's gain or loss.

### What to include:

1. **Individual ETF MTD returns** — Look up the major holdings (no need to look up every tiny position)
2. **Attribution** — Which holdings drove most of the gain/loss? Which lagged or detracted?
3. **Plain-language summary** — Was it one holding doing the heavy lifting, or spread across several?

### Example:

> "Looking at the individual holdings this month, most of the gain came from the gold and bond sleeves. GLD was up around +8% for the month, and TLT gained about +5%, while SPY was roughly flat. So even though stocks are only 25% of this portfolio, the 'ballast' side—gold and long Treasuries—did the heavy lifting this month."

### Key rules:
- Look up actual MTD performance for ETFs (use web search if needed)
- Use **MTD** (Month-to-Date) terminology, not YTD, for consistency with Paragraph 1
- Keep it plain language — no need for precise weighted contribution math
- If performance was roughly uniform across holdings, say so
- If one or two holdings dominated, call them out
- This helps readers understand WHY the portfolio performed the way it did

---

## Paragraph 3 — Positioning & Market Look Connection

This paragraph covers **why** — what the portfolio holds and how that connects to market themes.

### Required elements:

1. **Current positioning summary:**
   - Call out the biggest weights (with percentages)
   - Note the equity/bond/cash mix
   - Identify geographic or style tilts (U.S. vs international, developed vs EM, large vs small)

2. **Market Look connection (2-4 sentences):**
   - Does the portfolio's positioning align with or conflict with the Market Look's themes?
   - Which themes are relevant: risk vs safety, U.S. vs international, developed vs EM, small vs large, tech-heavy vs broad?
   - Did the positioning help or hurt recent performance?
   - Is the portfolio well-positioned going forward based on the Market Look?

### Market Look reference style:

Reference the Market Look as a published article:

**Good:**
- "That mix broadly lines up with this month's Market Look's 'stocks over bonds' backdrop..."
- "...it also leans into the Market Look's note that small caps may be starting to improve"
- "Where it's less aligned is the Market Look's point that developed international has been beating emerging markets lately"

**Bad:**
- "According to the analysis provided..."
- "The pasted text indicates..."
- "Based on the report above..."

### Example:

> "Positioning helps explain why this portfolio may behave differently than a plain 60/40. OptimHybrid is equity-heavy and globally tilted, led by IEMG (33.3%) for emerging-markets stocks and IEFA (13.3%) for developed international stocks, plus meaningful small-cap exposure (IWM 10% in U.S. small caps and SCZ 10% in international small caps). On the 'defensive/real asset' side it holds 10% cash, 6.1% gold (GLD), and only 1.7% in intermediate Treasuries (IEF). That mix broadly lines up with this month's Market Look's 'stocks over bonds' backdrop (very little bond exposure here), and it also leans into the report's note that small caps may be starting to improve (IWM/SCZ). Where it's less aligned is the report's point that developed international has been beating emerging markets lately – OptimHybrid's single biggest weight is emerging markets, even though it also carries a sizable developed-international sleeve (IEFA plus Europe/Japan). The chart alone can't prove which sleeve drove this month's jump, but the result is clear: the portfolio's current tilts have translated into a big Month-to-Date lead over the benchmark."

---

## Style Constraints

### Plain English, newsletter tone
- Write as if explaining to a curious friend
- No jargon without plain-language context
- Same voice as the Market Look (see tone-and-style-guide.md)

### ETF references
- When mentioning ETFs, include what they hold in parentheses
- Example: "IEMG (33.3%) for emerging-markets stocks"
- This helps readers who don't know ticker symbols

### Honesty about limitations
- If the chart doesn't support a claim, say so
- Example: "The chart alone can't prove which sleeve drove this month's jump"
- Don't fabricate causation

### What NOT to include
- Trade recommendations ("buy X" or "sell Y")
- Timing suggestions ("now is the time to...")
- Price targets
- Predictions about future performance
- Claims not supported by the inputs

---

## Validation Checklist

Before finalizing, confirm:

- [ ] Opening references the Market Look naturally
- [ ] Portfolio name matches the screenshot
- [ ] MTD numbers are stated for both portfolio and benchmark
- [ ] MTD comparison is calculated correctly
- [ ] 12-month narrative is grounded in what the chart shows
- [ ] Biggest holdings are called out with percentages
- [ ] Equity/bond/cash mix is described
- [ ] Market Look themes are referenced as a published article
- [ ] Alignment AND conflicts with Market Look are noted (if both exist)
- [ ] No trade recommendations or predictions
- [ ] Plain English throughout
