---
title: M3-Obj-3-1 - Vertical Analysis (Common-Sizing)
created: 2026-08-25
date: 2026-08-25
tags:
  - FSA
  - M3
  - Objective-3-1
  - Vertical-Analysis
aliases:
  - vertical-analysis
  - common-sizing
  - common-size-statements
---

# Learning Objective 3.1

## Perform Vertical Analysis and calculate common-sizing ratio metrics to evaluate a company's internal structural mix

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc.
> Throughout this note we continue our Tesla running example, now spanning three fiscal years (2023–2025), drawn from the FY2023 and FY2025 Form 10-K filings. All figures in millions of USD.

**Condensed Balance Sheet ($M):**

| Line Item | Dec 31, 2025 | Dec 31, 2024 | Dec 31, 2023 |
|-----------|-----:|-----:|-----:|
| Cash + short-term investments | $44,059 | $36,563 | $29,094 |
| Accounts receivable, net | $4,576 | $4,418 | $3,508 |
| Inventory | $12,392 | $12,017 | $13,626 |
| Property, plant & equipment, net | $40,643 | $35,836 | $29,725 |
| All other assets | $36,136 | $33,236 | $30,665 |
| **Total Assets** | **$137,806** | **$122,070** | **$106,618** |
| Accounts payable | $13,371 | $12,474 | $14,431 |
| All other liabilities | $41,570 | $35,916 | $28,578 |
| **Total Liabilities** | **$54,941** | **$48,390** | **$43,009** |
| **Total Equity** (incl. NCI & redeemable NCI) | **$82,865** | **$73,680** | **$63,609** |

*Total equity here includes both noncontrolling interests in subsidiaries and the mezzanine *redeemable* noncontrolling interests, so that Total Liabilities + Total Equity reconciles exactly to Total Assets. (See [[M2-Obj-2-1]] for the distinction between these equity components.)*

**Condensed Income Statement ($M):**

| Line Item | 2025 | 2024 | 2023 |
|-----------|-----:|-----:|-----:|
| **Total Revenues** | **$94,827** | **$97,690** | **$96,773** |
| Cost of revenues | $77,733 | $80,240 | $79,113 |
| **Gross Profit** | **$17,094** | **$17,450** | **$17,660** |
| R&D | $6,411 | $4,540 | $3,969 |
| SG&A | $5,834 | $5,150 | $4,800 |
| Restructuring & other | $494 | $684 | — |
| **Operating Income** | **$4,355** | **$7,076** | **$8,891** |
| **Net Income** | **$3,855** | **$7,153** | **$14,974** |
| Cash Flow from Operations | $14,747 | $14,923 | $13,256 |

---

### I. Core Philosophy of Vertical Analysis (Common-Sizing)

> [!info] What Is Vertical Analysis?
> **Vertical analysis** — also called **common-sizing** or preparing **common form (percentage) statements** — restates every line on a financial statement as a **percentage of one designated base figure** for the same period.
>
> Think of it like comparing two people's monthly spending. Person A earns \$100,000 and spends \$900 on groceries; Person B earns \$40,000 and spends \$600. In dollars, A spends more. As a *percentage of income*, B spends far more (1.5% vs. 0.9%). Vertical analysis does the same for financial statements: it strips away absolute size so structure and priorities become visible.
>
> The name "**vertical**" comes from the top-to-bottom columnar layout of financial statements — each item is measured against the base at the top of its own column.

**The mechanics are simple:**

$$\text{Common-Size \%} = \frac{\text{Any Line Item}}{\text{Base Figure}} \times 100$$

Every item on the statement is divided by a single **common base**, which always represents 100%. Two bases dominate practice:

| Statement | Base (= 100%) | Logic |
|-----------|---------------|-------|
| Balance Sheet | **Total Assets** | Every asset, liability, and equity claim is funded by (or competes for) the asset base |
| Income Statement | **Net Sales (Total Revenue)** | Every cost is incurred to generate the revenue dollar |

> [!info] What Is "Net Sales"?
> **Net sales** — the income-statement base used for vertical analysis — is the company's **total revenue** after returns, allowances, and discounts: the actual proceeds recognized from selling goods and services, before any expenses are deducted. On a multiple-step income statement, **net sales** is the **top line** — it *is* **total revenue**. (The label the company uses may be "Net sales," "Revenues," or "Total revenues"; in every case it is the income statement's total revenue figure.)
>
> For Tesla, net sales = total revenue = **$94,827M (2025)**, shown as the "Total Revenues" line of the condensed income statement above. Because vertical analysis expresses every expense as a percentage of this figure, net sales is always set to **100%** on a common-size income statement.

> [!tip] Why Analysts Use It
> 1. **Internal structural analysis** — how the firm allocates its capital across asset classes, period over period
> 2. **Cross-company comparison** — compare firms of vastly different sizes head-to-head (a \$138B giant vs. a \$2B competitor)
> 3. **Trend detection** — subtle, gradual structural shifts that hide inside growing absolute dollar amounts

---

### II. The Common-Size Balance Sheet

On a common-size balance sheet, the designated base is **Total Assets** (mathematically equivalent to Total Liabilities + Equity). Each item becomes a share of the total resource pool.

#### Tesla's Common-Size Balance Sheets (% of Total Assets)

| Line Item | 2025 | 2024 | 2023 |
|-----------|-----:|-----:|-----:|
| Cash + short-term investments | **32.0%** | 30.0% | 27.3% |
| Accounts receivable, net | 3.3% | 3.6% | 3.3% |
| Inventory | **9.0%** | 9.8% | 12.8% |
| Property, plant & equipment, net | 29.5% | 29.4% | 27.9% |
| All other assets | 26.2% | 27.2% | 28.8% |
| **Total Assets** | **100%** | **100%** | **100%** |
| Accounts payable | 9.7% | 10.2% | 13.5% |
| All other liabilities | 30.2% | 29.4% | 26.8% |
| **Total Liabilities** | **39.9%** | **39.6%** | **40.3%** |
| **Total Equity** | **60.1%** | **60.4%** | **59.7%** |

*Percentages may not sum precisely due to rounding.*

#### Reading the Structure — Detective Applications

**Key structural asset metrics** reveal subtle changes invisible in raw dollar figures:

- **Cash + investments as % of total assets:** Rising from 27.3% → 32.0%. Tesla is holding an ever-larger share of its resource pool in liquid form — nearly one-third of every asset dollar is now cash-like liquidity.
- **Inventory as % of total assets:** Falling sharply from 12.8% → 9.0%. This is the mirror image of a distress signal: no involuntary inventory buildup here. Tesla generates more sales from proportionally less inventory — improving inventory efficiency. (Contrast: a company whose inventory share balloons toward half its assets is signaling unsold goods piling up — a sales slowdown.)
- **Accounts receivable as % of total assets:** Stable around 3–4%. Credit extension to customers is steady relative to the business size — a rising AR share would have suggested reliance on credit sales or collection struggles.
- **PP&E as % of total assets:** Creeping up from 27.9% → 29.5%. Over a multi-year horizon this means the business is becoming slightly **more capital-intensive** — more fixed costs, higher operating leverage, potentially more volatile earnings. Watch how this connects to the income statement below.

**Structural liability and equity metrics:**

- **Debt-to-assets ratio (Total liabilities ÷ Total assets):** Remarkably stable at ~40% (40.3% → 39.6% → 39.9%). Per the classic interpretation: if liabilities fund 40% of assets, those assets could lose up to 60% of their value before lenders' claims would be impaired. That 60-point buffer is the **equity cushion**.
- **Capitalization mix:** With equity consistently funding ~60% of the balance sheet — and most of it paid-in capital plus retained earnings rather than debt — Tesla's permanent capital structure remains conservative despite its growth spending.

> [!tip] The Pattern-Hunting Mindset
> Single-year percentages tell you *what* the structure is. Multi-year percentages tell you *where it is heading*. Always read common-size statements left to right, hunting for gradual drift — that is where early warnings live.

---

### III. The Common-Size Income Statement

On a common-size income statement, the base is **Net Sales (Total Revenue)** = 100%. Recasting expenses as percentages of sales exposes the underlying cost structure and the efficiency of converting revenue into profit.

```
                     ┌──────────────────────────────────────┐
                     │          NET SALES = 100%            │
                     └──────────────────┬───────────────────┘
                                        │
           ┌────────────────────────────┼────────────────────────────┐
           ▼                            ▼                            ▼
┌──────────────────────┐     ┌──────────────────────┐     ┌──────────────────────┐
│ GROSS PROFIT MARGIN  │     │ OPERATING MARGIN     │     │  NET PROFIT MARGIN   │
│                      │     │                      │     │                      │
│   (Sales - COGS)     │     │  Operating Profit    │     │     Net Income       │
│  ─────────────       │     │  ────────────────    │     │  ─────────────       │
│       Sales          │     │        Sales         │     │       Sales          │
└──────────────────────┘     └──────────────────────┘     └──────────────────────┘
```

#### Tesla's Common-Size Income Statement (% of Revenue)

| % of Revenue | 2025 | 2024 | 2023 |
|--------------|-----:|-----:|-----:|
| Cost of revenues | 82.0% | 82.2% | 81.7% |
| **Gross Profit Margin** | **18.0%** | **17.9%** | **18.2%** |
| R&D | **6.8%** | 4.6% | 4.1% |
| SG&A | 6.2% | 5.3% | 5.0% |
| Restructuring & other | 0.5% | 0.7% | — |
| **Operating Profit Margin** | **4.6%** | **7.2%** | **9.2%** |
| **Net Profit Margin** | **4.1%** | **7.3%** | **15.5%*** |
| **Cash Flow Margin** (CFO ÷ Revenue) | 15.6% | 15.3% | 13.7% |

*\*2023's 15.5% net margin was inflated by a one-time \$6.5B deferred tax benefit — see the caution below.*

#### The Four Stages of Measurement

- **Gross profit margin** = (Revenue − COGS) ÷ Revenue. Measures profitability from core product sales before overhead, i.e., the ability to control manufacturing costs and pass price changes to customers. Because COGS% and gross margin are complements, they always sum to exactly 100% (COGS ~82% ⇔ GM ~18%).
- **Operating profit margin** = Operating income ÷ Revenue. Excludes interest and taxes, isolating management's core operating prowess from financing strategy and tax jurisdiction.
- **Net profit margin** = Net income ÷ Revenue. The bottom line — reflects *everything*, including items outside management's operational control.
- **Cash flow margin** = CFO ÷ Revenue. Because net income is subject to non-cash accruals, estimates, and timing choices, this margin checks **earnings quality**: the true ability to turn sales into cold, hard cash.

#### Interpreting Tesla's Three-Year Trend

| Metric | 2023 | 2024 | 2025 | Analytical Interpretation |
|--------|------|------|------|---------------------------|
| Gross margin | 18.2% | 17.9% | 18.0% | Rock-steady cost structure — pricing cuts offset by manufacturing efficiency |
| Operating margin | 9.2% | 7.2% | 4.6% | Halved while gross margin held flat — the squeeze came entirely from operating expenses |
| R&D % of revenue | 4.1% | 4.6% | 6.8% | Aggressive AI/robotics investment; grew even as revenue shrank |
| SG&A % of revenue | 5.0% | 5.3% | 6.2% | Overhead did not scale down with sales |
| Net margin | 15.5% | 7.3% | 4.1% | Followed operating margin down once 2023's one-time tax benefit is stripped out |
| Cash flow margin | 13.7% | 15.3% | 15.6% | *Earnings quality check:* operations kept converting 14–16 cents of each sales dollar into cash throughout — the cash engine never stalled even as accrual profits compressed |

> [!warning] One Number, Two Stories
> Vertical analysis exposed what raw dollars hid: between 2023 and 2025, revenue barely moved (−2%) yet operating margin fell by half. The cause is visible only in percentages — **R&D alone rose from 4.1% to 6.8% of revenue**, consuming roughly 2.7 extra cents of every sales dollar. No single absolute dollar figure would have made this trade-off (deliberate AI investment vs. shrinking auto profitability) this legible.
>
> Also remember from [[M2-Obj-2-2]]: 2023's net margin benefited from regulatory credits (1.9% of revenue at nearly pure margin) and the one-time tax benefit. Vertical analysis makes such distortions easier to spot — but you must still know *what* sits inside each percentage.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Vertical analysis** | Restating each financial statement line as a percentage of a single base figure for the same period |
| **Common-sizing** | Synonym for vertical analysis; produces "common form" (percentage) statements |
| **Common base** | The denominator representing 100% — Total Assets (balance sheet) or Net Sales (income statement) |
| **Debt-to-assets ratio** | Total liabilities ÷ total assets; measures credit protection available to lenders |
| **Equity cushion** | The percentage of assets funded by owners; the loss-absorbing buffer before creditors are impaired |
| **Gross profit margin** | (Sales − COGS) ÷ Sales; core product profitability before overhead |
| **Operating profit margin** | Operating income ÷ Sales; core efficiency excluding financing and taxes |
| **Net profit margin** | Net income ÷ Sales; all-in bottom-line profitability |
| **Cash flow margin** | CFO ÷ Sales; earnings-quality check on accrual-based profits |
| **Capital-intensive** | A structure with heavy fixed assets relative to total assets; implies higher fixed costs and operating leverage |

---

> [!danger] Red Flags — What Common-Sizing Reveals (and Hides)
> **Reveals:**
> - **Involuntary inventory buildup** — inventory share climbing quarter after quarter signals unanticipated sales slowdown
> - **Credit-driven growth** — rising AR share suggests loosening credit terms or collection trouble
> - **Margin squeeze** — stable gross margin + falling operating margin = overhead or investment spend outgrowing revenue
> - **Stealth capital-intensity creep** — slowly rising PP&E share quietly raises fixed costs and earnings volatility
>
> **Hides:**
> - **Absolute scale** — a 1% improvement on \$95B of revenue (\~\$950M) dwarfs a 5% improvement on \$500M (\$25M). Percentages normalize away magnitude
> - **Composition within lines** — "All other liabilities at 30%" says nothing about whether it is deferred revenue (healthy) or overdue payables (stretched)
> - **One-shot distortions** — a single unusual item (like 2023's tax benefit) can paint a whole column a misleading color
>
> Rule: common-size first for *structure*, then zoom back into dollars for *materiality*.

---

### Review Questions

> [!question]- 1. What base figure is used for a common-size balance sheet, and why?
> **Total Assets** (= Total Liabilities + Equity). Every asset, liability, and equity account represents a claim on or allocation of the same finite resource pool, so expressing all items against that single pool reveals the internal structural mix.

> [!question]- 2. Tesla's inventory fell from 12.8% to 9.0% of total assets over 2023–2025. Why is this a *positive* structural signal rather than a warning?
> Because the danger sign is an *involuntary buildup*: inventory share rising while sales slow. Tesla's inventory share *fell* while unit volumes stayed substantial — meaning proportionally less capital is tied up supporting each revenue dollar. Rising share = possible demand trouble; falling share = improving efficiency (context and direction matter).

> [!question]- 3. Tesla's gross margin was essentially flat (~18%) across 2023–2025, yet operating margin halved from 9.2% to 4.6%. What does this tell you analytically?
> The deterioration originated entirely below gross profit — in operating expenses. R&D rose from 4.1% to 6.8% of revenue and SG&A from 5.0% to 6.2% while revenue shrank slightly. This is a deliberate investment/overhead story, not a manufacturing-cost or pricing problem.

> [!question]- 4. If total liabilities represent 40% of total assets, how much could asset values decline before lenders' claims are impaired?
> Up to **60%** — the equity cushion. Assets can lose value equal to the entire equity share before the remaining value falls short of liabilities.

> [!question]- 5. Why is the cash flow margin described as a "vital check on earnings quality"?
> Net income is built on accruals, estimates, allocations, and timing judgments. The cash flow margin compares operating cash generation directly to sales, bypassing those accrual choices. When accrual net margin collapses but cash flow margin holds firm (Tesla 2024–2025), the cash generation capability is intact; when both fall together (or cash turns negative while income stays positive), earnings quality is suspect.

> [!question]- 6. Name two things a common-size statement *cannot* show you.
> Any two of: absolute dollar magnitudes/materiality; composition within aggregated lines; one-time vs. recurring items; cross-statement causality (e.g., whether CapEx drove the PP&E share increase).

---

### Practice Activity

Using Tesla's condensed balance sheet data below, compute the common-size percentages for **December 31, 2024**:

| Item | $M |
|------|---:|
| Cash + ST investments | 36,563 |
| Inventory | 12,017 |
| PP&E, net | 35,836 |
| Total assets | 122,070 |
| Total liabilities | 48,390 |

1. Cash + investments as % of total assets
2. Inventory as % of total assets
3. PP&E as % of total assets
4. Debt-to-assets ratio and implied equity cushion %

> [!success]- Check Your Answers
> 1. 36,563 ÷ 122,070 = **30.0%**
> 2. 12,017 ÷ 122,070 = **9.8%**
> 3. 35,836 ÷ 122,070 = **29.4%**
> 4. 48,390 ÷ 122,070 = **39.6%** debt-to-assets → equity cushion ≈ **60%**
>
> Your percentages should match the 2024 column in the common-size balance sheet above. If they do, you have mastered the mechanic — the real skill is the interpretation layer built on top of it.

---

### Related Notes

- [[M2-Obj-2-1]] — The Balance Sheet being resized in Section II
- [[M2-Obj-2-2]] — The Income Statement behind Section III's margins
- [[M2-Obj-2-3]] — CFO source for the cash flow margin
- [[M3-Overview]] — Module roadmap
- [[M3-Obj-3-2]] — Next: horizontal analysis adds the *time dimension*
