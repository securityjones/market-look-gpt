# Portfolio Look Output Format Guide

## Purpose

This document defines the required structure, content, and presentation for Jeff's monthly portfolio update posts.

The Portfolio Look is a **companion piece** to the Market Look article. It has two parts:
1. **Backward-looking:** How did the portfolio perform, and why — in the context of Market Look themes?
2. **Forward-looking:** Do the recommended allocation changes align with what the Market Look is telling us?

This guide governs what the reader sees.

## Article Framing

The Portfolio Look should open with a framing sentence that:
- References the Market Look as a published article
- Sets up the two purposes: reviewing past performance AND assessing upcoming changes
- Makes it natural for Jeff to add an embedded link to "Market Look" when publishing

**Example opening:**
> "Today we want to look at our portfolio — how it performed this past month in the context of this month's Market Look, and whether the recommended changes ahead line up with what the charts are telling us."

The GPT should write this framing naturally — Jeff will add the hyperlink when publishing.

## Required Inputs

The Portfolio Look requires three inputs:

1. **Market Look article** — Provided as:
   - A URL to the published Substack article (e.g., jjfyi.substack.com/p/market-look-...)
   - An attached .md or .docx file
   - Pasted text
2. **Portfolio screenshot** — From allocatesmartly.com or similar (shows new recommendations + changes)
3. **Benchmark screenshot** — Typically 60/40, same format as portfolio

**Important:** The screenshot shows NEW recommended allocations with ± change indicators. To get the current/past allocation (what was held during the month), calculate: Displayed allocation − Change. See screenshot-reference-guide.md for details.

## Portfolio Context: TAA Strategies

The portfolios analyzed are **Tactical Asset Allocation (TAA) strategies** — rules-based approaches that Jeff follows mechanically with month-end adjustments.

**Background knowledge (not required in output):**

- **Mechanical execution:** The strategy dictates the allocation; Jeff follows it without discretion
- **Month-end rebalancing:** Changes happen at month-end based on the strategy's rules
- **Typical TAA tradeoff:** TAAs often slightly underperform in strong bull markets as the cost of avoiding big drawdowns
- **Diversification-oriented:** TAAs typically spread across asset classes rather than concentrating in one area

This is context for understanding what you're looking at — not a template for commentary. Only mention TAA characteristics if they're relevant to explaining the performance story.

## Execution Steps

Follow these steps to produce the Portfolio Look:

**Part 1 — How We Did (Backward-Looking):**
1. Extract portfolio name from screenshot (top left)
2. Extract MTD % from both portfolio and benchmark screenshots (bottom right)
3. Calculate outperformance/underperformance delta
4. Read the 12-month performance chart visually (above/below benchmark, divergence, convergence)
5. **Calculate current/past allocations** from screenshot (Displayed − Change = what we held)
6. **Categorize each ETF** using ticker-guide.md (do NOT trust shorthand labels on screenshot)
   - **Critical:** Label EM holdings as "international emerging-market stocks" — not just "emerging markets"
   - This ensures later steps correctly count them as part of "international"
7. **Calculate MTD performance** for major holdings using the procedure in "Calculating MTD Performance" section
8. **Categorize current holdings** — calculate totals for:
   - U.S. vs International (EM holdings count as international!)
   - Within International: developed vs international emerging-market
   - Within U.S.: large vs small
   - Equity vs bonds/cash/gold/commodities
9. Identify key themes from the provided Market Look
10. Connect past performance to Market Look themes (did our tilts help or hurt?)

**Part 2 — What's Changing (Forward-Looking):**
11. Extract recommended changes from screenshot (the ± change indicators)
12. Summarize key changes: what's being increased, what's being decreased
13. Assess whether changes align with or conflict with Market Look signals

## Output Structure

The output consists of two parts with **clean section headers** (no parenthetical explanations):

**Part 1 — Backward-Looking**
1. **Opening framing sentence** — references Market Look, sets up both parts
2. **How we did** — Performance summary (MTD comparison, 12-month chart narrative)
3. **Why it happened** — Attribution and Market Look reflection

**Part 2 — Forward-Looking**
4. **Recommended adjustments** — What's changing and does it align with Market Look?

**Header formatting:** Use the exact headers above as bold text on their own line. Do NOT add parenthetical explanations to headers.

Total length: Opening + 3 sections (approximately 300-400 words total)

---

## Opening Framing Sentence

One sentence that:
- Tells the reader what we're doing (reviewing performance AND assessing changes)
- References this month's Market Look
- Sets up the two-part structure

**Good examples:**
- "Today we want to look at our portfolio — how it performed this past month in the context of this month's Market Look, and whether the recommended changes ahead line up with what the charts are telling us."
- "Let's check in on the portfolio: how did it do this month, why, and do the upcoming allocation changes make sense given what the Market Look showed us?"

---

# PART 1 — HOW WE DID (Backward-Looking)

This section analyzes the allocation we HELD during the past month.

## How we did (Performance Summary)

**Section header:** Use "**How we did**" as the header (bold, own line). No parenthetical.

This section covers **what happened** — the numbers and the visual story from the chart.

### Required elements:

1. **Portfolio MTD %** — State the exact number from the screenshot
2. **Benchmark MTD %** — State the exact number from the screenshot
3. **Comparison** — Outperformed or underperformed, by how much, in plain language
4. **12-month visual narrative** — Describe the chart story:
   - Did the portfolio line stay above or below the benchmark?
   - When did it diverge or converge?
   - Where does it stand now relative to where it's been?
5. **Today's performance** (if shown) — Frame naturally: "Even with the big drop today..." not "give-back right at the end"

### Example:

> **How we did**
>
> OptimHybrid finished the month up +5.64% Month-to-Date, versus the 60/40 benchmark's +0.79%, so it ended January ahead by about 4.85 percentage points. The 12-month chart tells a pretty clean story: most of the year the portfolio line ran below the benchmark, then it started closing the gap in the back half of the year – and it finally moved above the benchmark with a sharp jump this month. Even with the big drop today (the screenshot shows Today: -1.90%), the month still delivered outsize gains.

### Key rules:
- Use the portfolio name from the screenshot (e.g., "OptimHybrid")
- State actual numbers, not vague comparisons
- Describe what you can SEE on the chart — don't invent narrative the chart doesn't show
- Say "this month" not "very late in the period"
- Plain language throughout

---

## Why it happened (Attribution & Market Look Reflection)

**Section header:** Use "**Why it happened**" as the header (bold, own line). No parenthetical.

This section explains **why** the portfolio performed the way it did, connecting to Market Look themes.

### Structure: Lead with category totals, then list ETFs

**Do NOT** list ETFs one by one without context. **DO** calculate category totals first, connect them to Market Look themes, then list ETFs as supporting detail.

Use ticker-guide.md for ETF categorization and naming. Group holdings to align with Market Look themes.

### Required elements (in this order):

1. **Category totals that connect to Market Look themes:**
   - Stocks vs Safety: "The allocation we held was about X% stocks and Y% safety"
   - U.S. vs International (within stocks): "Within stocks, roughly X% was international and Y% was U.S."
   - Developed vs Emerging (if meaningful): Split within international
   - **Connect each total to Market Look theme** as you state it

2. **ETF breakdown as supporting detail:**
   - List the specific ETFs that make up each category
   - Use plain-language names from ticker-guide.md (e.g., "international emerging-market stocks" not "emerging-market stocks")

3. **ETF attribution** (what drove performance):
   - Calculate MTD % gain for major holdings (see "Calculating MTD Performance" below)
   - **Show percentages only** — do NOT show the underlying prices (e.g., say "IEMG was up about +7.9% in January" NOT "IEMG was up about +7.9% in January (67.22 → 72.56)")
   - Which holdings contributed most to gains/losses?
   - Was it concentrated in one area or spread across several?

4. **Market Look connection** (did positioning help or hurt?):
   - Connect the performance to Market Look themes
   - Did our tilts align with what the charts showed?
   - Did that alignment/misalignment explain our outperformance or underperformance?

### Example (good — leads with category totals):

> **Why it happened**
>
> The mix we held was about 82% stocks / 18% safety (cash, a small bond slice, and gold). Within stocks, it was heavily global: roughly 62% international and 20% U.S. – with a big chunk in international emerging-market stocks (IEMG ~33%), plus international developed stocks (IEFA/EWJ/VGK) and international small-company stocks (SCZ). That's basically the same "diversification is paying" message the Market Look described: international stocks doing better than U.S. stocks lately, emerging markets doing better recently, and gold (and even commodities) staying competitive. On the month itself, the big building blocks were genuinely strong: IEMG was up about +7.9% in January; IWM was up about +5.5%; SPY was up about +1.5%; and GLD was up about +12.3% for the month. When your biggest weight is emerging markets and you've also got some gold in the mix, that's exactly the kind of setup that benefits in the current market.

### Example (bad — lists ETFs without grouping):

> "The biggest pieces were IEMG (~33.3%) for emerging-markets stocks, IEFA (~13.3%) for developed international stocks, SCZ (10%) for international small-company stocks, IWM (10%) for U.S. small-company stocks..."

The bad example lists ETFs one by one without first stating category totals or connecting to Market Look themes. It also says "emerging-markets stocks" instead of "international emerging-market stocks."

### Market Look reference style:

Reference the Market Look as a published article:

**Good:**
- "This lines up with what the Market Look showed..."
- "The Market Look noted that international has been beating U.S. stocks — our heavy IEFA weight benefited from exactly that"
- "Where we were misaligned with the Market Look was..."

**Bad:**
- "According to the analysis provided..."
- "The pasted text indicates..."
- "Based on the report above..."

---

# PART 2 — WHAT'S CHANGING (Forward-Looking)

This section assesses the RECOMMENDED allocation changes.

## Recommended adjustments (Changes Assessment)

**Section header:** Use "**Recommended adjustments**" as the header (bold, own line). No parenthetical.

This section covers **what's being recommended** and whether it aligns with Market Look signals.

### Required elements:

1. **Summarize the key recommended changes:**
   - What's being increased? What's being decreased?
   - **Simplify the numbers** — say "drops SPY and IEF to 0%" not "drops SPY to 0% (-10%) and IEF to 0% (-1.7%)"
   - Only include specific percentages for new positions or major moves
   - What's the net effect on positioning? (more/less international, more/less defensive, etc.)

2. **Assess alignment with Market Look:**
   - Do these changes move the portfolio in a direction the Market Look supports?
   - Are there any changes that conflict with Market Look signals?
   - Overall, do the recommended changes make sense given what the charts showed?

3. **Plain-language assessment** (not trade advice):
   - This is observation and analysis, not a recommendation to follow or ignore the changes
   - If the changes align well, say so
   - If there's tension with the Market Look, note it

### Example:

> **Recommended adjustments**
>
> The recommended allocation for this strategy takes a noticeable step away from "plain U.S. stock + bonds." It drops SPY and IEF to 0%, adds a commodities position of 13.3%, and nudges gold and a couple international positions a bit higher. The new mix is closer to ~70% stocks / ~30% safety, but the "safety" is mostly cash + gold + commodities, not bonds. That generally matches the Market Look's nuance: stocks still look fine versus bonds, but gold and commodities have been holding their own – and the strongest "tilt" signal has been global rather than purely U.S.

### Key rules:
- State the changes factually (what's going up, what's going down)
- **Simplify change descriptions** — combine similar changes, don't list every +/- delta
- Connect each significant change to relevant Market Look themes
- Be honest about alignment and conflicts — don't force a narrative
- This is analysis, not advice — don't tell the reader whether to follow the recommendations
- Plain language throughout

---

## Calculating MTD Performance

To calculate Month-to-Date % gain for ETFs or mutual funds, follow the procedure in **mtd-calculation-guide.md**.

The guide defines:
- Which sites to use (stockanalysis.com primary, Yahoo Finance backup)
- How to find first/last trading day closing prices
- The calculation formula
- How to report results in plain language

---

## Style Constraints

### Plain English, newsletter tone
- Write as if explaining to a curious friend
- No jargon without plain-language context
- Same voice as the Market Look (see tone-and-style-guide.md)

### Tight language
- Say "The mix we held" not "The mix we actually held"
- Say "this month" not "very late in the period"
- Say "Even with the big drop today" not "give-back right at the end"
- Avoid unnecessary qualifiers and hedge words

### Avoid jargon
- Say "portion" or "part" — NOT "sleeve" (industry jargon)
- Say "positions" or "holdings" — NOT "exposures"
- If a term wouldn't be understood by a curious non-investor, don't use it

### Correct categorization language
- **Always say "international emerging-market stocks"** — never just "emerging markets"
- This reinforces that EM is a subset of international, not a separate category
- Wrong: "less international developed, more emerging markets"
- Right: "shifts within international: less developed, more international emerging-market stocks"
- Right: "reallocates international exposure from developed to international emerging-market stocks"
- The top-level split is: U.S. vs International (then within international: developed vs international emerging-market)

### Don't create false tension in alignment analysis
- If the Market Look says "international is outpacing U.S." — a shift from developed to international emerging-market stocks is NOT tension
- Both developed and international emerging-market stocks are international — shifting between them maintains international exposure
- Only flag tension when a change actually moves AGAINST a Market Look signal (e.g., reducing total international when Market Look favors international)

### ETF references
- When mentioning ETFs, include what they hold in parentheses
- Example: "IEMG (33.3%) for emerging-markets stocks"
- This helps readers who don't know ticker symbols

### Honesty about limitations
- If the chart doesn't support a claim, say so
- Example: "The chart alone can't prove which sleeve drove this month's jump"
- Don't fabricate causation
- If recommended changes conflict with Market Look signals, say so plainly

### What NOT to include
- Trade recommendations ("buy X" or "sell Y")
- Timing suggestions ("now is the time to...")
- Price targets
- Predictions about future performance
- Claims not supported by the inputs
- Advice on whether to follow the recommended changes

---

## Validation Checklist

Before finalizing, confirm:

**Opening:**
- [ ] Opening references the Market Look naturally
- [ ] Opening sets up both backward-looking (performance) and forward-looking (changes) analysis

**Part 1 — How We Did:**
- [ ] Portfolio name matches the screenshot
- [ ] MTD numbers are stated for both portfolio and benchmark
- [ ] MTD comparison is calculated correctly
- [ ] 12-month narrative is grounded in what the chart shows
- [ ] Current/past allocations are calculated correctly (Displayed − Change)
- [ ] Biggest holdings are called out with percentages
- [ ] ETF MTD performance is looked up for attribution
- [ ] Performance is connected to Market Look themes (did tilts help or hurt?)

**Part 2 — What's Changing:**
- [ ] Key recommended changes are summarized (what's going up/down)
- [ ] Changes are assessed against Market Look signals
- [ ] Both alignment AND conflicts are noted (if both exist)
- [ ] No advice given on whether to follow the changes

**Throughout:**
- [ ] Market Look is referenced as a published article
- [ ] No trade recommendations or predictions
- [ ] Plain English throughout
