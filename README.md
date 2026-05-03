# AI-Based Data Extraction Project

## Objective
Compare how well ChatGPT and Claude extract structured HSE data 
from a real sustainability report — same prompt, same document, 
scored against the source.

**Source:** ExxonMobil 2025 Sustainability Report (71 pages)  
**Models:** ChatGPT (GPT-4o) vs Claude (Sonnet 4.5)  
**Data points validated:** 225 across 10 sections

---

## Progress Log

### ✅ Day 1 — First Attempt (Raw Prompt)
- Gave both models a basic unstructured prompt
- Spotted first red flag: ChatGPT showed SOx/NOx/VOC = "25%" 
  (should be 0.05/0.11/0.13 million metric tons)
- Claude got the data table values right; ChatGPT seemed to 
  only read the Executive Summary
- Decided to build a proper schema for Day 2

### ✅ Day 2 — Built 10-Section Schema, Re-ran Both Models
- Designed structured extraction prompt with mandatory NULL rules, 
  page citations, 5-year time series requirement
- Re-ran both models with the same schema
- Gap got clearer: Claude followed the schema completely; 
  ChatGPT still missed the performance data table (pp. 67–69)
- Found 2 more errors in ChatGPT: wrong water target metric, 
  environmental fines showing NULL when data exists

### ✅ Day 3 — Validated All 225 Data Points
- Cross-checked every extracted value against source document
- Final score: ChatGPT 48/225 (21%) vs Claude 225/225 (100%)
- 3 confirmed factual errors in ChatGPT output
- Root cause: ChatGPT appears to have read Executive Summary only

---

## Final Scorecard

| Section | ChatGPT | Claude |
|---------|---------|--------|
| Safety KPIs | 8/42 (19%) | 42/42 (100%) |
| Environmental KPIs | 7/45 (16%) | 45/45 (100%) |
| Regulatory/Compliance | 5/14 (36%) | 14/14 (100%) |
| Programs & Initiatives | 2/27 (7%) | 27/27 (100%) |
| Workforce Data | 5/28 (18%) | 28/28 (100%) |
| **TOTAL** | **48/225 (21%)** | **225/225 (100%)** |

---

## Files

- `prompts/` → 10-section HSE extraction prompt (reusable)
- `docs/` → daily progress notes (Day 1, 2, 3)
- `validation/` → 225-point scorecard vs source document

---

## Key Finding

> ChatGPT's output *looked* professional but contained 3 factual errors.  
> The most dangerous: SOx/NOx/VOC shown as "25%" instead of actual  
> million metric ton values — plausible enough to miss in a quick review.

---

*Personal learning project — May 2026*
