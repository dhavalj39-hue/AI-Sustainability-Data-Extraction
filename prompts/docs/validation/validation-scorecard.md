# Validation Scorecard — 225-Point Head-to-Head

> Full validation of both extractions against ExxonMobil 2025 Sustainability Report source document.
> Primary source: Performance Data Table pp. 67–69. Secondary: full document.
>
> **Verdict key:** ✅ CORRECT | ❌ WRONG | 🟡 PARTIAL | ⬜ MISSING | ➖ N/A (correct NULL)

---

## Section 1 — Report Metadata (12 points)

| Field | Source Value | ChatGPT | Verdict A | Claude | Verdict B |
|-------|-------------|---------|-----------|--------|-----------|
| Report Title | 2025 Sustainability Report | 2025 Sustainability Report | ✅ | 2025 Sustainability Report | ✅ |
| Company Name | Exxon Mobil Corporation | ExxonMobil | 🟡 | Exxon Mobil Corporation | ✅ |
| Period Start | January 1, 2024 | 2024-01-01 | ✅ | January 1, 2024 | ✅ |
| Period End | December 31, 2024 | 2024-12-31 | ✅ | December 31, 2024 | ✅ |
| Publication Date | April 30, 2025 | 2025-04 | 🟡 | April 30, 2025 | ✅ |
| Report Version | NULL | NULL | ✅ | NULL | ✅ |
| Applicable Standards | 9 standards | 3 standards | 🟡 | All 9 standards | ✅ |
| Assurance Provider | Lloyd's Register QA Ltd | Lloyd's Register QA Ltd | ✅ | Lloyd's Register QA Ltd | ✅ |
| Assurance Level | Reasonable (Ipieca core elements) | Reasonable | 🟡 | Reasonable + full scope qualifier | ✅ |
| Acquisition coverage | Denbury Nov 2023; Pioneer May 2024 | Not extracted | ⬜ | Both dates captured | ✅ |
| Data as-of dates | Safety: Mar 12; Water: Mar 24 | Not extracted | ⬜ | Both captured | ✅ |
| GHG/energy caveat | In Advancing Climate Solutions Report | Not extracted | ⬜ | Explicitly noted | ✅ |

**S1 Score: ChatGPT 4/12 (33%) | Claude 12/12 (100%)**

---

## Section 2 — Safety KPIs (42 points — selected rows shown)

| KPI | Year | Source (p.68) | ChatGPT | Verdict A | Claude | Verdict B |
|-----|------|---------------|---------|-----------|--------|-----------|
| Fatalities — Employees | 2024 | 0 | NULL | ⬜ | 0 | ✅ |
| Fatalities — Employees | 2023 | 1 | NULL | ⬜ | 1 | ✅ |
| Fatalities — Employees | 2022 | 0 | NULL | ⬜ | 0 | ✅ |
| Fatalities — Contractors | 2024 | 1 | NULL | ⬜ | 1 | ✅ |
| Fatalities — Contractors | 2022 | 3 | NULL | ⬜ | 3 | ✅ |
| FAR — Total WF | 2024 | 0.003/1M hrs | NULL | ⬜ | 0.003/1M hrs | ✅ |
| FAR — Total WF | 2022 | 0.009/1M hrs | NULL | ⬜ | 0.009/1M hrs | ✅ |
| LTIR — Total WF | 2024 | 0.02/200K hrs | 0.02 | ✅ | 0.02 | ✅ |
| LTIR — Total WF | 2023 | 0.02/200K hrs | 0.02 | ✅ | 0.02 | ✅ |
| LTIR — Total WF | 2022 | 0.02/200K hrs | NULL | ⬜ | 0.02 | ✅ |
| LTIR — Employees | 2024 | 0.03/200K hrs | NULL | ⬜ | 0.03 | ✅ |
| LTIR — Employees | 2023 | 0.01/200K hrs | NULL | ⬜ | 0.01 | ✅ |
| LTIR — Contractors | 2024 | 0.02/200K hrs | NULL | ⬜ | 0.02 | ✅ |
| TRIR — Total WF | 2024 | 0.17/200K hrs | NULL | ⬜ | 0.17 | ✅ |
| TRIR — Employees | 2024 | 0.13/200K hrs | NULL | ⬜ | 0.13 | ✅ |
| TRIR — Contractors | 2024 | 0.20/200K hrs | NULL | ⬜ | 0.20 | ✅ |
| PS Tier 1 Events | 2024 | 61 | NULL | ⬜ | 61 | ✅ |
| PS Tier 1 Events | 2023 | 55 | NULL | ⬜ | 55 | ✅ |
| PS Tier 1 Events | 2021 | 44 | NULL | ⬜ | 44 | ✅ |
| Near-Miss Count | — | NULL (not in report) | NULL | ➖ | NULL | ➖ |
| Work Hours Total | — | NULL (not disclosed) | NULL | ➖ | NULL (flagged) | ✅ |

**S2 Score: ChatGPT 8/42 (19%) | Claude 42/42 (100%)**

---

## Section 4 — Environmental KPIs — Critical Errors (selected)

| KPI | Year | Source (p.67) | ChatGPT | Verdict A | Claude | Verdict B |
|-----|------|---------------|---------|-----------|--------|-----------|
| **SOx Emitted** | 2024 | **0.05 M MT** | **25%** ❌ | **❌ WRONG** | 0.05 M MT | ✅ |
| **NOx Emitted** | 2024 | **0.11 M MT** | **25%** ❌ | **❌ WRONG** | 0.11 M MT | ✅ |
| **VOC Emitted** | 2024 | **0.13 M MT** | **25%** ❌ | **❌ WRONG** | 0.13 M MT | ✅ |
| Freshwater Withdrawn | 2024 | 480 M m³ | NULL | ⬜ | 480 M m³ | ✅ |
| Freshwater Withdrawn | 2023 | 440 M m³ | NULL | ⬜ | 440 M m³ | ✅ |
| Freshwater Consumption | 2024 | 330 M m³ | NULL | ⬜ | 330 M m³ | ✅ |
| HC Spills — Count | 2024 | 441 | NULL | ⬜ | 441 | ✅ |
| HC Spills — Volume | 2024 | 4.8 '000 BBL | NULL | ⬜ | 4.8 '000 BBL | ✅ |
| Haz Waste Gen — Ops | 2024 | 0.4 M MT | NULL | ⬜ | 0.4 M MT | ✅ |
| Non-Haz Waste Gen — Ops | 2024 | 1.5 M MT | NULL | ⬜ | 1.5 M MT | ✅ |
| **Env Fines** | 2024 | **$0.001B ($1M)** | **NULL** | **❌ WRONG** | $0.001B = $1M | ✅ |
| **Env Fines** | 2022 | **$0.002B ($2M)** | **NULL** | **❌ WRONG** | $0.002B = $2M | ✅ |
| Env Expenditures | 2024 | $9.0B | NULL | ⬜ | $9.0B = $9,000,000,000 | ✅ |
| Water recycled Permian | 2024 | 98% | 98% | ✅ | 98% (DUPLICATE+SCOPE flags) | ✅ |

> ⚠️ **The 25% error explained:** The value "~25% reduction in NOx/SOx/VOC from 2016–2024" appears in narrative text (pp.4, 29). The actual emission quantities are in the data table (p.67). ChatGPT extracted the narrative trend as if it were the measured value — a fundamental data identification failure.

**S4 Score: ChatGPT 7/45 (16%) | Claude 45/45 (100%)**

---

## Section 6 — Regulatory & Compliance

| Item | Source | ChatGPT | Verdict A | Claude | Verdict B |
|------|--------|---------|-----------|--------|-----------|
| ISO 14001 status | COMPLIANT (p.17) | Listed (no status) | 🟡 | COMPLIANT + evidence | ✅ |
| ISO 45001 status | COMPLIANT (p.44) | Not extracted | ⬜ | COMPLIANT | ✅ |
| World Bank Flaring | PARTIAL (p.28) | Not extracted | ⬜ | PARTIAL — nuanced | ✅ |
| EU REACH, GHS | COMPLIANT (p.41) | Not extracted | ⬜ | Both COMPLIANT | ✅ |
| Env Fines 2024 | $1,000,000 | NULL | ❌ | $1,000,000 | ✅ |
| Env Fines 2022 | $2,000,000 | NULL | ❌ | $2,000,000 | ✅ |
| Regulatory violations | NULL | NULL | ✅ | NULL | ✅ |
| EITI countries 2024 | 17 | Not extracted | ⬜ | 17 (5-year series) | ✅ |

**S6 Score: ChatGPT 5/14 (36%) | Claude 14/14 (100%)**

---

## Section 7 — Targets (critical error)

| Target | Source | ChatGPT | Verdict A | Claude | Verdict B |
|--------|--------|---------|-----------|--------|-----------|
| Net zero operated 2050 | Target (p.70) | Not extracted | ⬜ | Captured | ✅ |
| **Permian water >90% by 2030** | **>90% by 2030; 87% current (p.26)** | **500M lbs (WRONG metric)** | **❌ WRONG** | >90% by 2030; 87% current; ON TRACK | ✅ |
| Lower-emission investments | $30B by 2030 (p.11) | $30,000,000,000 | ✅ | Up to $30B — correct | ✅ |
| Advanced recycling 500M lbs | Announced (p.39) | 500M lbs | ✅ | 500M lbs — correct | ✅ |
| LTIR industry-leading | 0.02 maintained (p.43) | Not extracted | ⬜ | Maintained — YES | ✅ |
| Zero transport fatalities | 0 (2017–2024) (p.41) | Not extracted | ⬜ | ACHIEVED | ✅ |

**S7 Score: ChatGPT 2/17 (12%) | Claude 17/17 (100%)**

---

## Overall Results

| | ChatGPT | Claude |
|--|---------|--------|
| **Total correct** | 48/225 | 225/225 |
| **Completeness** | 21% | 100% |
| **Factual errors** | 3 confirmed | 0 |
| **Data quality flags** | 8/24 | 24/24 |
| **5-year time series** | Rarely | Always |
| **Page citations** | Rarely | Every row |
| **Winner** | | **🏆 Claude** |

---

## Confirmed Factual Errors in ChatGPT

| # | Error | Source Truth | Impact |
|---|-------|-------------|--------|
| 1 | SOx/NOx/VOC = "25%" | Actual values: 0.05/0.11/0.13 M MT (p.67) | Would cause incorrect compliance calculations |
| 2 | Permian water target = "500M lbs recycling" | Actual: >90% water recycling by 2030 (p.26) | Wrong KPI entirely — different program |
| 3 | Env fines = NULL (all years) | Actual: $1M–$2M per year visible on p.67 | Financial data suppressed — audit risk |

---

*Validated against source: ExxonMobil 2025 Sustainability Report — Performance Data Table pp. 67–69*
*Validation completed: May 2026*
