---
title: M7-Obj-7-1 - Build Pro Forma Financial Statements and Determine External Financing Needs
created: 2026-11-08
date: 2026-11-08
tags:
  - FSA
  - M7
  - Objective-7-1
  - Forecasting
aliases:
  - pro-forma-modeling
  - percentage-of-sales-method
  - external-financing-needed
---

# Learning Objective 7.1

## Build Pro Forma Financial Statements and Determine External Financing Needs

**By the end of this note, you can:**
- Explain what a pro forma statement is, who builds one, and what three decisions it serves (strategy, credit, M&A)
- Run the four-step forecast method: sales anchor → cost and interest projection → balance-sheet accounts → retained earnings and the **external financing needed (EFN)** plug
- Interpret the sign of the EFN and the three ways a model can absorb it — and what each absorption hides
- Build a full pro forma income statement and balance sheet from a percentage-of-sales starting point, then prove your answer with a cash reconciliation
- Apply the method to Tesla's FY2025 10-K base and state every assumption and simplification you had to make

> [!tip] How to read this note
> Read the method first (§I–II), then work the Titan Dynamics case with the solution collapsed (§III), then watch the same four steps applied to Tesla (§IV). In §III and the Review Questions, **attempt each task before expanding a solution** — the answers are collapsed on purpose. If the ratio machinery (DSO/DSI/DPO, margins) feels rusty, the *Related Notes* at the bottom link the exact primers.

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc. — and the Analyst Who Must Fund the Future
> Modules 2–4 taught us to *read* statements; Module 5 taught us to distrust their earnings; Module 6 taught us to map the risks hiding inside them. Module 7 turns the instrument around: we now **write** the statements, forward. A pro forma statement is a forward-looking financial report built on an explicit set of assumptions about revenue, costs, capital spending, and financing — and its most consequential output is not the earnings line but the **gap**: the amount of external financing the plan needs before it can balance.
>
> The running company remains **Tesla, Inc.** (FY2025 Form 10-K). This is a *demanding* calibration case for forecasting, because Tesla is doing three things at once: growing a high-margin services and energy business, running a capital-intensive factory ramp, and sitting on a cash fortress (\$44,059M of cash and investments) that lets it fund the plan without asking anyone. The danger shapes come from the course reference (Fridson & Alvarez): **Titan Dynamics** (the clean percentage-of-sales model), the **Sage Inc.** store-expansion story (planning a rollout you must fund), and **Colossal Chemical** (a forecast that breaks under margin compression).

Three questions, three clocks — this module's forecast layers:

| Layer | What can go wrong | Clock | Core instruments |
|---|---|---|---|
| **The sales anchor** | Volume, price, and mix assumptions replacing history | Years | Bottom-up segment build · nominal vs. real growth decomposition |
| **The cost and balance-sheet build** | Fixed-cost absorption, working-capital velocity, capital spending | Quarters | % of sales · DSO/DSI/DPO anchors · PP&E roll-forward · operating leverage |
| **The plug** | The plan not balancing — and the choice of which financing absorbs the gap | Days to years | EFN · retained-earnings roll-forward · debt vs. equity vs. cash absorption |

> [!tip] Where Module 7 Splits in Three
> 7.1 builds the forecast and the financing gap — the plan and the money it needs. 7.2 ([[M7-Obj-7-2]]) asks what happens when the assumptions move — because a forecast is a set of *assumptions*, and a forecast that cannot be stressed is a guess with formatting. 7.3 ([[M7-Obj-7-3]]) asks what the projected cash flows are *worth* — turning a forecast into a valuation, and a valuation into a decision.

---

### I. Purpose & Architecture of Pro Forma Modeling

#### 1. What a pro forma statement is

A pro forma statement is **not a forecast of history** — it is a forward-looking financial report constructed on an explicit set of assumptions about future revenue growth, cost behavior, capital investment, and financing. The word *pro forma* means "as if": the statements show what the balance sheet and earnings would look like if the plan happened.

The single most important property of a pro forma model is that it is **transparent about assumptions**. Every projected number must be traceable to either (a) a stated assumption, (b) a historical ratio from the statements, or (c) another projected line. A projected number that is traceable to none of the three is an invention, and it will be the number that is wrong.

#### 2. The three decisions a pro forma model serves

| Use | The question it answers | Typical reader | Example |
|---|---|---|---|
| **Long-range strategic planning** | Can we fund the growth we are planning? | Management, board | Sage Inc.'s retail rollout: does the expansion self-fund, or does it need a credit facility? |
| **Credit underwriting** | Will projected cash flows cover debt service? | Lenders | Does projected CFO cover scheduled principal and interest, and how much cushion is left? |
| **M&A and restructuring** | What happens to earnings per share and leverage after the deal? | Acquirers, investors | Post-merger EPS accretion, or the leverage change after a large buyback funded with debt |

Note what all three have in common: the model is a **decision document**. Nobody builds a pro forma to learn what next year's revenue will be — they build it to see how a plan behaves, and then to defend it.

> [!danger] The forecast is not a prediction
> A pro forma statement is a **conditional** document: *if* revenue grows at 10%, *if* the cost ratio holds, *if* working capital turns at the historical rate, *then* the plan needs \$X of external financing. The number that matters is not the point estimate — it is the **sensitivity of the answer to the assumptions** ([[M7-Obj-7-2]]) and the **value** of the resulting cash flows ([[M7-Obj-7-3]]). A forecast that arrives with no assumption list is not analysis; it is a number.

#### 3. The four-step forecasting flow

<div style="display:flex;flex-direction:column;align-items:center;gap:0.5rem;margin:1rem 0">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.4rem;font-weight:600">THE FOUR-STEP PRO FORMA FLOW</div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;align-items:stretch;gap:0.75rem;width:100%">
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Step 1 · Sales anchor</b><br/><span style="font-size:0.85em">Bottom-up volume and price · nominal vs. real growth</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Step 2 · Costs and interest</b><br/><span style="font-size:0.85em">% of sales · fixed vs. variable · embedded cost of debt</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Step 3 · Balance sheet</b><br/><span style="font-size:0.85em">DSO/DSI/DPO anchors · PP&amp;E roll-forward</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Step 4 · The plug</b><br/><span style="font-size:0.85em">Retained-earnings roll-forward · EFN</span></div>
  </div>
</div>

---

### II. The Four-Step Method

#### Step 1 — The sales anchor

Sales revenue is the **common denominator** of the entire forecast: every cost line, every working-capital account, and every ratio in the model is anchored to it. Three ways to build the anchor:

1. **Bottom-up segment build.** Project physical volume and price by product line and geography, then multiply and add. This is the analyst's default when the disclosure supports it — Tesla reports automotive sales, automotive leasing, regulatory credits, services and other, and energy generation and storage as separate revenue streams, so a bottom-up build is feasible in principle.
2. **Top-down growth rate.** Apply a management-guided or industry growth rate to the historical base. Fast, and it hides the question "growth in *what*?"
3. **Price and volume decomposition.** Separate nominal growth into price and volume, and then separate nominal into real growth and inflation:

$$\text{Nominal Growth} = \text{Real Volume Growth} + \text{Price Growth} + \text{Mix} \approx (1 + g_{\text{real}})(1 + g_{\text{price}}) - 1$$

The reason this decomposition matters: **a forecast built on nominal growth inherits the inflation assumption implicitly, and a cost ratio built on nominal sales inherits it too**. If the revenue anchor carries 4% inflation but the cost ratios were computed on last year's *real* cost base, the forecast quietly invents margin.

> [!tip] Beginner's on-ramp: three questions before you touch the model
> 1. **What is the unit?** Forecast units and price, not just dollars — units is where the operating story lives.
> 2. **Which of the two do I forecast, and which do I hold?** If revenue is the anchor, every other line is either a ratio of revenue or an independent assumption (CapEx, D&A, tax rate, dividends) — write the list down.
> 3. **Where does the cash go?** Sketch the cash bridge (earnings + non-cash charges − investment − working capital) *before* building the balance sheet. The plug is easier to predict this way than the other way round.

#### Step 2 — Cost projection and the cost of debt

**Percentage-of-sales method.** Operating costs (cost of revenues, SG&A, and R&D) are first modeled as historical percentages of sales:

$$\text{Projected Cost} = \text{Projected Sales} \times \text{Historical Cost Ratio}$$

**Fixed vs. variable distortion.** The percentage-of-sales method is a *starting point*, not an answer. Fixed overhead — plant depreciation, engineering headcount, factory leases — does **not** scale with volume. Consequently:

- in growth, holding the ratio flat **overstates** cost and understates margin (the fixed base is spread over more units);
- in contraction, holding the ratio flat **understates** cost and overstates margin (the fixed base is spread over fewer units).

This is the operating-leverage machinery of [[M6-Obj-6-1]] §II.2 arriving in a forecast: the same fixed-cost intensity that made the downturn case brutal is what makes a growth forecast optimistic. Honest models either split costs into fixed and variable components or stress the ratio explicitly ([[M7-Obj-7-2]]).

**Interest expense and the embedded cost of debt.** Interest in a forecast is not a percentage of sales; it is a rate applied to the debt the plan actually carries:

$$\text{Projected Interest Expense} = \text{Projected Total Debt} \times \text{Embedded Interest Rate}$$

The *embedded* rate comes from the historical statements (interest expense ÷ average debt) and is the rate the company actually pays on what it has already borrowed — not the rate a lender might quote for new money.

#### Step 3 — Balance-sheet account projection

**Working capital is anchored to velocity, not to a balance.** Each working-capital account is projected from projected sales or cost of revenues using the historical days metric:

$$\text{Accounts Receivable} = \text{Projected Sales} \times \left(\frac{\text{Target DSO}}{365}\right)$$

$$\text{Inventory} = \text{Projected Cost of Revenues} \times \left(\frac{\text{Target DSI}}{365}\right)$$

$$\text{Accounts Payable} = \text{Projected Cost of Revenues} \times \left(\frac{\text{Target DPO}}{365}\right)$$

The forecast assumption is not "accounts receivable goes up 10%" but "receivables turn in 17.6 days" — the first is an assumption about a balance, the second is an assumption about *behavior*, and behavior is what actually changes when a firm grows.

**PP&E rolls forward.** Projected net PP&E is a roll-forward, not a ratio:

$$\text{Ending Net PP\&E} = \text{Beginning Net PP\&E} + \text{CapEx} - \text{Depreciation}$$

**Cash is a policy, not a forecast.** Most models hold cash at a target minimum balance (a revolver buffer) and let the plug absorb the difference. Cash held *above* the target is idle; cash held *below* it is an unfinanced gap. Both are decisions, and both must be visible.

**Equity rolls forward.** Ending retained earnings is a roll-forward too:

$$\text{Ending Retained Earnings} = \text{Beginning Retained Earnings} + \text{Projected Net Income} - \text{Projected Dividends}$$

#### Step 4 — Reconciliation and the external financing plug

Projected assets rarely equal projected liabilities plus equity on the first pass, because the model has not yet decided **who funds the gap**. The balancing item is the external financing needed:

$$\text{EFN} = \text{Projected Total Assets} - (\text{Projected Total Liabilities} + \text{Projected Total Equity})$$

| EFN sign | Reading | Financing response |
|---|---|---|
| **EFN > 0** | Asset growth exceeds internal cash generation | Raise external money: short-term notes, long-term debt, or equity issuance |
| **EFN < 0** | Internal cash generation exceeds investment needs | Surplus cash accumulates — cash above target, or debt repaid, or a distribution to shareholders |
| **EFN = 0** | The plan is exactly self-funding | The rarest and most fragile outcome: any assumption slip breaks it |

> [!warning] Three ways to make the plug disappear — and what each one hides
> A model can always be balanced. The *honest* question is which financing absorbs the gap:
> 1. **Debt** — preserves ownership and EPS, but adds fixed interest obligations and covenant constraints ([[M6-Obj-6-1]] §I.3).
> 2. **Equity** — removes the financing risk and the interest, but dilutes existing owners; note that Tesla issued **535M shares** during 2025 (3,751M outstanding vs. 3,216M a year earlier), so dilution is a live cost even at a fortress balance sheet.
> 3. **Cash** — the easiest and the most self-deceiving: "fund it from the balance sheet" is a financing decision that *hides* the fact that the cash was earning something and may be needed for the next capex cycle. In our Tesla forecast this is exactly where the plug lands, and §IV makes that visible rather than quiet.
>
> And a fourth, illegitimate option: **plug the hole with a smaller cash balance** so the statement "balances" while liquidity quietly falls below the minimum the business needs to run.

---

### III. Worked Calculation: Titan Dynamics

> [!tip] Before you flip any answer
> Attempt all four tasks with the baseline data in front of you. The solution is collapsed on purpose. Titan is a clean teaching case on purpose: no unusual items, no leases, no equity issuance — so every number you produce must come from the method, not from judgment.

#### Scenario

You are a financial analyst at a commercial bank evaluating **Titan Dynamics Corp.** for a \$15,000 thousand expansion loan. Titan's baseline FY2024 statements (\$ in thousands):

| Income statement (FY2024) | Amount | | Balance sheet (Dec 31, 2024) | Amount |
|---|---:|---|---|---:|
| Net revenue | 100,000 | | Cash and securities | 5,000 |
| Cost of goods sold (60.0% of sales) | 60,000 | | Accounts receivable (DSO = 54.75 days) | 15,000 |
| SG&A (20.0% of sales) | 20,000 | | Inventory (DSI = 73.00 days) | 12,000 |
| Depreciation | 5,000 | | Net PP&E | 48,000 |
| Operating income (EBIT) | 15,000 | | **Total assets** | **80,000** |
| Interest expense (8.0% on 25,000 debt) | 2,000 | | Accounts payable (DPO = 54.75 days) | 9,000 |
| Pre-tax income | 13,000 | | Accrued current liabilities | 6,000 |
| Income tax expense (30%) | 3,900 | | Total debt (short and long-term) | 25,000 |
| **Net income** | **9,100** | | Stockholders' equity (CS 10,000 + RE 30,000) | 40,000 |
| | | | **Total liabilities and equity** | **80,000** |

**Forecast assumptions for FY2025:**
1. Net revenues grow by **15.0%**.
2. COGS and SG&A maintain their baseline percentage-of-sales ratios (60.0% and 20.0%).
3. Planned capital expenditures = **\$10,000 thousand**; 2025 depreciation = **\$6,000 thousand**.
4. Receivables, inventory, and payables grow proportionally with sales/COGS (baseline DSO, DSI, DPO maintained). Accrued liabilities stay at \$6,000.
5. Cash is held at a target minimum balance of **\$5,000 thousand**.
6. Titan pays out **30.0%** of net income as cash dividends.
7. Existing debt carries an 8.0% rate; assume interest on any new EFN borrowing is paid in 2026.

**Tasks.** (1) Construct the pro forma income statement for FY2025 and the addition to retained earnings. (2) Construct the pro forma balance sheet before financing adjustments. (3) Calculate the EFN. (4) State whether Titan generates sufficient internal cash to fund its expansion or requires external bank debt.

> [!success]- Solution
> **(1) Pro forma income statement (FY2025)**
> - Revenue = 100,000 × 1.15 = **115,000**
> - COGS = 115,000 × 0.60 = **69,000**
> - SG&A = 115,000 × 0.20 = **23,000**
> - Depreciation = **6,000**
> - EBIT = 115,000 − 69,000 − 23,000 − 6,000 = **17,000**
> - Interest = 25,000 × 8.0% = **2,000** → pre-tax = 15,000
> - Tax at 30% = **4,500** → **Net income = 10,500**
> - Dividends (30%) = 3,150 → **addition to retained earnings = 7,350**
>
> **(2) Pro forma balance sheet (FY2025, pre-financing)**
> - Cash (target minimum) = **5,000**
> - Accounts receivable = 15,000 × 1.15 = **17,250**
> - Inventory = 12,000 × 1.15 = **13,800**
> - Net PP&E = 48,000 + 10,000 − 6,000 = **52,000**
> - **Total assets = 5,000 + 17,250 + 13,800 + 52,000 = 88,050**
> - Accounts payable = 9,000 × 1.15 = **10,350**; accrued = **6,000**; debt = **25,000**
> - Stockholders' equity = 40,000 + 7,350 = **47,350**
> - **Total liabilities and equity = 10,350 + 6,000 + 25,000 + 47,350 = 88,700**
>
> **(3) EFN** = 88,050 − 88,700 = **−650** (a *surplus*, not a shortfall)
>
> **(4) Determination.** Titan is **self-funding** and does **not** need external bank debt. Sources of \$8,700 (retained-earnings addition 7,350 + payables growth 1,350) exceed the \$8,050 of asset investment (receivables 2,250 + inventory 1,800 + net PP&E 4,000) by **\$650**. Proof by cash reconciliation: net income 10,500 + depreciation 6,000 − CapEx 10,000 − working-capital investment 2,700 − dividends 3,150 = **+650** of cash, so cash could be 5,650 instead of the 5,000 target.

> [!danger] Reading the EFN: −650 is a surplus, and a surplus is still a decision
> A negative EFN is not an error and it is not free money. It says the plan generates more cash than it needs at the target cash balance. Three legitimate responses: let cash build above target, repay debt, or distribute to shareholders. The illegitimate response — and the one this note warns against — is to bury the surplus in "cash" without disclosing it, because a reader who sees only "assets = liabilities + equity" cannot tell a self-funding plan from a plan quietly running its balance sheet down to nothing.

---

### IV. Applying the Method to Tesla (FY2026 forecast)

Now the same four steps, applied to Tesla's FY2025 Form 10-K base. **Every assumption below is instructor-set for teaching** — none of it is Tesla guidance, and the point of the exercise is the mechanics and the disclosures, not a forecast of Tesla.

#### The FY2025 base (from the 10-K)

| Income statement (FY2025, \$M) | Amount | | Balance sheet (Dec 31, 2025, \$M) | Amount |
|---|---:|---|---|---:|
| Total revenues | 94,827 | | Cash and cash equivalents | 16,513 |
| Cost of revenues | 77,733 | | Short-term investments | 27,546 |
| Gross profit | 17,094 | | Accounts receivable, net | 4,576 |
| Research and development | 6,411 | | Inventory | 12,392 |
| Selling, general and administrative | 5,834 | | Prepaid and other current assets | 7,615 |
| Restructuring and other | 494 | | Total current assets | 68,642 |
| **Income from operations (EBIT)** | **4,355** | | Operating lease vehicles, net | 4,912 |
| Interest income | 1,680 | | Energy generation and storage systems, net | 4,604 |
| Interest expense | (338) | | Property, plant and equipment, net | 40,643 |
| Other income (expense), net | (419) | | Operating lease right-of-use assets | 6,027 |
| Income before income taxes | 5,278 | | Digital assets | 1,008 |
| Provision for income taxes | 1,423 | | Deferred tax assets | 6,925 |
| **Net income** | **3,855** | | Other non-current assets | 5,045 |
| | | | **Total assets** | **137,806** |
| | | | Accounts payable | 13,371 |
| | | | Accrued liabilities and other | 13,279 |
| | | | Deferred revenue (current and non-current) | 7,055 |
| | | | Debt and finance leases (current and non-current) | 8,376 |
| | | | Other long-term liabilities | 12,860 |
| | | | **Total liabilities** | **54,941** |
| | | | Retained earnings | 39,003 |
| | | | Common stock + APIC + AOCI | 43,134 |
| | | | **Stockholders' equity** | **82,137** |
| | | | Noncontrolling and redeemable interests | 728 |
| | | | **Total liabilities and equity** | **137,806** |

Derived ratios (ending balances, the forecasting convention): **DSO 17.61 days**, **DSI 58.19 days**, **DPO 62.78 days**; cost of revenues **81.97%** of sales, R&D **6.76%**, SG&A **6.15%**, EBIT margin **4.59%**, effective tax rate **26.96%**, EBITDA \$10,503M, debt-to-assets **6.1%**.

> [!tip] A convention note before you compare with earlier notes
> [[M4-Obj-4-1]] and [[M6-Obj-6-1]] compute Tesla's conversion cycle on **average** balances (DSI 57.3 / DSO 17.3 / DPO 60.7 → CCC +13.9 days). This note computes on **ending** balances (58.19 / 17.61 / 62.78 → CCC +13.0 days). Both are correct for their purpose: average balances describe a *flow* over the year, while ending balances describe the balance sheet you are forecasting — and the forecast must start from the balance sheet that actually exists on December 31. Same firm, same filing, different question.

#### The FY2026 assumption set (instructor-set)

| # | Assumption | Value | Basis / label |
|---|---|---|---|
| 1 | Revenue growth | **+10.0%** → 104,310 | instructor-set |
| 2 | Cost of revenues | **82.0%** of sales → 85,534 | FY2025 actual 81.97% |
| 3 | R&D | **6.8%** of sales → 7,093 | FY2025 actual 6.76% |
| 4 | SG&A | **6.2%** of sales → 6,467 | FY2025 actual 6.15% |
| 5 | Restructuring and other | **500** | recurring: two consecutive years (684, then 494) per [[M6-Obj-6-2]] §II.3 |
| 6 | Depreciation and amortization | **7,000** | FY2025 6,148, rising with the capacity ramp |
| 7 | Capital expenditures | **10,000** | FY2025 8,527; instructor-set |
| 8 | Interest expense | 8,376 × 4.04% = **338** | FY2025 embedded rate on existing debt |
| 9 | Interest income | **1,680** | held flat |
| 10 | Other income (expense) | **0** | assumed away |
| 11 | Tax rate | **27.0%** | FY2025 effective rate 26.96% |
| 12 | Dividends | **0** | the 10-K states Tesla has **never** paid a cash dividend |
| 13 | Receivables | **17.61 days** of sales → 5,034 | FY2025 ending balance |
| 14 | Inventory | **58.19 days** of cost of revenues → 13,636 | FY2025 ending balance |
| 15 | Payables | **62.78 days** of cost of revenues → 14,713 | FY2025 ending balance |
| 16 | Accrued liabilities, deferred revenue, other long-term liabilities, non-operating assets | held at FY2025 levels | simplification (disclosed below) |
| 17 | Cash and short-term investments | **44,059** | fortress liquidity policy |

#### Step 1–2: projected income statement (FY2026)

| Line | FY2025 actual | FY2026 forecast | Note |
|---|---:|---:|---|
| Total revenues | 94,827 | **104,310** | +10.0% |
| Cost of revenues | 77,733 | **85,534** | 82.0% of sales |
| Gross profit | 17,094 | **18,776** | 18.00% |
| Research and development | 6,411 | **7,093** | 6.8% of sales |
| Selling, general and administrative | 5,834 | **6,467** | 6.2% of sales |
| Restructuring and other | 494 | **500** | held as recurring |
| Total operating expenses | 12,739 | **14,060** | |
| **Income from operations (EBIT)** | **4,355** | **4,716** | margin **4.52%** vs. 4.59% |
| Interest income | 1,680 | **1,680** | held flat |
| Interest expense | (338) | **(338)** | 4.04% on existing debt |
| Other income (expense), net | (419) | **0** | assumed away |
| Income before income taxes | 5,278 | **6,058** | |
| Provision for income taxes | 1,423 | **(1,636)** | 27.0% |
| **Net income** | **3,855** | **4,422** | |
| Dividends | 0 | **0** | no dividend policy |
| **Addition to retained earnings** | 3,855 | **4,422** | |

#### Step 3–4: projected balance sheet and the plug

| Line | Dec 31, 2025 | Dec 31, 2026 forecast | Driver |
|---|---:|---:|---|
| Cash and short-term investments | 44,059 | **44,059** | held at target |
| Accounts receivable | 4,576 | **5,034** | 17.61 days |
| Inventory | 12,392 | **13,636** | 58.19 days of cost of revenues |
| Prepaid, other current, lease vehicles, energy systems, digital assets | 18,139 | **18,139** | held flat |
| Property, plant and equipment, net | 40,643 | **43,643** | 40,643 + 10,000 − 7,000 |
| Right-of-use assets | 6,027 | **6,027** | held flat |
| Deferred tax assets | 6,925 | **6,925** | held flat |
| Other non-current assets | 5,045 | **5,045** | held flat |
| **Total assets** | **137,806** | **142,507** | |
| Accounts payable | 13,371 | **14,713** | 62.78 days |
| Accrued liabilities and other | 13,279 | **13,279** | held flat |
| Deferred revenue (current + non-current) | 7,055 | **7,055** | held flat |
| Debt and finance leases | 8,376 | **8,376** | no new borrowing assumed |
| Other long-term liabilities | 12,860 | **12,860** | held flat |
| **Total liabilities** | **54,941** | **56,283** | |
| Common stock + APIC + AOCI | 43,134 | **43,134** | no issuance assumed |
| Retained earnings | 39,003 | **43,425** | + 4,422 |
| **Stockholders' equity** | **82,137** | **86,559** | |
| Noncontrolling and redeemable interests | 728 | **728** | held flat |
| **Total liabilities and equity** | **137,806** | **143,570** | |
| **EFN** | — | **−1,063** | **surplus: the plan is self-funding** |

**Cash reconciliation (the proof).** Net income 4,422 + D&A 7,000 − CapEx 10,000 − working-capital investment 359 − dividends 0 = **+1,063**. The balance sheet and the cash statement agree, so the model is internally consistent.

**What the plug is telling you.** Tesla's base-case FY2026 plan needs **no external financing and generates \$1,063M of surplus**. Read that carefully: the surplus is not a growth dividend, it is cash that the plan does not need — sitting on a balance sheet that already holds \$44,059M of cash and investments. And note what produced it: **earnings of \$4,422M plus \$7,000M of non-cash depreciation against \$10,000M of capital spending.** If capital intensity rises without a matching earnings response, the surplus disappears; that is precisely the stress tested in [[M7-Obj-7-2]].

> [!danger] Five disclosures this forecast owes its reader
> 1. **Depreciation sits inside cost of revenues and opex here** (GAAP presentation), whereas the Titan case models it as a separate line. Same economics, different visibility — reconcile the two before comparing margins.
> 2. **Nine balance-sheet lines are held flat** (accrued liabilities, deferred revenue, other long-term liabilities, ROU, deferred tax assets, other non-current assets, non-operating current assets). In a real model they scale, amortize, or unwind. Holding them flat is conservative on assets and aggressive on the plug.
> 3. **All growth and margin assumptions are instructor-set.** They are not Tesla guidance, not consensus, and not derived from the filing.
> 4. **The plug is computed pre-financing.** If EFN were positive, the new borrowing would carry interest, which would reduce net income and retained earnings, which would change the plug — the model becomes iterative (the Titan case sidesteps this by assuming new-debt interest is paid in 2026). Our base case has EFN < 0, so no new debt arises and the circularity stays dormant.
> 5. **Cash is assumed to earn nothing and the cash balance is assumed to stay put.** A \$44,059M cash pile is an *investment* decision (interest income of \$1,680M, roughly 3.8% on the average balance) and a *resilience* asset ([[M6-Obj-6-1]] §IV) — not a line item to be plugged.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Pro forma statement** | Forward-looking financial report built on explicit assumptions about revenue, costs, capital spending, and financing |
| **Sales anchor** | The projected revenue line that every other forecast line is tied to |
| **Percentage-of-sales method** | Projecting each cost line as a historical ratio applied to projected sales |
| **Fixed vs. variable distortion** | Percentage-of-sales costs miss the operating leverage embedded in fixed overhead |
| **Embedded cost of debt** | The interest rate the firm actually pays on existing debt (interest expense ÷ average debt), applied to projected debt |
| **DSO / DSI / DPO** | Days of sales in receivables; days of cost of revenues in inventory; days of cost of revenues in payables — the velocity anchors for the working-capital forecast |
| **PP&E roll-forward** | Ending net PP&E = beginning net PP&E + CapEx − depreciation |
| **Retained-earnings roll-forward** | Ending RE = beginning RE + projected net income − projected dividends |
| **EFN (external financing needed)** | Projected total assets − (projected total liabilities + projected total equity); the model's balancing plug |
| **Surplus EFN** | Negative EFN: internal cash generation exceeds the plan's investment needs |
| **Absorption choice** | Whether the gap is funded with debt, equity, or cash — each with a different cost and a different disclosure obligation |
| **Iterative model** | A model where the plug affects earnings, which affects the plug — resolved by assumption or by iteration |
| **Assumption register** | The complete list of assumptions a forecast depends on, disclosed alongside the output |

---

> [!danger] Red Flags — Forecasting Discipline
> - A projected number that cannot be traced to an assumption, a historical ratio, or another projected line
> - Percentage-of-sales costs held flat across a volume swing in a fixed-heavy business
> - A negative EFN reported as "we have plenty of cash" without disclosing that the surplus was absorbed by the balance sheet
> - Cash pushed below its operating minimum to make a statement balance
> - A plug that includes interest on the borrowing it is supposed to size (and is therefore wrong by construction)
> - Equity issued without quantifying dilution, or dividends assumed without a payout policy
> - Working-capital ratios computed on a different balance convention than the historical comparison in the same deck
> - A forecast presented as a prediction, with no sensitivity analysis attached ([[M7-Obj-7-2]])

---

### Review Questions

> [!question]- Q1: Why is sales revenue called the "common denominator" of the forecast, and what happens to a model if it is set wrongly?
> Because every cost ratio, working-capital anchor, and margin in the model is expressed against revenue, an error in the anchor propagates through the entire statement: a 5% revenue overstatement inflates cost-of-revenue projections by 5% of sales, inflates receivables and inventory at their day rates, and shifts the EFN plug — while leaving the *percentage* margins looking perfectly plausible. The tell is that percentage-based outputs (margins, ratios) look reasonable while the dollar outputs are wrong.

> [!question]- Q2: Why does holding the cost-to-sales ratio flat understate cost in a downturn and overstate cost in growth?
> Because the ratio blends fixed and variable costs. In growth, the fixed block is spread over more units, so the true ratio *falls* — holding it flat overstates cost and understates margin. In contraction the fixed block is spread over fewer units, so the true ratio *rises* — holding it flat understates cost and overstates margin. This is operating leverage ([[M6-Obj-6-1]] §II.2) showing up in a forecast instead of in a historical analysis.

> [!question]- Q3: A model produces EFN = −650. Name the three legitimate ways to absorb it and the fourth, illegitimate one.
> Legitimate: let cash accumulate above the target balance; repay debt; distribute to shareholders. Illegitimate: reduce the cash balance below the operating minimum so the statement "balances" while the liquidity that funded the plan quietly disappears.

> [!question]- Q4: Why must the plug be computed *before* financing in a first-pass model, and what is the consequence of ignoring that?
> Because the plug is the *output* that sizes the financing; if you compute it after assuming the financing, the two are circularly dependent. Ignoring the circularity understates the cost of the gap: new debt brings interest, which lowers net income and retained earnings, which increases the gap it was supposed to fill. Titan's case avoids the issue by assuming interest on new borrowing is paid in 2026.

> [!question]- Q5: In Tesla's FY2026 forecast, the base case shows a \$1,063M surplus. Name the two largest arithmetic contributors and explain why that surplus is not free money.
> Earnings of \$4,422M and depreciation of \$7,000M, against \$10,000M of capital spending — i.e., the surplus exists because accounting earnings plus non-cash charges exceeded the plan's investment needs. It is not free money because it is cash the plan does not need sitting on a balance sheet that already holds \$44,059M of cash and investments; it is a choice (hold, repay, or distribute) and it disappears if capital intensity rises without an earnings response.

> [!question]- Q6: Your forecast holds nine balance-sheet lines flat "to keep it simple." Why is that a disclosure, not a simplification?
> Because "flat" is an assumption with a direction: holding non-operating assets flat understates the investment the business must make to grow, while holding accrued liabilities and deferred revenue flat removes a working-capital source that a scaling business would normally enjoy. Both biases run in the same direction — they flatter the plug. A reader is entitled to know that the surplus in the plug is partly an artifact of the simplifications.

---

### Practice Activity

> [!tip] Warm-up path
> New to the material? Do tasks 1–3 with §II open in front of you; tasks 4–5 belong after the Module 7 quiz.

You are the analyst building the FY2026 plan for Tesla, using the §IV base and the assumption set:

1. **Re-derive the anchors.** Compute DSO, DSI, and DPO from the FY2025 filing balance sheet and the income statement, and state the formula for each in one line. Then compute the FY2026 projected receivables, inventory, and payables *yourself* and compare with §IV — any difference is a modeling error, not a rounding difference.
2. **Rebuild the income statement.** Compute projected revenue, cost of revenues, R&D, SG&A, EBIT, pre-tax income, tax, and net income. Then compute the **EBIT margin** and compare it with FY2025's 4.59%. In one sentence: did the base case assume margin expansion or compression, and where did the assumption come from?
3. **Compute the plug two ways.** (a) EFN from the projected balance sheet. (b) A cash reconciliation: net income + D&A − CapEx − working-capital investment − dividends. The two must agree; if they do not, find your error. State the reconciliation as your proof.
4. **Change one assumption.** Re-run the model with revenue growth of **0%** and everything else unchanged. Compute the new EFN, then explain in two sentences why the *earnings* fell more than the *financing need*.
5. **Write the plan sentence.** One sentence for the credit committee that quotes the projected EBIT, the EFN, and one assumption you had to make — and states what would have to change for the plug to turn positive.

---

### Related Notes

- [[M7-Overview]] — Module 7 overview
- [[M7-Obj-7-2]] — Next: stress the forecast's assumptions and find the break-even points
- [[M7-Obj-7-3]] — then: value the projected cash flows (DCF and multiples)
- [[M2-Obj-2-1]] — the classified balance sheet; Tesla's debt schedule, leases, and the D&A that drives the PP&E roll-forward
- [[M2-Obj-2-3]] — cash-flow statement; the working-capital movements behind the DSO/DSI/DPO anchors
- [[M3-Obj-3-1]] — margin ratios and the DuPont machinery behind the cost-ratio assumptions
- [[M4-Obj-4-1]] — DSI/DSO/DPO for Tesla and BYD (average-balance convention)
- [[M5-Obj-5-3]] — regulatory credits and the core-earnings stack; why restructuring is forecast as recurring
- [[M6-Obj-6-1]] — operating leverage (§II.2) and the equity cushion that makes a negative EFN survivable
- [[M6-Obj-6-2]] — the serial-restructurer test (§II.3) and the pro-forma mirage this method can create

---

> [!info] Sources
> - Tesla, Inc. FY2025 Form 10-K (filed Jan 2026), SEC EDGAR (accession `0001628280-26-003952`) — consolidated statements of operations, balance sheet, and cash flows; dividend policy; share counts
> - Market data: 3,751M shares issued and outstanding at Dec 31, 2025 (10-K balance sheet parenthetical); diluted weighted-average shares 3,528M; TSLA close \$449.72 (Dec 31, 2025)
> - Titan Dynamics worked case compiled from the course reference: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed), Part IV (Ch. 12 & 14, "Forecasts and Security Analysis")
> - All Tesla forecast assumptions in §IV are instructor-set for teaching; no forecast in this note is Tesla guidance
> - Cross-referenced Tesla figures validated in [[M2-Obj-2-1]], [[M2-Obj-2-3]], [[M4-Obj-4-1]], and [[M6-Obj-6-1]]
