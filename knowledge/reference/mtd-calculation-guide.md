# MTD Calculation Guide

## Purpose

This document defines the procedure for calculating Month-to-Date (MTD) percentage gain for any ticker (ETF, stock, or mutual fund). Use this whenever you need to determine how a holding performed during the current month.

---

## Procedure

### Step 1: Access the price history

**Primary source — stockanalysis.com:**
- ETFs/Stocks: `https://stockanalysis.com/etf/{TICKER}/history/`
- Mutual funds: `https://stockanalysis.com/funds/{TICKER}/history/`

If stockanalysis.com doesn't have the ticker, proceed to the fallback method below.

### Step 2: Get the PREVIOUS month's last trading day close

Find the closing price for the **last trading day of the PREVIOUS month**.

- For January MTD: use December 31 close (or Dec 30/29 if 31st was a weekend/holiday)
- For February MTD: use January 31 close (or last trading day in January)
- This is your **baseline** — where the month started

### Step 3: Get the CURRENT month's most recent close

Find the closing price for the **most recent trading day in the current month**.

- Use today's close if the market has closed
- Use yesterday's close if the market is still open
- For mutual funds: price is set at end-of-day, so check that the date shown is actually current

### Step 4: Calculate the MTD gain

```
MTD % = (Current Month Close − Previous Month Close) / Previous Month Close × 100
```

---

## Examples

### ETF Example (SPY in January 2026)

1. Go to `https://stockanalysis.com/etf/SPY/history/`
2. Dec 31, 2025 close: $681.92 (previous month's last trading day)
3. Jan 30, 2026 close: $691.18 (current month's most recent)
4. MTD = (691.18 − 681.92) / 681.92 × 100 = **+1.36%**

### Mutual Fund Example (VBINX in January)

1. Go to `https://stockanalysis.com/funds/VBINX/history/`
2. Find Dec 31 close (previous month's last trading day)
3. Find the most recent January close
4. MTD = (Recent Close − Dec 31 Close) / Dec 31 Close × 100

---

## Output Format

When reporting MTD performance in analysis:

- **Round to whole percentages or one decimal** for readability
- **Use approximate language** since prices fluctuate: "up about +6%", "gained around +3%"
- **No need to show the calculation** — just state the result

**Good:**
> "IEMG was up about +6% for the month, while SPY gained around +3%..."

**Not needed:**
> "IEMG: (156.20 − 147.35) / 147.35 = +6.0%..."

### MTD Data Source Status

At the end of your output, include a brief status line indicating which method was used:

**If all tickers used primary method:**
> *MTD data: stockanalysis.com*

**If some tickers used fallback:**
> *MTD data: stockanalysis.com; fallback search used for: VBINX, XYZ*

**If any tickers couldn't be found:**
> *MTD data: stockanalysis.com; fallback search used for: VBINX; not found: ABC*

---

## Common Tickers

For reference, here are frequently used tickers and their stockanalysis URLs:

| Ticker | Type | URL |
|--------|------|-----|
| SPY | ETF | stockanalysis.com/etf/SPY/history/ |
| VOO | ETF | stockanalysis.com/etf/VOO/history/ |
| IEF | ETF | stockanalysis.com/etf/IEF/history/ |
| IEMG | ETF | stockanalysis.com/etf/IEMG/history/ |
| IEFA | ETF | stockanalysis.com/etf/IEFA/history/ |
| GLD | ETF | stockanalysis.com/etf/GLD/history/ |
| VBINX | Mutual Fund | stockanalysis.com/funds/VBINX/history/ |

---

## Notes

- **Baseline is PREVIOUS month's close:** MTD measures gain from where the month started (end of previous month), not from the first trading day of the current month
- **Consistency matters:** Use the same source and methodology for all tickers in a single analysis to ensure comparability
- **Check the dates:** Make sure you're getting the actual last day of the previous month and the actual current/recent date — don't assume
- **Market hours:** Before market close on a trading day, the "most recent" close will be the previous trading day
- **Mutual funds:** Price updates at end-of-day, so during market hours you may see yesterday's price labeled as today's

---

## Fallback Method

If stockanalysis.com doesn't have the ticker (e.g., obscure mutual funds, international securities):

1. **Search for monthly performance:** Search the web for "{TICKER} monthly performance" or "{TICKER} 1-month return"
2. **Look for pre-calculated data:** Many financial sites display "1-Month" or "MTD" performance directly on quote pages — use that if available
3. **Verify the time period:** Confirm the data is for the current month or 1-month trailing period
4. **Last resort:** If no reliable MTD data can be found, note that in your output and omit that ticker from MTD comparisons

**Known blocked sites (do not waste time on these):**
- Yahoo Finance — blocked by Content Security Policy
- Barchart — redirects to ad trackers
- StockCharts — Cloudflare bot protection
- WSJ — paywall (401 error)
