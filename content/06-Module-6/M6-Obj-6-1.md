---
title: M6-Obj-6-1 - Identify Financial, Operational, and Strategic Risks
created: 2026-11-01
date: 2026-11-01
tags:
  - FSA
  - M6
  - Objective-6-1
  - Risk-Analysis
aliases:
  - risk-identification
  - liquidity-risk
  - operating-leverage
  - cash-conversion-cycle-risk
---

# Learning Objective 6.1

## Identify Financial, Operational, and Strategic Risks

**By the end of this note, you can:**
- Compute and interpret the liquidity triad (current, quick, cash-flow liquidity) — and explain the liquidity paradox
- Build the leverage and coverage picture (debt-to-capital, EBIT and cash coverage, Beaver payback) and spot covenant tripwires
- Diagnose the operational and strategic layers (CCC components, operating leverage, policy and seasonality exposures) and map *where a firm is fragile*

> [!tip] How to read this note
> Read top to bottom: the tests first (§I–III), then watch every test applied to Tesla (§IV), then work the three exam-grade cases (§V). In §V and the Review Questions, **attempt each task before expanding a solution** — the answers are collapsed on purpose. If any term feels rusty (DSI/DSO/DPO, payback, debt-to-assets), the *Related Notes* at the bottom link the exact primers.

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc. — and the Detective's Risk Diagnosis
> Module 5 deconstructed earnings quality: we learned *which* reported profits survive accrual, cash, and normalization tests. Module 6 asks the next question a lender, insurer, or long-term investor must answer: **what underlying risks do those earnings have to survive?** A clean earnings story can still sit inside a fragile business — high fixed costs, stretched supplier payments, policy-dependent revenue — and the analyst's job now is to find the vulnerabilities *before* they find the firm.
>
> This objective diagnoses risk in three layers. The running company remains **Tesla, Inc.** (FY2025 Form 10-K) — deliberately a *low*-risk calibration case, letting us see what a fortress looks like and where its residual watch items hide. The danger shapes are supplied by textbook cases compiled in the course reference (Fridson & Alvarez): **Sage Inc.** (the liquidity paradox), **Rock Solid vs. Hollowman** (operating leverage in a downturn), and **Vanguard Equipment** (covenant tripwires).

Three layers, three different clocks — hours (liquidity), quarters (coverage), and years (cushion and competitiveness):

| Layer | What can break it | Clock that matters | Core instruments |
|---|---|---|---|
| **Financial risk** | Contractual commitments: interest, lease rents, principal, payables | Days to a few years | Liquidity ratios · leverage ratios · coverage ratios · covenants |
| **Operational risk** | Working-capital stalls and fixed-cost intensity | Quarters | DSI/DSO/DPO (the CCC) · operating leverage · supplier/customer concentration |
| **Strategic & nonfinancial risk** | Recession, seasonality, weather, reputation shocks | Years | Qualitative screening the ratios systematically miss |

> [!tip] Where Module 6 Splits in Two
> 6.1 finds the risks using the statements as given. 6.2 ([[M6-Obj-6-2]]) asks whether the reporting itself hides them — because a covenant test, a liquidation value, or a bankruptcy score can pass or fail *solely because of an accounting choice*. Every risk found here has a mirror question: **is it visible in the numbers, or masked?**

---

### I. Financial Risks: Liquidity, Leverage, and Debt Service

Financial risk is a firm's exposure to **contractual financial commitments** — interest payments, lease rents, debt principal, merchandise payables — measured against liquid assets and cash-generating ability. Fixed obligations cut both ways: financial leverage amplifies equity returns in growth periods and multiplies insolvency risk in downturns.

#### 1. Short-Term Liquidity — and the Liquidity Paradox

Short-term liquidity asks whether obligations coming due can be met without catastrophic disruption. Three measures, progressively more cash-based:

$$\text{Current Ratio} = \frac{\text{Current Assets}}{\text{Current Liabilities}}$$

$$\text{Quick (Acid-Test) Ratio} = \frac{\text{Cash} + \text{Marketable Securities} + \text{Net Receivables}}{\text{Current Liabilities}} = \frac{\text{Current Assets} - \text{Inventories}}{\text{Current Liabilities}}$$

$$\text{Cash Flow Liquidity Ratio} = \frac{\text{Cash} + \text{Marketable Securities} + \text{CFO}}{\text{Current Liabilities}}$$

Each excludes the weakness of the one before: the current ratio counts **inventory and prepaids** that may be uncollectible or unsellable; the quick ratio still measures a *point in time* — balance-sheet snapshots fluctuate from one day to the next ([[M2-Obj-2-1]]), and receivables can be slow even when booked; the cash-flow liquidity ratio finally adds the statement that covers a *period* — actual operational cash generation.

> [!danger] The Liquidity Paradox
> Balance-sheet ratios can fall while true liquidity improves. A firm expanding stores and stocking inventory pushes accounts payable up — dragging the current and quick ratios down — while the same expansion positions inventory to convert into strong CFO. The **cash-flow liquidity ratio** then surges and reveals solvency improving even as the traditional ratios deteriorate. The lesson: never read a liquidity panel without the cash-flow leg (the Sage Inc. case in §V works this through in full).

#### 2. Capital Structure and the Equity Cushion

$$\text{Debt-to-Capital} = \frac{\text{Total Debt}}{\text{Total Debt} + \text{Stockholders' Equity}} \qquad \text{Debt-to-Equity} = \frac{\text{Total Debt}}{\text{Stockholders' Equity}}$$

Stockholders' equity is the **equity cushion** — the loss-absorbing layer beneath creditors. The higher the debt proportion, the thinner the cushion: in liquidation lenders stand ahead of owners, so every point of leverage increases what a given asset-value decline costs the debt holders. ([[M3-Obj-3-1]] built the same arithmetic as *debt-to-assets*: at Tesla's ~40% total-liability share, assets could lose ~60% of value before lender claims were impaired.)

#### 3. Debt Service: Coverage, Payback, and Covenant Tripwires

Earnings-based coverage must be cross-examined against cash-based coverage:

$$\text{EBIT Interest Coverage} = \frac{\text{Operating Income}}{\text{Interest Expense}} \qquad \text{Cash Interest Coverage} = \frac{\text{CFO} + \text{Interest Paid} + \text{Taxes Paid}}{\text{Interest Paid}}$$

$$\text{Beaver Debt Payback (years)} = \frac{\text{Total Debt}}{\text{CFO}}$$

- **High accrual profits do not pay interest; cash does.** A firm with robust EBIT but negative CFO from inventory build-up has a misleading EBIT coverage ([[M5-Obj-5-2]] taught the same hierarchy from the earnings side).
- **The Beaver payback** asks how many years of *all* operating cash flow would retire 100% of debt. A payback longer than the debt's average maturity creates refinancing risk in a credit crunch.
- **Covenant tripwires.** Credit agreements carry restrictive covenants — minimum interest coverage, maximum debt-to-capital, maximum payback. Breach is **technical default**: lenders gain the right to freeze dividends, accelerate repayment, or dictate operations — *before* any actual default on payments.
- **Rating trajectories.** Analysts read coverage over cycles: **cycle-to-cycle stability** (similar highs and lows across expansions and recessions) signals durable credit; **cycle-to-cycle deterioration** — successively lower highs and lower lows — signals structural decline long before a breach.

---

### II. Operational Risks: Working-Capital Velocity and Fixed-Cost Intensity

#### 1. The Cash Conversion Cycle

Operational liquidity rides on how fast an operating dollar circulates:

$$\text{Cash Conversion Cycle (CCC)} = \text{DSI} + \text{DSO} - \text{DPO}$$

| Component | Reading | Risk signal when it |
|---|---|---|
| **DSI** — days inventory held ($\text{Inventory}/\text{COGS}\times365$) | how long goods sit unsold | **rises** — glut, obsolescence, markdown risk |
| **DSO** — days sales outstanding ($\text{AR}/\text{Sales}\times365$) | how long customers withhold cash | **rises** — lenient credit, bad debt, or channel stuffing ([[M5-Obj-5-1]]) |
| **DPO** — days payable outstanding ($\text{AP}/\text{COGS}\times365$) | how long the firm holds suppliers' cash | **rises** — stretched suppliers finance operations temporarily; relationships strain, and a reversal hits CFO at once |

([[M4-Obj-4-1]] computed all three for Tesla and BYD: 57.3 / 17.3 / 60.7 vs. a deeply negative BYD cycle.)

#### 2. Operating Leverage and Fixed-Cost Intensity

Fixed operating costs (plant depreciation, property taxes, facility leases) create operating leverage: when sales fall, profit collapses *far faster than revenue*, because the fixed block cannot shrink. Variable-cost-heavy firms can shed expenses in a downturn and preserve debt-service capacity. Break-even logic generalizes: the closer a firm operates to its break-even volume, the more any revenue dip is leveraged into the bottom line.

> [!danger] The Double-Edged Sword — with a Merton-era Twist
> High operating leverage is the *operational* twin of high financial leverage, and the two compound: a cyclical sales decline hits a firm that carries both heavy fixed costs and heavy fixed interest hardest. Note the counterintuitive distress result in §V's Rock Solid/Hollowman case: **in a collapse, the asset-heavy firm's non-cash depreciation add-back lets it cover cash interest *longer* than the asset-light competitor** — accrual EBIT coverage flattered the flexible firm while cash paid the bill.

---

### III. Strategic, Environmental, and Nonfinancial Risks

Qualitative context sets the boundaries ratios operate within — and supplies the shocks ratios never see coming.

- **Macroeconomic and cyclical sensitivity.** Cyclical industries (sporting goods, capital equipment) ride recession volatility; defensive industries (packaged foods, pharmaceuticals) hold stable demand and can safely carry more debt. The *same* leverage that looks conservative in food processing is aggressive in mining.
- **Climatic dependencies and seasonality.** Weather bottlenecks (a warm winter destroying ski-equipment sales) and tight sales calendars (retailers buying inventory months before November/May peaks) create recurring quarterly cash dips independent of business execution. Seasonal working capital peaks *before* revenue does.
- **Nonfinancial, reputational, and ESG shocks.** Product-safety incidents, environmental liabilities, and governance scandals can impair brand value and equity value instantly — rendering a pristine ratio panel irrelevant. Classic illustration shapes: a fitness-equipment maker's stock dropping ~11% on product-safety placement ([[M6-Obj-6-2]] carries the litigation form of this risk), or social-media platform episodes where governance headlines move market value faster than any financial metric.

> [!warning] What No Ratio Catches
> The three strategic risks share a property: **none appears on the balance sheet until it hits.** That is precisely why LO 6.2 exists — some of what masks these risks is accounting (contingent liabilities left unrecorded, leases kept off the debt lines), and the analyst must know both the risk and the reporting apparatus around it.

---

### IV. Applying the Tests to Tesla (FY2025)

Tesla is the calibration case for risk analysis: a manufacturer with fortress financing whose residual risks concentrate in *operations* and *policy*, not in solvency.

#### Financial side — the fortress

| Test | Tesla evidence | Read |
|---|---|---|
| Debt stock | Debt **+** finance-lease obligations **\$8,376M** total (\$1,640M due within a year) [[M2-Obj-2-1]] | Modest for a global manufacturer |
| Cash tower | Cash **\$16,513M** + short-term investments **\$27,546M** = **\$44,059M** | Exceeds total debt 5:1 — internal funding for 2026 CapEx |
| Debt-to-assets (interest-bearing only) | 8,376 ÷ 137,806 ≈ **6.1%** | vs. ~40% total-liabilities share ([[M3-Obj-3-1]]) — most liabilities are supplier/operating, not borrowed |
| EBIT interest coverage | **57.0× → 20.2× → 12.9×** (FY2023–25; OI 4,355 ÷ interest 338 in FY2025) | Falling with margin compression; nowhere near any covenant range |
| Beaver payback | 8,376 ÷ CFO 14,747 ≈ **0.57 years** | Debt could be retired with ~7 months of operating cash |
| CCC | **+13.9 days** (DSI 57.3 + DSO 17.3 − DPO 60.7) [[M4-Obj-4-1]] | Fast cycle; collections under three weeks |

#### Operational side — where the risk lives

- **Operating leverage in action.** FY2024: revenue **+0.9%**, operating income **−20.4%**. FY2025: revenue **−2.9%**, operating income **−38.5%** — margin compressed 9.2% → 4.6%. Price cuts against a fixed-heavy manufacturing base (D&A rose 4,667 → 6,148) turn small top-line moves into large profit erosion: textbook operating leverage, inside a company whose *coverage* still comfortably carries it.
- **Supplier-financed CFO.** Accounts payable + accrued & other rose **≈\$3.5B** on the 2025 balance sheet (12,474 + 10,723 → 13,371 + 13,279), and the cash-flow reconciliation shows **+\$4.4B** of payables-driven working-capital relief ([[M2-Obj-2-3]]). CFO of \$14,747M leans on that stretch; if DPO normalizes, cash flow drops without any margin change — an operational risk embedded in a *healthy* ratio.
- **Inventory drift.** Inventory rose **12,017 → 12,392 (+3.1%)** against revenue **−2.0%** — a mild DSI-direction watch item consistent with (but far gentler than) the Sage-style glut in §V.

#### Strategic side — the two concentrated exposures

- **Policy-dependent revenue.** Regulatory credits (**\$1,993M**, 100% margin, **≈46% of FY2025 operating income**) phase out by law as programs tighten — a scheduled erosion, not a competitive one ([[M5-Obj-5-3]] §VI).
- **Resale-value guarantees.** Maximum exposure **\$1.45B → \$3.45B** in one year, with no income-statement effect today — a **written put** on used-car values (a promise to buy back at preset terms if resale prices fall; [[M5-Obj-5-3]] §II). Note the two-step risk: the *guarantee* is the operational/strategic risk; its *hidden reporting boundary* is the LO 6.2 subject.

> [!success] Verdict — Tesla Risk Profile
> **Financial risk: minimal and falling** — fortress liquidity, sub-one-year payback, double-digit coverage even at the margin trough. **Operational risk: moderate and specific** — fixed-cost leverage demonstrated in the 2024–25 margin path, and a CFO quality that depends on continued supplier generosity. **Strategic risk: two named exposures** — credit phase-out and resale guarantees — both *scheduled* and *monitorable*. The calibration lesson: a risk diagnosis is not a list of red flags; it is a **map of where the firm is fragile**, which for Tesla is operations and policy — precisely the areas where accounting latitude (leases, contingencies, non-GAAP packaging) matters most. That bridge is [[M6-Obj-6-2]].

---

### V. Worked Calculations

> [!tip] Before you flip any answer
> Every scenario below is exam-grade. Attempt the tasks — on paper, from the numbers alone — before expanding any solution.

#### Calculation 1: The Liquidity Paradox (Sage Inc.)

> [!example] Scenario — Sage Inc. (retailer, two consecutive fiscal years, \$ thousands)
>
> | Item | FY2024 | FY2025 |
> |---|---:|---:|
> | Cash | \$10,386 | \$9,333 |
> | Net accounts receivable | \$8,350 | \$8,960 |
> | Merchandise inventory | \$36,769 | \$47,041 |
> | Prepaid expenses & other | \$759 | \$512 |
> | **Total current assets** | **\$56,264** | **\$65,846** |
> | Accounts payable | \$7,591 | \$14,294 |
> | Accrued & other current | \$12,841 | \$13,167 |
> | **Total current liabilities** | **\$20,432** | **\$27,461** |
> | CFO | **−\$3,767** | **+\$10,024** |

**Tasks.** Compute (1) current ratio, (2) quick ratio, (3) cash-flow liquidity ratio for both years; (4) explain why traditional ratios deteriorate while cash liquidity more than doubles.

> [!success]- Solution
> **(1) Current ratio:** FY2024 = 56,264 / 20,432 = **2.75×** → FY2025 = 65,846 / 27,461 = **2.40×** (deteriorating).
>
> **(2) Quick ratio:** FY2024 = (10,386 + 8,350) / 20,432 = **0.92×** → FY2025 = (9,333 + 8,960) / 27,461 = **0.67×** (deteriorating faster).
>
> **(3) Cash-flow liquidity:** FY2024 = (10,386 + 0 − 3,767) / 20,432 = **0.32×** → FY2025 = (9,333 + 0 + 10,024) / 27,461 = **0.70×**.
>
> **(4) The paradox resolved.** Current and quick ratios fell because accounts payable nearly doubled (**7,591 → 14,294, +88.3%**) as Sage opened stores and built a seasonal inventory (36,769 → 47,041) ahead of peak selling. FY2024 itself carried a cash crunch (CFO **−\$3,767**) after a recession trapped inventory; the expansion of *trade credit* — not borrowing — funded the move. In FY2025 the inventory sold through and CFO swung to **+\$10,024**, so the cash-flow liquidity ratio **doubled (0.32× → 0.70×)** even as the snapshot ratios sagged. The supplier, not the snapshot, was the liquidity source.

#### Calculation 2: Operating Leverage in a Downturn (Rock Solid vs. Hollowman)

> [!example] Scenario — two competitors, identical baseline revenue and coverage
> Both earn gross margin **\$240.0M**, pay SG&A **\$40.0M** (fixed), interest **\$100.0M**, tax rate **40%** in the baseline year. Rock Solid is asset-heavy (depreciation **\$75.0M**); Hollowman is asset-light (depreciation **\$30.0M**). A recession cuts gross margins 40%, to **\$144.0M**; fixed costs do not move.

**Tasks.** Compute (1) baseline EBIT, net income, EBIT interest coverage for both; (2) the same in recession; (3) recessionary EBITDA interest coverage; (4) explain who survives longer and why.

> [!success]- Solution
> **(1) Baseline.** Rock Solid: EBIT = 240 − 40 − 75 = **\$125.0M**; NI = (125 − 100) × 0.60 = **\$15.0M**; coverage = 125/100 = **1.25×**. Hollowman: EBIT = **\$170.0M**; NI = **\$42.0M**; coverage = **1.70×** — the asset-light firm looks *safer* on every accrual measure.
>
> **(2) Recession.** Rock Solid: EBIT = 144 − 40 − 75 = **\$29.0M**; coverage = **0.29×**; pretax **−\$71.0M** → NI **−\$42.6M**. Hollowman: EBIT = **\$74.0M**; coverage = **0.74×**; pretax **−\$26.0M** → NI **−\$15.6M**. Both cover *cash* interest only via add-backs.
>
> **(3) EBITDA coverage.** Rock Solid: (29 + 75)/100 = **1.04×**. Hollowman: (74 + 30)/100 = **1.04×** — identical, and both barely above 1.0.
>
> **(4) Who survives.** Both post severe accrual losses; both EBITDA coverages are borderline. But Rock Solid's **\$75M depreciation is non-cash**: its cash operating cushion over interest is larger for longer, and its cost structure cannot shrink but also cannot starve cash service immediately. Hollowman's variable-heavy structure drains liquid cash quickly as revenue collapses. Two 1.04× EBITDA coverages hide opposite cash-death trajectories — which is why coverage must be read with cost-structure and cash-flow context, not in isolation.

#### Calculation 3: Covenant Tripwires (Vanguard Equipment)

> [!example] Scenario — Vanguard Equipment Corp. (\$ thousands)
> Total debt **\$180,000** (\$50,000 short-term notes + \$130,000 long-term bonds). Covenants: EBIT interest coverage **≥ 3.00×**; total debt-to-CFO payback **≤ 4.50 years**. FY2025: sales \$200,000; EBIT \$24,000; interest \$10,000; net income \$9,600; depreciation \$6,400; working-capital drain from AR & inventory build **−\$12,000**.

**Tasks.** Compute (1) EBIT coverage and covenant #1; (2) CFO and Beaver payback and covenant #2; (3) the operational cause and credit consequences.

> [!success]- Solution
> **(1)** EBIT coverage = 24,000 / 10,000 = **2.40×** < 3.00× → **Covenant #1 breached**.
>
> **(2)** CFO = 9,600 + 6,400 − 12,000 = **\$4,000** → payback = 180,000 / 4,000 = **45.0 years** vs. 4.50 allowed → **Covenant #2 severely breached**.
>
> **(3) Cause and consequences.** Vanguard is profitable on paper (NM \$9,600, EBIT \$24,000) — the breach is *operational*: **\$12,000 of working-capital drain** (inventory and receivables) absorbed the cash profit would have produced, collapsing CFO to \$4,000. In **technical default on both covenants**, lenders may accelerate the \$50,000 short-term note, impose penalty pricing, freeze dividends, or force restructuring — consequences that arrive *before* any missed payment. The lesson doubles as the LO 6.1 → 6.2 bridge: a technically defaulting firm can look profitable; what the covenant tests is *cash discipline*, and if the working-capital build was engine-driven or misreported, the reported numbers never showed the tripwire at all.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Current ratio** | Current assets ÷ current liabilities; a snapshot of near-term coverage including inventory |
| **Quick (acid-test) ratio** | (Cash + marketable securities + net receivables) ÷ current liabilities; excludes inventory and prepaids |
| **Cash-flow liquidity ratio** | (Cash + marketable securities + CFO) ÷ current liabilities; adds period-based operational cash |
| **Liquidity paradox** | Traditional ratios fall while cash liquidity improves — typically trade-credit-funded working-capital builds |
| **Equity cushion** | Stockholders' equity as the loss-absorbing layer beneath creditor claims |
| **Debt-to-capital** | Total debt ÷ (total debt + stockholders' equity); permanent financial leverage |
| **EBIT interest coverage** | Operating income ÷ interest expense; earnings-based debt-service measure |
| **Cash interest coverage** | (CFO + interest paid + taxes paid) ÷ interest paid; cash-based debt-service measure |
| **Beaver payback (debt-to-CFO)** | Total debt ÷ CFO; years of operating cash needed to retire all debt |
| **Covenant** | A restrictive credit-agreement condition — e.g., minimum coverage, maximum debt-to-capital |
| **Technical default** | Covenant breach that activates lender rights (acceleration, dividend freeze) without a missed payment |
| **Cycle-to-cycle deterioration** | Successively lower coverage highs and lows across business cycles — structural credit decay |
| **Cash conversion cycle (CCC)** | DSI + DSO − DPO; days an operating dollar is tied up in the cycle |
| **Operating leverage** | Profit sensitivity created by fixed operating costs; downturns amplify EBIT declines |
| **Seasonal working capital** | Inventory buildup preceding peak sales, producing recurring pre-revenue cash dips |

---

> [!danger] Red Flags — Risk Diagnosis
> - Current and quick ratios falling while payables surge — liquidity from suppliers, not performance
> - EBIT coverage strong but CFO negative — accrual profits unable to service cash interest
> - Beaver payback lengthening beyond the debt's maturity schedule — refinancing risk at the worst moment
> - Coverage highs and lows sinking cycle over cycle
> - Any covenant amending or waving during stress — the tripwire already trip
> - DPO stretching year over year — supplier financing disguised as cash strength
> - Operating income moving several times faster than revenue — fixed-cost leverage compounding downturns
> - Profit that depends on policy revenue (credits, subsidies) or on a single season, customer, or weather calendar

---

### Review Questions

> [!question]- Q1: Why can the current and quick ratios fall while the cash-flow liquidity ratio rises sharply?
> Because the first two are point-in-time balance-sheet measures that punish working-capital *builds* (inventory up, payables up), while the third folds in period-specific operational cash generation. If the build was funded by expanded supplier credit and the inventory subsequently sells through, CFO surges and the cash-based ratio doubles even as the snapshot ratios sag.

> [!question]- Q2: What does the equity cushion protect, and from what?
> It protects **creditors** from **asset-value losses**: stockholders' equity is the first-loss layer beneath debt, so higher leverage means a given decline in asset values reaches lenders sooner. At ~40% debt-to-assets, assets can lose ~60% of value before lender claims are impaired ([[M3-Obj-3-1]]).

> [!question]- Q3: Why must EBIT interest coverage be read beside a cash-based coverage measure?
> Interest is paid in cash, not earnings. A firm can show robust EBIT while building inventory and receivables that drive CFO deeply negative — the EBIT ratio says "coverable," the cash ratio says "unserviced." Both are needed, and the gap between them is itself diagnostic.

> [!question]- Q4: What is technical default, and why does it matter before any payment is missed?
> A breach of a covenant (coverage, leverage, payback) triggers lender rights — acceleration, dividend freeze, penalty pricing, operational control — without an actual missed payment. It moves the clock: the refinancing or workout negotiation happens while the firm is *profitable*, which is the only strong negotiating position it will have.

> [!question]- Q5: In the Rock Solid vs. Hollowman recession case, why does the *asset-heavy* firm last longer despite worse EBIT coverage?
> Its \$75M depreciation is a non-cash charge: EBITDA coverage shows both firms at 1.04×, but Rock Solid's cash cushion above fixed interest is larger and more durable, while Hollowman's variable-heavy cost structure lets cash drain as revenue falls. Accrual coverage and cash-service capacity point opposite ways — the exact lesson of the accrual-vs-cash coverage pair.

> [!question]- Q6: Tesla's EBIT interest coverage fell from 57× to 12.9× in two years. Is that a financial red flag or something subtler?
> Neither a breach case nor a non-event: the *level* remains far above covenant ranges and the Beaver payback is ~0.57 years. But coverage ratios that fall five-fold while revenue stays flat reveal the operating-leverage effect — margin compression converts small revenue moves into large income declines. The financial-risk verdict stays "calm"; the *operational* reading is the one that matters, and the direction is the monitor.

---

### Practice Activity

> [!tip] Warm-up path
> New to the material? Do tasks 1–2 with the §IV tables open in front of you; come back to tasks 3–5 after the Module 6 quiz problems.

You are writing the risk profile of Tesla for a credit committee memo, using the figures in §IV and the M5/M2/M3/M4 notes as citations:

1. **Compute the coverage triad** for FY2023–FY2025: EBIT interest coverage, CFO-based payback (Tesla's debt + finance-lease obligations were \$8,376M at FY2025), and cash tower vs. debt. State each trajectory in one number.
2. **Locate the operating leverage.** Using revenue and operating income for FY2024 and FY2025, compute how much faster operating income moved than revenue in each year. Then explain in two sentences why a *price cut* produces this pattern in a fixed-heavy automaker.
3. **Name the CFO dependency.** Reconstruct from [[M2-Obj-2-3]] how much of Tesla's FY2025 CFO came from payables expansion, and state what happens to CFO if DPO normalizes — in numbers if you can.
4. **Classify three Tesla exposures** — regulatory credits (46% of operating income, phased out by law), resale guarantees (\$3.45B, off statement), supplier-financed CFO — each into one of the three layers (financial / operational / strategic), and note for each whether it is **visible** in the primary statements or **masked** (the masked ones lead into [[M6-Obj-6-2]]).
5. **Write the memo sentence**: one sentence for the credit committee that quotes at least two computed figures and states the single biggest *actionable* risk.

---

### Related Notes

- [[M6-Overview]] — Module 6 overview
- [[M6-Obj-6-2]] — Next: how accounting choices and reporting limits mask the risks this note located
- [[M2-Obj-2-1]] — the classified balance sheet; Tesla's debt schedule and lease note
- [[M2-Obj-2-3]] — cash-flow statement; the AP-driven CFO warning reused in §IV
- [[M3-Obj-3-1]] — debt-to-assets and the equity-cushion arithmetic
- [[M4-Obj-4-1]] — DSI/DSO/DPO and the Tesla–BYD conversion-cycle duel
- [[M5-Obj-5-2]] — the cash-flow ladder; CFO/FCF quality behind the payback metric
- [[M5-Obj-5-3]] — regulatory credits and resale guarantees (credits §VI, guarantees §II)

---

> [!info] Sources
> - Tesla, Inc. FY2025 Form 10-K (filed Jan 2026), SEC EDGAR (accession `0001628280-26-003952`) — balance sheet (cash, debt and finance leases, payables), cash-flow statement, interest expense, inventory and guarantee disclosures
> - Worked cases (Sage Inc., Rock Solid Corp. vs. Hollowman, Inc., Vanguard Equipment Corp.) compiled from the course reference: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed) — risk-analysis chapters
> - Cross-referenced Tesla figures validated in [[M2-Obj-2-1]], [[M2-Obj-2-3]], [[M3-Obj-3-1]], [[M4-Obj-4-1]], and [[M5-Obj-5-2]]
