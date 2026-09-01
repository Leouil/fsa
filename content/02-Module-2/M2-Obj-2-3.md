---
title: M2-Obj-2-3 - Deconstructing the Statement of Cash Flows
date: 2026-08-22
tags:
  - FSA
  - M2
  - Objective-2-3
  - Cash-Flow-Statement
aliases:
  - cash-flow-analysis
  - statement-of-cash-flows
  - free-cash-flow
---

# Learning Objective 2.3

## Deconstruct the Statement of Cash Flows to evaluate internal cash generation, corporate life cycles, financial flexibility, and strategic cash flow manipulation

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc.
> Throughout this note we use Tesla's FY2025 Form 10-K (fiscal year ended December 31, 2025) as our running example. Key consolidated cash flow figures (in millions):

| Section | 2025 | 2024 | 2023 |
|-----------|-----:|-----:|-----:|
| **Operating Activities (CFO)** | | | |
| Net Income | \$3,855 | \$7,153 | \$14,974 |
| Stock-Based Compensation | \$2,825 | \$1,999 | \$1,812 |
| Depreciation & Amortization (est.) | ~\$3,500 | ~\$3,200 | ~\$2,900 |
| Digital asset loss/(gain), net | \$68 | (\$589) | — |
| Deferred income taxes | \$123 | \$477 | (\$6,349) |
| Changes in operating assets/liabilities (net) | +\$1,374 | +\$2,083 | +\$1,586 |
| **Net Cash Provided by Operating Activities** | **\$14,747** | **\$14,923** | **\$13,256** |
| **Investing Activities (CFI)** | | | |
| Purchases of PPE (CapEx) | (\$8,527) | (\$11,342) | (\$8,899) |
| Purchases of investments | (\$37,109) | (\$35,955) | (\$19,112) |
| Proceeds from maturities/sales of investments | \$30,158 | \$28,510 | \$12,491 |
| **Net Cash Used in Investing Activities** | **(\$15,478)** | **(\$18,787)** | **(\$15,584)** |
| **Financing Activities (CFF)** | | | |
| Proceeds from debt issuances | \$5,586 | \$5,744 | \$3,931 |
| Repayments of debt | (\$5,546) | (\$2,500) | (\$1,351) |
| Proceeds from stock options/issuances | \$1,186 | \$1,241 | \$700 |
| Principal payments on finance leases | (\$104) | (\$381) | (\$464) |
| NCI distributions/buyouts | (\$78) | (\$237) | (\$198) |
| **Net Cash Provided by Financing Activities** | **\$1,139** | **\$3,853** | **\$2,589** |
| **Free Cash Flow (CFO − CapEx)** | **\$6,220** | **\$3,581** | **\$4,357** |

> *D&A not separately disclosed in Tesla's cash flow statement; estimated from PP&E rollforward and footnotes. Free Cash Flow = CFO − CapEx.*

---

### I. The Core Philosophy of Cash Flow: Why Profits Are Not Cash

#### The Malleability of Profit

Over time, accrual net income has proven highly malleable — easily enlarged, reduced, or smoothed by corporate management to meet expectations. Accrual accounting uses estimates, timing allocations, and bookkeeping assumptions that can obscure real economic health.

#### The Ultimate Reality Check

The Statement of Cash Flows serves as the final "reality check" for a business. Many highly profitable corporations on paper have collapsed into bankruptcy because they failed to generate actual cash from operations.

> [!example] Tesla: Profits Vanished, Cash Engine Ran
> **2023 → 2025**: Tesla's net income **collapsed 74%** (\$14,974M → \$3,855M) — yet **CFO held steady and grew** (\$13,256M → \$14,747M, +11%).
>
> | Driver | 2023 | 2025 | Change |
> |---|---:|---:|---:|
> | Net Income | \$14,974M | \$3,855M | **−\$11,119M** |
> | SBC | \$1,812M | \$2,825M | +\$1,013M |
> | D&A (est.) | ~\$2,900M | ~\$3,500M | +\$600M |
> | Digital asset swing | — | \$68M loss | +\$68M |
> | Deferred tax swing | (\$6,349M) | +\$123M | +\$6,472M |
> | Working capital | +\$1,586M | +\$1,374M | −\$212M |
> | **CFO** | **\$13,256M** | **\$14,747M** | **+\$1,491M** |
>
> The "profit disappearance" was largely **non-cash**: a massive deferred tax *benefit* in 2023 (from releasing a valuation allowance) reversed to an expense in 2025, and SBC/D&A grew. The cash-generating capacity of the business — selling cars, collecting cash, paying suppliers — actually **improved**.

#### The Case of Nocash Corporation (Revisited)

This classic scenario illustrates how a company can go broke while showing a profit on paper:
- Year 2: Nocash reports **\$30,000 accrual net income**
- But liberal credit terms → **AR +\$20,000** (revenue booked, cash not collected)
- Overproduction → **Inventory +\$15,000** (cash spent, not yet sold)
- Paid suppliers → **AP −\$5,000** (cash out)
- **Result: CFO = −\$10,000** — a cash deficit despite "profit"
- Nocash borrows \$10,000 to survive — "selling itself out of business" to fund unprofitable growth

---

### II. Systematic Classification of Cash Flows

Under **SFAS 95** (mandatory for fiscal years ending after July 15, 1988), cash flows must be classified into three distinct categories:

```
                      ┌─────────────────────────────────┐
                      │   TOTAL CHANGE IN CASH & EQUIV  │
                      └────────────────┬────────────────┘
                                       │
          ┌────────────────────────────┼────────────────────────────┐
          ▼                            ▼                            ▼
┌─────────────────┐          ┌─────────────────┐          ┌─────────────────┐
│ OPERATING (CFO) │          │ INVESTING (CFI) │          │ FINANCING (CFF) │
└─────────────────┘          └─────────────────┘          └─────────────────┘
```

#### 1. Operating Activities (CFO)

**Plain-language definition:** cash generated from the company's **core day-to-day business** — selling its goods and services. This is the engine that pays the bills; a healthy company generates positive CFO consistently, independent of how it is funded.

**Rule of thumb:** *"Would a corner store see this cash from just running the shop?"* Cash tied to making, selling, and collecting on the product — plus the taxes and interest that go with running it — is operating. Under U.S. GAAP this bucket also includes **interest paid** and **dividends received** (surprising to many students, since both feel "financial"; note the asymmetry with dividends *paid*, which sit in CFF).

Transactions that enter into the determination of net income and reflect the delivery of goods or services.

| Inflows | Outflows |
|---------|----------|
| Cash from sales of goods/services | Payments for inventory |
| Returns on equity securities (dividends) | Payments for operating expenses (salaries, rent) |
| Returns on interest-earning assets (interest) | Payments to trade suppliers |
| | Interest paid to lenders |
| | Income taxes paid |

**Tesla's CFO Composition (2025):**
- **Core**: Cash collected from customers (auto, energy, services)
- **Working capital boost**: AP/accrued **+\$4,376M** (vendor financing), Deferred revenue **+\$363M** (FSD/connectivity prepayments)
- **Working capital drag**: Prepaid/other assets **−\$3,181M** (restricted cash, supplier advances, MyPower loans), Inventory **−\$630M**, AR **−\$261M**
- **Non-cash add-backs**: SBC **\$2,825M**, D&A **~\$3.5B**, Digital asset loss **\$68M**

> [!warning] Analytical Note
> Tesla's CFO is propped up by **accounts payable growth** (+\$4.4B in 2025, +\$3.6B in 2024). If AP growth slows, CFO will drop sharply unless operating margins recover. This is a form of **supplier financing** — watch for sustainability.

#### 2. Investing Activities (CFI)

**Plain-language definition:** cash tied to the company's **future** — buying or selling long-term productive assets (factories, equipment, intangibles, acquisitions) and financial investments. Positive net CFI is usually negative or near-zero, because a growing business spends more on CapEx than it collects from asset sales.

**Rule of thumb:** *"Is the corner store buying its building and bakery ovens, or selling them off?"* CapEx on productive assets, purchases/maturities of securities, loans made or collected, and business acquisitions or divestitures all live here. But note: **interest received** is classified as operating under U.S. GAAP, though it arises from investment-like holdings — another FASB quirk to keep straight.

Acquisition and disposal of long-term productive assets and debt/equity securities.

| Inflows | Outflows |
|---------|----------|
| Sale of PP&E | Purchases of PP&E (CapEx) |
| Loan principal collections | Loans made to others |
| Sale of debt/equity securities of others | Purchases of debt/equity securities of others |
| Sale of business segment | Business acquisitions |

**Tesla's CFI Composition (2025):**
- **CapEx**: **\$8,527M** — Gigafactories (TX, Berlin, Shanghai), AI infrastructure, Supercharger network
- **Investment portfolio churn**: **\$37,109M purchases** vs **\$30,158M maturities** — massive short-term investment turnover (trading securities classified as investing, but *trading gains/losses may leak into CFO*)
- **Net CFI: −\$15,478M** — Tesla is a heavy reinvestor

> [!tip] CapEx in Liabilities
> Supplemental disclosure shows **\$1,913M of CapEx included in liabilities** (2025) — accrued but unpaid. True cash CapEx > reported CapEx. Analysts should add this to CapEx for true free cash flow.

#### 3. Financing Activities (CFF)

**Plain-language definition:** cash exchanged with the people who **fund** the company — creditors (lenders) and owners (shareholders). This reveals how the company raises and returns capital: does it lean on debt or equity, and does it return cash via dividends or buybacks?

**Rule of thumb:** *"How is the corner store paying for everything — borrowing from the bank, taking in money from owners, or paying them back?"* Proceeds from borrowing, debt repayments, equity issuance, share repurchases, and **cash dividends paid** all belong here. Dividends paid are **CFF** (an outflow to owners); dividends received are **CFO** (an operating inflow) — a pairing worth memorizing.

Transactions with creditors and equity owners — capital structure management.

| Inflows | Outflows |
|---------|----------|
| Proceeds from borrowing (short/long-term) | Repayments of debt principal |
| Proceeds from issuing equity | Repurchase of own shares (treasury stock) |
| | Payment of cash dividends |

**Tesla's CFF Composition (2025):**
- **Debt treadmill**: Issued **\$5,586M**, repaid **\$5,546M** — net ~\$0. Rolling short-term facilities.
- **Equity issuances**: **\$1,186M** — mostly stock option exercises (not primary capital raises)
- **No dividends, no buybacks** — all cash retained for growth
- **Net CFF: \$1,139M** — minimal net financing; business largely self-funded at this stage

---

### III. Mechanics: The Indirect Method Reconciliation

Because double-entry bookkeeping balances, a change in the cash account equals the sum of changes in all other balance sheet accounts:

$$\Delta\text{Cash} = \Delta\text{Liabilities} + \Delta\text{Equity} - \Delta\text{Non-Cash Assets}$$

**Inflow Triggers:** Decrease in asset (sell inventory, collect AR) or Increase in liability/equity (borrow, issue stock)
**Outflow Triggers:** Increase in asset (buy PPE, build inventory) or Decrease in liability/equity (repay debt, pay dividends)

#### The Indirect Method Formula

$$\text{CFO} = \text{Net Income} + \text{Non-Cash Expenses} \pm \text{Non-Operating Gains/Losses} \pm \Delta\text{Working Capital}$$

**Tesla 2025 Walkthrough:**

| Step | Adjustment | Amount | Logic |
|---|---|---:|---|
| 1 | Start: Net Income | +\$3,855 | Accrual bottom line |
| 2 | Add: SBC | +\$2,825 | Non-cash, dilutive |
| 3 | Add: D&A (est.) | +~\$3,500 | Non-cash allocation |
| 4 | Add: Digital asset loss | +\$68 | Fair-value, nonoperating |
| 5 | Add: Deferred tax increase | +\$123 | Tax expense > cash paid |
| 6 | Adjust: AR increase | −\$261 | Revenue > collections |
| 7 | Adjust: Inventory increase | −\$630 | Cash spent > COGS |
| 8 | Adjust: Prepaid/other increase | −\$3,181 | Cash out for future benefit |
| 9 | Adjust: AP/accrued increase | +\$4,376 | Bought on credit, cash kept |
| 10 | Adjust: Deferred revenue increase | +\$363 | Collected cash, not earned |
| | **= CFO** | **\$14,747** | |

> [!example] The "Big Three" Working Capital Levers for Tesla
> 1. **AP/Accrued (+\$4.4B)** — biggest CFO booster; vendor financing
> 2. **Prepaid/Other Assets (−\$3.2B)** — biggest CFO drag; opaque bucket
> 3. **Deferred Revenue (+\$0.4B)** — growing FSD/connectivity liability = cash collected early

---

### IV. Analytical Frameworks for Cash Flow Evaluation

#### 1. Cash Flow and the Business Life Cycle

| Life Cycle Stage | Sales | Net Income | CFO | CFI | CFF |
|---|---|---|---|---|---|
| **Start-Up** | Near Zero | Deep Loss | Strongly (−) | (−) CapEx | Strongly (+) VC/Equity |
| **Emerging Growth** | Rapid Rise | Loss → Profit | (−) to Flat | Strongly (−) | Strongly (+) Outside capital |
| **Established Growth** | High Growth | Profitable | **(+)** | Strongly (−) | Varies |
| **Mature** | Stable | Highly Profitable | Strongly (+) | (−) Maint. CapEx | Strongly (−) Divs/Buybacks |
| **Declining** | Decreasing | Shrinking/Loss | (−) | Flat/(+) Divest | Strongly (−) Debt paydown |

**Tesla's Life Cycle Position: Established Growth → Early Maturity**

| Metric | 2023 (Hyper-Growth) | 2025 (Established) |
|---|---|---|
| Revenue | \$96.8B | \$94.8B |
| Net Income | \$15.0B | \$3.9B |
| CFO | \$13.3B | \$14.7B |
| CapEx | \$8.9B | \$8.5B |
| Free Cash Flow | \$4.4B | **\$6.2B** |
| CFF | +\$2.6B | +\$1.1B |

- **2023**: Explosive profit, heavy external financing (emerging growth)
- **2025**: Profit compressed, **FCF doubled**, minimal net financing (established maturity)
- **Signal**: Tesla is transitioning from "funded by investors" to "funded by operations" — but FCF is still **100% reinvested** (no dividends/buybacks)

#### 2. Financial Flexibility and Cash "Slack"

**Financial flexibility** = capacity to sustain CapEx, pay obligations, and weather downturns without high-cost external capital.

**Tesla's Flexibility Assessment (2025):**
- **CFO \$14.7B** > **CapEx \$8.5B** = **\$6.2B discretionary FCF**
- **Cash + ST investments = \$44.1B** — massive liquidity buffer
- **Debt minimal** (\$8.4B total vs \$137.8B assets = 6% debt-to-assets)
- **No near-term maturities wall** — debt well-laddered

> [!info] Tesla's Slack
> Tesla carries **more cash than total debt** — a rare position for a capital-intensive manufacturer. This "fortress balance sheet" lets it: (1) fund \$20B+ 2026 CapEx internally, (2) retain talent in downturns, (3) out-invest competitors when credit tightens. The risk: **cash drag** if returns on \$44B cash/investments are low.

> [!tip] What Lenders Actually Watch
> Particularly for a highly levered borrower, creditors do **not** rely on reported net income — which can be a large negative while debt is being serviced. They focus on **cash generation available to service debt**, measured as **CFO − CapEx** (free cash flow), and the **debt-paydown trajectory** those cash flows imply. The lesson generalizes: a company's *ability to repay* is a cash-flow question, not an earnings question.

---

### V. Advanced Detective Analysis: Spotting Cash Flow Manipulations

Proactive analysts do not take CFO at face value. Managers use several techniques to artificially inflate CFO:

```
                ┌─────────────────────────────────────┐
                │    STRATEGIES TO ARTIFICIALLY       │
                │            INFLATE CFO              │
                └──────────────────┬──────────────────┘
                                   │
       ┌───────────────────────────┼───────────────────────────┐
       ▼                           ▼                           ▼
┌──────────────┐            ┌──────────────┐            ┌──────────────┐
│ Capitalizing │            │ Receivable   │            │ Managing     │
│ Operating    │            │ Factoring    │            │ Supplier     │
│ Expenses     │            │  (Sales)     │            │ Payables     │
└──────────────┘            └──────────────┘            └──────────────┘
```

#### 1. Capitalizing Operating Expenses
- **Scheme**: Reclassify OpEx (maintenance, line costs) as CapEx
- **Double distortion**: NI overstated (slow depreciation vs. immediate expense); **CFO overstated** (cash outflow moves to CFI)
- **Tesla check**: CapEx is transparent (\$8.5B, disclosed by segment); no evidence of OpEx capitalization. But **CapEx in liabilities (\$1.9B)** warrants scrutiny — are payables to contractors being stretched?

#### 2. Accounts Receivable Factoring
- **Scheme**: Sell receivables to a factor → accelerates collections, drops AR, boosts CFO
- **Tesla check**: Tesla **originates and sells** some vehicle loans (MyPower, leasing partnerships). Disclosed in AR footnote (\$247M current, \$554M non-current financing receivables). **Not factoring** — these are held or sold via structured VIEs (Note 14). No artificial AR reduction detected.

#### 3. Supplier Payables Management (Stretching Payables)
- **Scheme**: Delay supplier payments near quarter-end → AP spikes → CFO boost
- **Sage Inc. (source text)**: CFO turned from −\$3,767K to +\$10,024K driven by **AP surge of \$6,703K** — not core performance

> [!danger] Tesla's AP Surge
> Tesla's AP/accrued grew **+\$4,376M (2025)** and **+\$3,588M (2024)** — **\$7.9B cumulative in two years**.
> - Revenue roughly flat (\$97.7B → \$94.8B)
> - AP grew from ~\$12.5B to ~\$17.5B (estimated from accrued liabilities line)
> - **Days Payable Outstanding (DPO) likely increased significantly**
> - **Skeptical question**: Is Tesla stretching vendors to fund operations? If AP growth reverses, CFO drops by billions.

#### 4. Classifying Non-Operating Items in CFO
- **Scheme**: Move investing/financing flows into CFO
- **Trading securities**: GAAP allows purchase/sale of trading securities in CFO — structurally investing, should be stripped out
- **GE (2021)**: Added back \$6.5B debt extinguishment costs to CFO (financing → operating)

> [!warning] Tesla's Investment Churn & Digital Assets
> - **Investment portfolio**: \$37B purchases / \$30B maturities in 2025 — **massive turnover**. If trading securities, gains/losses may be in CFO.
> - **Digital assets (Bitcoin)**: \$68M loss in CFO (2025) vs \$589M gain (2024) — **fair-value volatility in operating cash flow**. This is nonoperating noise.
> - **Analyst adjustment**: Strip digital asset gains/losses and investment trading gains/losses from CFO for "core CFO."

#### 5. Deferred Revenue as a CFO Booster
- Tesla collects FSD/connectivity/Supercharging cash **upfront** → deferred revenue liability → recognized over years
- 2025: **Deferred revenue +\$363M** → CFO boost
- 2024: +\$244M (from \$3,599M → \$3,867M balance)
- **Watch**: If FSD take-rate slows or regulatory changes (OBBBA) cut credit revenue, deferred revenue growth could reverse → CFO headwind

---

## Key Terms

| Term | Definition |
|------|------------|
| **Statement of Cash Flows** | Classifies cash inflows/outflows into Operating, Investing, Financing |
| **CFO (Cash Flow from Operations)** | Cash generated by core business activities |
| **CFI (Cash Flow from Investing)** | Cash from buying/selling long-term assets and securities |
| **CFF (Cash Flow from Financing)** | Cash from debt/equity issuance and repayment |
| **Free Cash Flow (FCF)** | CFO − Capital Expenditures — discretionary cash after maintaining asset base |
| **Indirect Method** | Reconciles net income to CFO by adjusting for non-cash items and working capital |
| **Working Capital** | Current assets − current liabilities (operating: AR, Inventory, AP, Accrued, Def Rev) |
| **DPO (Days Payable Outstanding)** | (AP / COGS) × 365 — how long company takes to pay suppliers |
| **Financial Flexibility** | Ability to fund operations/CapEx/debt service without external capital in a downturn |
| **Capitalizing Expenses** | Recording operating costs as assets (CapEx) to boost NI and CFO |
| **Receivable Factoring** | Selling AR to a factor for immediate cash; accelerates collections artificially |
| **Stretching Payables** | Delaying supplier payments to temporarily boost CFO via AP increase |
| **Trading Securities in CFO** | GAAP allows trading portfolio cash flows in operating — should be reclassified to investing |
| **Deferred Revenue** | Cash collected before revenue recognized; liability that boosts CFO when growing |
| **CapEx in Liabilities** | Accrued but unpaid capital expenditures; supplemental disclosure, adds to true CapEx |

---

## Red Flags to Identify

> [!danger] Cash Flow Statement Warning Signs
>
> - CFO rising while net income falling (check: non-cash add-backs, working capital one-timers)
> - AP/accrued growing faster than revenue/COGS (supplier stretching)
> - Large "Prepaid/Other Assets" increases (cash leaving for opaque purposes)
> - Digital asset / investment fair-value swings in CFO (nonoperating noise)
> - CapEx in liabilities growing (unpaid contractor bills)
> - Investment portfolio churn >> CapEx (trading gains/losses in CFO?)
> - Deferred revenue growth slowing (prepaid cash collections decelerating)
> - CFF strongly positive while CFO negative (survival via financing, not operations)
> - FCF negative for 3+ years in "established growth" stage (structural cash burn)
> - Non-GAAP "adjusted CFO" excluding recurring items (SBC, restructuring, maintenance CapEx)

---

## Review Questions

> [!question]- Why did Tesla's CFO grow (+11%) while net income collapsed (−74%) from 2023 to 2025?
> The profit drop was largely non-cash: a massive deferred tax benefit reversal (\$6.3B swing), plus growing SBC and D&A. Core cash generation from selling cars and collecting from customers actually improved.

> [!question]- What is the "supplier financing" signal in Tesla's cash flow, and why is it risky?
> AP/accrued surged +\$7.9B over 2024–2025 while revenue was flat. This vendor financing boosts CFO temporarily; if DPO normalizes or suppliers tighten terms, CFO will drop sharply without margin improvement.

> [!question]- How should an analyst adjust Tesla's CFO for "core" operating cash flow?
> Strip out: (1) Digital asset fair-value loss/gain (\$68M/−\$589M), (2) Investment trading gains/losses (from \$37B/\$30B churn), (3) One-time restructuring cash costs. Result = cleaner view of auto/energy cash engine.

> [!question]- What does Tesla's \$1.9B "CapEx in liabilities" tell you?
> True cash CapEx > reported CapEx. Contractors/suppliers for factory/AI builds are being paid on credit. Add this to CapEx for true free cash flow: FCF* ≈ \$6.2B − \$1.9B = \$4.3B.

> [!question]- In the business life cycle framework, where is Tesla in 2025 and how do you know?
> **Established Growth → Early Maturity**: High revenue, profitable, strong CFO, heavy CapEx, but **FCF positive and growing** (\$6.2B), minimal net financing need. Transitioning from investor-funded to self-funded.

> [!question]- Why is "Free Cash Flow = CFO − CapEx" insufficient for Tesla?
> It misses: (1) CapEx in liabilities (+\$1.9B), (2) Finance lease principal payments (\$104M, debt-like), (3) NCI distributions (\$78M). **Adjusted FCF ≈ CFO − CapEx − CapEx payables − finance lease principal − NCI cash**.

---

## Practice Activity

> [!example] Practice: Analyze Tesla, Inc.'s Statement of Cash Flows
>
> Open Tesla's FY2025 Form 10-K via SEC EDGAR and locate the Consolidated Statements of Cash Flows and supporting notes:
>
> 1. **Indirect Method Reconstruction**: Start with Net Income (\$3,855M) and walk through every line to arrive at CFO (\$14,747M). Identify the three largest adjustments and explain their economic meaning.
> 2. **Supplier Financing Test**: Compute the implied DPO for 2024 and 2025 using COGS + change in inventory − change in AP (simplified). Has Tesla materially extended payment terms? What happens to CFO if AP is flat in 2026?
> 3. **Core CFO Adjustment**: Strip digital asset loss (\$68M) and estimate investment trading impact (hint: \$37B purchases vs \$30B maturities suggests active portfolio). Compute "core CFO" and compare to reported.
> 4. **Free Cash Flow Reality**: Calculate FCF three ways: (a) CFO − CapEx, (b) CFO − CapEx − CapEx in liabilities, (c) CFO − CapEx − CapEx in liabilities − finance lease principal. Which best represents discretionary cash?
> 5. **Life Cycle Diagnosis**: Using the 5-stage framework, argue whether Tesla is "Established Growth" or "Early Maturity" in 2025. Cite three cash flow metrics that support your classification.

---

## Related Notes

- [[M2-Overview]] — Module 2 Overview
- [[M2-Obj-2-1]] — Deconstructing the Balance Sheet
- [[M2-Obj-2-2]] — Analyzing the Income Statement
- [[M3-Obj-3-1]] — Vertical Analysis (Common-Sizing)
- [[M3-Obj-3-2]] — Horizontal Analysis (Trend Analysis)
- [[M3-Obj-3-3]] — Ratio Analysis (Liquidity, Leverage, Turnover)
- [[M1-Obj-1-2]] — Detecting Management Gimmicks (cash flow manipulations)