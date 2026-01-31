# Knowledge Files Guide

## Purpose

This document lists all knowledge files for Market Look GPT, their purposes, and how to use them. Follow these files rigorously, not loosely.

---

## Knowledge File Inventory

### Shared (Used by Both Tasks)

| File | Purpose |
|------|---------|
| **knowledge-guide.md** | This file — index of all knowledge files and when to use each |
| **tone-and-style-guide.md** | Voice, plain language rules, abstraction ban, editorial discipline |

### Task 1 — Market Look

| File | Purpose |
|------|---------|
| **output-format-guide.md** | Report structure, paragraph purposes, section order, validation checklist |
| **chart-reference-guide.md** ⚠️ AUTHORITATIVE | How to read and interpret every market chart type (VIX, NAHL, ratio charts) |

### Task 2 — Portfolio Look

| File | Purpose |
|------|---------|
| **portlook-output-guide.md** | Report structure, execution steps, Market Look reference style, validation checklist |
| **screenshot-reference-guide.md** ⚠️ AUTHORITATIVE | How to read portfolio screenshots, allocation calculation |
| **ticker-guide.md** | ETF categorization, naming, and grouping rules (~150 ETFs) |
| **mtd-calculation-guide.md** | How to calculate Month-to-Date performance for any ticker |

---

## Compliance Rules

### AUTHORITATIVE Files

Files marked ⚠️ AUTHORITATIVE define interpretation rules that override general knowledge:

- **chart-reference-guide.md** — Defines thresholds, crossover rules, and signal interpretation for all market charts
- **screenshot-reference-guide.md** — Defines how to extract data from portfolio screenshots

**If these files conflict with your general knowledge, the guide wins.**

### Key Reminders

**Task 1 (Market Look):**
- The chart contains the history
- Compare the right edge (now) to 4-5 bars left (one month ago)
- READ what you see, don't assume

**Task 2 (Portfolio Look):**
- Screenshot shows NEW recommended allocations
- Calculate current/past allocations: Displayed − Change = what we held
- Use ticker-guide.md for ETF categorization (don't trust screenshot labels)
- Use mtd-calculation-guide.md for performance attribution
- Reference the Market Look as a published article

---

## When to Consult Each File

### Before Starting

| Task | Consult First |
|------|---------------|
| Market Look | chart-reference-guide.md (interpretation rules) |
| Portfolio Look | screenshot-reference-guide.md (data extraction), ticker-guide.md (ETF lookup) |

### During Execution

| Need | Consult |
|------|---------|
| Report structure | output-format-guide.md (Task 1) or portlook-output-guide.md (Task 2) |
| Tone/language check | tone-and-style-guide.md |
| ETF categorization | ticker-guide.md |
| MTD % calculation | mtd-calculation-guide.md |

### Before Finalizing

| Task | Consult |
|------|---------|
| Market Look | Validation checklist in output-format-guide.md |
| Portfolio Look | Validation checklist in portlook-output-guide.md |
