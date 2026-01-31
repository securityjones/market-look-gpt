# Market Look GPT

A custom GPT for analyzing stock charts and portfolio screenshots to generate structured market analysis and portfolio update reports for Jeff's Substack.

## Overview

Market Look GPT has two capabilities:

### 1. Market Look Report
Analyzes stock chart images and produces monthly market analysis reports with:
- Executive Summary (3 paragraphs: what changed, context, chart-by-chart snapshot)
- What Should We Do? (portfolio posture guidance, non-prescriptive)
- Detailed Chart Analysis (per-chart breakdown with signal strength ratings)

### 2. Portfolio Look Report
Analyzes portfolio screenshots and produces companion articles with:
- Performance summary (MTD comparison vs 60/40 benchmark, 12-month chart narrative)
- Attribution (which holdings drove gains/losses, with MTD lookup)
- Market Look connection (alignment/conflicts with market themes)
- Recommended changes assessment (do new allocations align with Market Look?)

**Note:** Portfolios are assumed to be TAA (Tactical Asset Allocation) strategies with mechanical month-end execution.

## Project Structure

```
├── docs/                       # Documentation and planning
│   ├── plan.md                 # Project roadmap
│   ├── progress.md             # Development log
│   └── design/                 # Design documents
│       └── portfolio-look-design.md
│
├── knowledge/                  # GPT knowledge files
│   └── reference/
│       ├── tone-and-style-guide.md      # Voice, tone, editorial rules (shared)
│       ├── output-format-guide.md       # Market Look report structure
│       ├── chart-reference-guide.md     # Market chart interpretation rules
│       ├── portlook-output-guide.md     # Portfolio Look report structure
│       └── screenshot-reference-guide.md # Portfolio screenshot interpretation
│
├── samples/
│   ├── charts/                 # Sample market chart images (PNG)
│   ├── portcharts/             # Sample portfolio screenshots (PNG)
│   └── outputs/                # Example/aspirational outputs
│
├── gpt-config/                 # GPT configuration
│   ├── instructions.md         # System instructions
│   └── conversation-starters.md
│
├── .gitignore
└── README.md
```

## Knowledge Files

### Shared
| File | Purpose |
|------|---------|
| tone-and-style-guide.md | Conversational voice, "we" framing, plain language rules, editorial discipline |
| knowledge-guide.md | Index of all knowledge files and when to use each |

### Market Look (Task 1)
| File | Purpose |
|------|---------|
| output-format-guide.md | Report structure, section order, paragraph requirements |
| chart-reference-guide.md | SMA framework for ratio charts, VIX thresholds, NAHL interpretation rules |

### Portfolio Look (Task 2)
| File | Purpose |
|------|---------|
| portlook-output-guide.md | Report structure, execution steps, validation checklist |
| screenshot-reference-guide.md | Screenshot layout, allocation calculation (Displayed − Change = current) |
| ticker-guide.md | ETF categorization and naming (~150 ETFs pre-categorized) |
| mtd-calculation-guide.md | How to calculate Month-to-Date performance (stockanalysis.com primary) |
## Market Charts (Task 1)

**Tier 1 — Macro Conditions:**
- **$VIX** — Volatility Index
- **$NAHL** — New Highs vs New Lows

**Tier 2 — Big Allocation Questions:**
- **VOO:IEF** — Stocks vs Bonds
- **VOO:IAU** — Stocks vs Gold
- **VOO:BCI** — Stocks vs Commodities
- **VOO:VEA** — US vs International Developed
- **VOO:VWO** — US vs Emerging Markets

**Tier 3 — Drilling Down:**
- **VOO:IJR** — Large vs Small Cap (within US)
- **VOO:QQQ** — Broad Market vs Tech-Heavy (within US)

## Portfolio Screenshots (Task 2)

From allocatesmartly.com or similar:
- Portfolio screenshot (name, holdings, MTD return, performance chart)
- Benchmark screenshot (60/40 for comparison)

## Development Status

✅ **Phase 1-4: Market Look** — Complete & Deployed

✅ **Phase 5: Portfolio Look** — Complete (pending deployment)
- [x] Output format designed (two-part structure: backward + forward-looking)
- [x] Knowledge files created (portlook-output-guide, screenshot-reference-guide, ticker-guide, mtd-calculation-guide)
- [x] TAA strategy context added
- [x] Language and categorization rules refined
- [ ] Deploy updated GPT to OpenAI

✅ **Phase 7-8: Market Look Enhancements** — Complete
- Expanded to 9 charts (added VOO:IAU, VOO:BCI)
- Flexible chart inputs (3 required, 6 optional)

🔜 **Phase 6: Help/Usage Task** — Next
🔜 **Phase 7: Help/Usage Task**

## ⚠️ Model Requirement

**Market Look GPT requires a thinking-enabled model.**

**Recommended:** ChatGPT 5.2 Thinking (tested and confirmed working)

Non-thinking models fail at chart interpretation — they guess rather than read visual data. Thinking models accurately read charts and follow knowledge file rules.
