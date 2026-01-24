# Market Look GPT

A custom GPT for analyzing stock charts and generating structured market analysis reports for Jeff's Substack.

## Overview

Market Look GPT takes stock chart images as input and produces monthly market analysis reports with:
- Executive Summary (3 paragraphs: what changed, context, segment snapshot)
- What Should We Do? (portfolio posture guidance, non-prescriptive)
- Detailed Chart Analysis (per-chart breakdown with signal strength ratings)

## Project Structure

```
├── docs/                       # Documentation and planning
│   ├── plan.md                 # Project roadmap
│   ├── progress.md             # Development log
│   └── design/                 # Design documents
│
├── knowledge/                  # GPT knowledge files
│   └── reference/
│       ├── tone-and-style-guide.md    # Voice, tone, editorial rules
│       ├── output-format-guide.md     # Report structure requirements
│       └── chart-reference-guide.md   # Chart interpretation rules
│
├── samples/
│   ├── charts/                 # Sample chart images (PNG)
│   └── outputs/                # Example/aspirational outputs
│
├── gpt-config/                 # GPT configuration
│   ├── instructions.md         # System instructions (V2)
│   └── conversation-starters.md
│
├── .gitignore
└── README.md
```

## Knowledge Files

| File | Purpose |
|------|---------|
| tone-and-style-guide.md | Defines conversational voice, "we" framing, plain language rules, editorial discipline |
| output-format-guide.md | Specifies exact report structure, section order, paragraph requirements |
| chart-reference-guide.md | SMA framework for ratio charts, VIX thresholds, NAHL interpretation rules |

## Sample Charts

- **$VIX** — Volatility Index
- **$NAHL** — New Highs vs New Lows
- **IJR_VOO** — Small vs Large Cap
- **QQQ_RSP** — Concentration Proxy
- **VOO_IEF** — Stocks vs Bonds
- **VOO_VEA** — US vs International Developed
- **VEA_VWO** — Developed vs Emerging International

## Development Status

✅ **Phase 1: Foundation** — Complete

✅ **Phase 2: GPT Configuration** — Complete
- [x] System instructions drafted
- [x] Conversation starters created
- [x] V1 deployed to OpenAI

🔄 **Phase 3: Testing & Iteration** — In Progress
- [x] V1 tested with sample charts
- [x] Issues identified and documented
- [x] V2 revisions applied
- [ ] V2 testing pending
