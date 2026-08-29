---
title: M3-Obj-3-3 - Du Pont Synthesis (ROE Deconstruction)
created: 2026-08-25
date: 2026-08-25
tags:
  - FSA
  - M3
  - Objective-3-3
  - DuPont
  - ROE
aliases:
  - du-pont-analysis
  - dupont-system
  - roe-decomposition
---

# Learning Objective 3.3

## Synthesize financial ratios through the Du Pont System to deconstruct Return on Equity (ROE) and evaluate sustainable growth

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc.
> We complete the Module 3 trilogy by synthesizing everything into one question: *what return did Tesla actually deliver to its shareholders, and what drove it?* All figures in millions of USD except ratios and per-share data. Balance sheet figures are **averages** — (beginning + ending) ÷ 2 — to align with full-year income flows.

| Input | 2023 | 2024 | 2025 |
|-------|-----:|-----:|-----:|
| Net income | $14,974 | $7,153 | $3,855 |
| Total revenues | $96,773 | $97,690 | $94,827 |
| Average total assets | $94,478 | $114,344 | $129,938 |
| Average stockholders' equity | $53,669 | $67,773 | $77,525 |
| Interest expense | $156 | $350 | $338 |

*Opening (Dec 31, 2022) balances used in averages: total assets \$82,338; stockholders' equity \$44,704.*

---

### I. The Philosophy of Ratio Synthesis: Beyond the Silo

Introductory courses teach ratios in silos — liquidity over here, profitability over there. But ratios do not live in isolation: they form an integrated web where operational decisions directly shape financing outcomes.

> [!info] What Is the Du Pont System?
> The **Du Pont system** (developed by engineers at DuPont Corporation a century ago) is a mathematical framework that multiplies simple ratios together so they *explain* the big ones. It is the ultimate tool for completing a firm's evaluation because it shows how:
> - **Operational choices** — profit margins and asset turnover
> - **Financing choices** — capital structure and interest burden
>
> ...combine over an accounting period to produce the overall return earned by shareholders (**ROE**). Instead of asking *"is ROE high or low?"*, Du Pont asks *"WHICH lever moved?"*

The system has three layers, each answering a deeper question:

```
Layer 1 (Classic):    ROA  = Asset Turnover  ×  Net Profit Margin
                            "How hard do assets work?" × "How much survives each sale?"

Layer 2 (Modified):   ROE  = ROA  ×  Financial Leverage
                            "Operating return" × "Equity multiplier from debt"

Layer 3 (Extended):   EPS, FLI, Sustainable Growth Rate
                            "What does each share earn?" · "Is debt helping?" · "How fast CAN we grow?"
```

---

### II. Layer 1 — Deconstructing Return on Assets (Classic Du Pont)

$$\text{Return on Assets (ROA)} = \frac{\text{Net Income}}{\text{Total Assets}} = \underbrace{\frac{\text{Net Sales}}{\text{Total Assets}}}_{\text{Asset Turnover}} \times \underbrace{\frac{\text{Net Income}}{\text{Net Sales}}}_{\text{Net Margin}}$$

ROA measures the overall efficiency of the firm in generating earnings from its total investment in assets. The decomposition reveals the two strategic routes to the same destination:

- **High-volume / low-margin**: turn assets over very fast on thin margins (grocery retail, discounters)
- **Low-volume / high-margin**: sell slowly but richly (luxury goods, pharma)

Neither route is superior — but the decomposition tells you *which engine* a company runs on, and therefore which breakdowns matter.

#### Tesla's Classic Du Pont Decomposition

| Component | 2023 | 2024 | 2025 |
|-----------|-----:|-----:|-----:|
| Net profit margin ([[M3-Obj-3-1]]) | 15.5% | 7.3% | 4.1% |
| Asset turnover ([[M3-Obj-3-2]]) | 1.02× | 0.85× | 0.73× |
| **ROA (= product)** | **15.8%** | **6.3%** | **3.0%** |

*(Components rounded; product computed from unrounded values.)*

**Interpretation:** Tesla's ROA collapsed by a factor of ~5.3 in two years — and the decomposition shows this was a **double compression**: the margin engine weakened (price cuts, R&D surge) *while simultaneously* the turnover engine slowed (assets growing faster than sales). When both levers weaken at once, their effects compound multiplicatively: margin fell ÷3.8, turnover fell ÷1.4, so ROA fell ÷5.3. A single-ratio analyst would only see "ROA down"; the Du Pont analyst sees *both engines failing at once*.

---

### III. Layer 2 — From ROA to ROE: The Double-Edged Sword of Financial Leverage

Shareholders do not earn ROA — they earn ROE. The bridge between them is **financial leverage**: using fixed-cost debt to finance assets. Because interest is a **fixed contractual cost**, whatever operating returns remain flow entirely to equity holders — amplified in both directions.

#### Classroom Illustration: Sockee Corporation

Sockee has \$100,000 of assets financed 50/50 with debt (at 10% = \$5,000 fixed annual interest) and equity. Corporate tax rate: 40%.

| | A: Baseline | B: Ops Double | C: Ops Halve |
|---|---:|---:|---:|
| Operating earnings (EBIT) | \$20,000 | \$40,000 | \$10,000 |
| − Interest expense (fixed) | (\$5,000) | (\$5,000) | (\$5,000) |
| Earnings before tax | \$15,000 | \$35,000 | \$5,000 |
| − Tax (40%) | (\$6,000) | (\$14,000) | (\$2,000) |
| **Net earnings** | **\$9,000** | **\$21,000** | **\$3,000** |
| **ROE (÷ \$50,000 equity)** | **18%** | **42%** | **6%** |

- **Upside amplification:** operations rose +100%, but ROE rose **+133%** (18% → 42%) — the fixed interest cost stayed put while profits doubled
- **Downside amplification:** operations fell −50%, but ROE collapsed **−67%** (18% → 6%)

Leverage multiplies *risk* exactly as it multiplies *return*. Analysts must always weigh the benefit of debt against this inherent hazard.

#### Tesla's Modified Du Pont Decomposition

$$\text{Return on Equity (ROE)} = \text{ROA} \times \underbrace{\frac{\text{Total Assets}}{\text{Stockholders' Equity}}}_{\text{Financial Leverage (Equity Multiplier)}}$$

| Component | 2023 | 2024 | 2025 |
|-----------|-----:|-----:|-----:|
| ROA | 15.8% | 6.3% | 3.0% |
| Financial leverage | 1.76× | 1.69× | 1.68× |
| **ROE (= product)** | **27.9%** | **10.6%** | **5.0%** |

**Interpretation:** Tesla's financial leverage barely moved (1.76× → 1.68×) — liabilities have held steady near 40% of assets since 2023 ([[M3-Obj-3-1]]). Therefore essentially **none of the 23-point ROE collapse was financial**: it was almost purely the operational compression flowing through from Layer 1. Compare with Sockee's Scenario C: had Tesla been aggressively leveraged, the same operational decline could have produced a far uglier ROE. Conversely, the modest leverage means shareholders forgo some upside amplification in good years — a conservative trade-off visible directly in the math.

> [!tip] The ROE Inflation Warning
> Because ROE = ROA × Leverage, management can **artificially inflate ROE by taking on risky debt without improving operations at all**. Always decompose before praising a high ROE: ask whether it came from the operating engine (sustainable) or the leverage multiplier (fragile). Tesla's flat multiplier makes its answer easy; not every company gets that benefit of the doubt.

---

### IV. Measuring Leverage Efficiency: The Financial Leverage Index (FLI)

Is debt *helping* the shareholders or hurting them? The **Financial Leverage Index** answers directly:

$$\text{FLI} = \frac{\text{ROE}}{\text{Adjusted ROA}} \qquad \text{where} \qquad \text{Adjusted ROA} = \frac{\text{Net Income} + \text{Interest Expense} \times (1 - \text{Tax Rate})}{\text{Total Assets}}$$

Adding back the *after-tax* cost of interest strips financing effects out of ROA, leaving pure operating returns on the asset base:

- **FLI > 1** — ROE exceeds the unlevered operating return: debt is employed **beneficially**
- **FLI < 1** — the firm earns less on borrowed money than it costs: debt is destroying shareholder value

#### Tesla's FLI

| Year | Net Income | + Interest × (1−21%) | Adjusted ROA | ROE | **FLI** |
|------|-----------:|---------------------:|-------------:|----:|--------:|
| 2023 | $14,974 | +$123 | 16.0% | 27.9% | **1.75** |
| 2024 | $7,153 | +$277 | 6.5% | 10.6% | **1.62** |
| 2025 | $3,855 | +$267 | 3.2% | 5.0% | **1.57** |

*\*A statutory 21% tax rate is used because Tesla's effective rates are distorted — 2023's was negative (−50%) due to the one-time deferred-tax benefit, which would corrupt the adjustment.*

**Interpretation:** FLI stays comfortably above 1 throughout — every dollar of debt-financed assets earned more than debt's after-tax cost, so leverage consistently added to shareholder returns (consistent with Tesla's tiny interest expense against a large operating base). But the index is drifting down: 1.75 → 1.57. The cushion between operating returns and financing costs is narrowing — not yet a warning, but no longer a constant either. Track it forward.

---

### V. Advanced Synthesis Extensions

#### 1. EPS Disaggregation

The full Du Pont chain extends all the way to earnings per share:

$$\text{EPS} = \text{Asset Turnover} \times \text{Net Margin} \times \text{Financial Leverage} \times \text{Book Value Per Share}$$

Since the first three factors multiply back to ROE, EPS = ROE × BVPS. Using average balances and average shares outstanding:

| Component | 2023 | 2024 | 2025 |
|-----------|-----:|-----:|-----:|
| ROE | 27.9% | 10.6% | 5.0% |
| Book value per share (avg) | $16.91 | $21.18 | $22.25 |
| **Implied EPS** | **$4.72** | **$2.23** | **$1.11** |
| Reported diluted EPS | $4.30 | $2.04 | $1.08 |

*Differences arise from noncontrolling-interest attribution and averaging conventions — the identity approximates basic EPS well.*

The instructional value: EPS is often quoted as *the* number, but the disaggregation proves it is just the end of a causal chain. It also reveals the mathematical boundaries of growth — EPS cannot grow indefinitely through turnover or leverage expansion alone, since both have practical ceilings.

#### 2. Sustainable Growth Rate

$$g = \text{ROE} \times (1 - \text{Dividend Payout Ratio})$$

*g* is the maximum rate a firm can grow **using internally generated funds** — without issuing new equity or stretching beyond prudent leverage.

Tesla pays **no dividends** (payout ratio = 0), so its entire ROE is retained:

| Year | Sustainable growth rate \(g\) |
|------|------------------------------:|
| 2023 | 27.9% |
| 2024 | 10.6% |
| 2025 | **5.0%** |

**The tension this exposes:** from [[M3-Obj-3-2]], Tesla's asset base compounded at **+13.7% per year** (2023–2025 CAGR) — yet its internally fundable growth rate fell from 28% to 5%. The gap must be bridged externally: new debt, stock option exercises, and noncontrolling-interest contributions (the capital-raising pattern documented in [[M2-Obj-2-3]]). If ROE keeps compressing while the asset base keeps expanding, either growth slows or external dependence deepens. That single sentence — invisible in any one statement alone — is what ratio synthesis buys you.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Du Pont system** | Framework multiplying component ratios to deconstruct ROA and ROE into margin, turnover, and leverage drivers |
| **ROA** | Net income ÷ total assets; overall efficiency of the asset base |
| **Asset turnover** | Sales ÷ average total assets; how hard assets work |
| **Net margin** | Net income ÷ sales; profit surviving each revenue dollar |
| **Financial leverage (equity multiplier)** | Total assets ÷ stockholders' equity; the debt-driven amplifier between ROA and ROE |
| **ROE** | Net income ÷ stockholders' equity; the final return to owners |
| **Financial Leverage Index (FLI)** | ROE ÷ adjusted ROA; >1 means debt benefits shareholders |
| **Adjusted ROA** | [Net income + interest × (1 − tax rate)] ÷ total assets; unlevered operating return on assets |
| **EPS disaggregation** | Expressing EPS as turnover × margin × leverage × book value per share |
| **Sustainable growth rate (g)** | ROE × (1 − payout); maximum internal-funding growth rate |
| **Dividend payout ratio** | Dividends ÷ net income; Tesla's is zero |

---

> [!danger] Red Flags — What Synthesis Reveals (and Where It Misleads)
> **Reveals:**
> - **Leverage-inflated ROE** — rising ROE on a flat or falling ROA means the "improvement" came from added debt risk, not operations
> - **Double compression** — simultaneous margin and turnover decay compounds into outsized ROA/ROE collapse (Tesla 2023–2025: ÷5.3)
> - **Narrowing leverage cushion** — declining FLI signals operating returns converging toward financing costs
> - **Growth-funding gaps** — sustainable g below actual asset growth exposes deepening reliance on external capital
>
> **Misleads when:**
> - **Effective tax rates are distorted** — use statutory rates for the FLI interest adjustment when one-time items skew the effective rate (Tesla 2023: −50%)
> - **NCI is ignored** — equity attributable to noncontrolling interests muddies ROE; define the equity base explicitly
> - **Point-in-time balance sheets** — pairing full-year income with year-end balances mismatches flows and stocks; average them
> - **One exceptional base year** — every growth rate chained to an abnormal year inherits its distortion (see [[M3-Obj-3-2]])
>
> Rule: decompose before you judge, and ask *which lever moved* before asking *whether the number is good*.

---

### Review Questions

> [!question]- 1. State the classic and modified Du Pont identities and the question each layer answers.
> Classic: ROA = Asset Turnover × Net Margin — "which operating engine drives returns?" Modified: ROE = ROA × Financial Leverage — "how much does capital structure amplify (or shrink) the operating return for shareholders?"

> [!question]- 2. Tesla's ROA fell from 15.8% to 3.0%. Why is knowing the decomposition essential here that the raw ROA alone cannot provide?
> Because BOTH components fell simultaneously — margin ÷3.8 AND turnover ÷1.4 — and multiplicative compounding turned two moderate declines into a ÷5.3 collapse. The raw number shows magnitude; the decomposition shows mechanism (margin-led pricing/investment pressure plus asset-base outgrowing sales), which determines what management could do about it.

> [!question]- 3. In Sockee's Scenario C, operating earnings fell 50% but ROE fell 67%. Explain the mechanics.
> Interest expense is a fixed contractual cost (\$5,000 regardless of performance). When EBIT halves, that fixed burden consumes twice the relative share of earnings, so the residual to shareholders shrinks disproportionately: \$9,000 → \$3,000 on an unchanged \$50,000 equity base. Leverage transmits operating volatility to shareholders *amplified*, in both directions (+100% ops became +133% ROE in Scenario B).

> [!question]- 4. Could a company show a rising ROE while its operations deteriorate? Construct the scenario.
> Yes: hold ROA falling but increase financial leverage faster — e.g., borrow heavily to repurchase shares or fund assets. ROE = ROA × Leverage can rise arithmetically even as margins and turnover decay. This is precisely why analysts decompose ROE before praising it: the improvement may be purchased with fragility, and FLI would expose whether the new debt even earns above its after-tax cost.

> [!question]- 5. Why is a statutory tax rate (21%) used in Tesla's adjusted ROA instead of the effective rate?
> The adjustment needs a clean, stable rate to strip the tax shield on interest. Tesla's effective rates are distorted by one-time items — 2023's was negative (−50%, the deferred-tax benefit) — which would produce a nonsensical interest adjustment. Statutory rates keep the metric comparable across years and companies.

> [!question]- 6. Tesla retains 100% of earnings, so g = ROE fell from 28% to 5%, yet assets grew 13.7%/yr. What does this divergence imply, and where would you look to confirm how the gap was funded?
> Internal capacity to fund growth collapsed below actual expansion — the difference must be financed externally (or growth must slow). Confirmation lives in financing activities ([[M2-Obj-2-3]]): debt issuance/repayment patterns, stock option exercises, and noncontrolling-interest contributions — Tesla funded via option proceeds, incremental debt within its treadmill, and NCI rather than dividends or buyback-free dilution.

---

### Practice Activity

Using Tesla's 2024 inputs below, rebuild the full Du Pont chain:

| Input | Value |
|-------|------:|
| Net income | $7,153M |
| Net sales | $97,690M |
| Average total assets | $114,344M |
| Average stockholders' equity | $67,773M |
| Interest expense | $350M (statutory tax rate 21%) |

1. Net margin and asset turnover
2. ROA (classic identity)
3. Financial leverage and ROE (modified identity)
4. Adjusted ROA and FLI

> [!success]- Check Your Answers
> 1. Net margin = 7,153 ÷ 97,690 = **7.3%**; asset turnover = 97,690 ÷ 114,344 = **0.85×**
> 2. ROA = 0.85 × 7.3% ≈ **6.3%** (unrounded: 7,153 ÷ 114,344 = 6.26%)
> 3. Leverage = 114,344 ÷ 67,773 = **1.69×**; ROE = 6.26% × 1.687 = **10.6%** (check: 7,153 ÷ 67,773 = 10.55%)
> 4. Adjusted ROA = (7,153 + 350 × 0.79) ÷ 114,344 = 7,430 ÷ 114,344 = **6.5%**; FLI = 10.55% ÷ 6.50% = **1.62**
>
> Your chain should reproduce the 2024 column in each table above. You have now built the complete synthesis: margin → turnover → ROA → leverage → ROE → leverage efficiency.

---

### Related Notes

- [[M3-Obj-3-1]] — Vertical analysis: source of the margin components
- [[M3-Obj-3-2]] — Horizontal analysis: source of turnover and growth trajectories
- [[M2-Obj-2-3]] — Financing activities confirming the external funding gap
- [[M3-Overview]] — Module roadmap
- [[03-Module-3/FSA-Skills-Ratio-Analysis]]
