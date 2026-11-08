---
title: "M7-Obj-7-3 - Value the Firm: Intrinsic (DCF) and Relative (Multiples) Valuation"
created: 2026-11-08
date: 2026-11-08
tags:
  - FSA
  - M7
  - Objective-7-3
  - Valuation
aliases:
  - discounted-cash-flow
  - gordon-growth-ddm
  - ev-ebitda-multiple
  - wacc
---

# Learning Objective 7.3

## Value the Firm: Intrinsic (DCF) and Relative (Multiples) Valuation

**By the end of this note, you can:**
- Position a valuation question inside the intrinsic/relative spectrum and state what each family of methods can and cannot answer
- Apply the Gordon-growth dividend discount model, and explain why it returns **zero** for a firm that has never paid a dividend
- Build a free-cash-flow-to-firm (FCFF) discounted cash flow: explicit forecast, WACC discounting, terminal value, and the bridge from enterprise value to a per-share number
- Explain why terminal value dominates a DCF, and read a WACC × terminal-growth sensitivity grid for the fragility it creates
- Apply P/E and EV/EBITDA multiples, and show why EV/EBITDA is the capital-structure-neutral comparison while P/E is not
- Value a real filing on both routes and state honestly what the gap between them means

> [!tip] How to read this note
> The methods first (§I–III), then two worked valuations with solutions collapsed (§IV), then Tesla valued on both routes with every assumption labeled (§V). In §IV and the Review Questions, **attempt each task before expanding a solution** — the answers are collapsed on purpose. The forecast these values rest on is in [[M7-Obj-7-1]]; its stress set is in [[M7-Obj-7-2]].

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc. — and the Gap Between Price and Value
> Module 7 has built a forward-looking statement ([[M7-Obj-7-1]]) and stress-tested it ([[M7-Obj-7-2]]). The last question is the one the analyst was hired to answer: **what are those cash flows worth?** Valuation is where a forecast becomes a decision — an acquisition, a capital raise, a covenant, a sell.
>
> The running company remains **Tesla, Inc.** (FY2025 Form 10-K). Tesla is a *hard* calibration case for valuation, and that is exactly why it is useful: it has **never paid a dividend** (so the dividend discount model returns zero), it holds **\$44,059M** of cash and investments against **\$8,376M** of debt (so the capital structure is inverted), and it trades at **157× EV/EBITDA** (so market multiples are far from any anchor). The danger shapes come from the course reference (Fridson & Alvarez): **Aegis Technologies** (a clean two-stage DCF) and the **Solon Corp. vs. Vesta Inc.** pair (two identical businesses valued by two different multiples). The LBO arithmetic is kept as a brief illustration only.

| Family | Method | What it answers | Dominant weakness |
|---|---|---|---|
| **Intrinsic** | DDM · FCFF DCF | "What are these cash flows worth to today's capital?" | The discount rate and terminal assumptions carry most of the answer |
| **Relative** | P/E · EV/EBITDA | "What does the market pay for comparable cash flows?" | The multiple is an *output* of expectations, not an independent anchor |
| **Asset-based** | Liquidation value · LBO debt capacity | "What can the assets support?" | Ignores the operating business unless the business is the asset |

> [!tip] Where this fits in Module 7
> 7.1 built the forecast ([[M7-Obj-7-1]]), 7.2 found how fragile it is ([[M7-Obj-7-2]]), and 7.3 prices it. Note the dependency chain: a valuation is only as good as the forecast underneath it, and a forecast that was never stressed ([[M7-Obj-7-2]]) will produce a precise-looking number with no error bars.

---

### I. Purpose & Architecture of Valuation

#### 1. What valuation is (and is not)

Valuation is the estimation of the **intrinsic value** of a business — the present value of the cash flows it can be expected to generate for its providers of capital. It is not:

- a prediction of the market price (the market price is a *different* estimate, made by different people, with different information and different opinions);
- a single number (every valuation is a range conditioned on assumptions);
- a substitute for judgment (a DCF run on a bad forecast produces a precise, worthless answer).

> [!danger] The three questions any valuation must answer
> 1. **What cash flows, and to whom?** Free cash flow to the *firm* (available to all capital) values the enterprise; free cash flow to *equity* values the shareholders' claim directly. Mixing them is the single most common valuation error.
> 2. **What discount rate?** A valuation is a statement about risk as much as about cash flows — the same forecast at a different discount rate is a different valuation.
> 3. **What happens after the explicit forecast?** For most companies, the terminal value is the majority of the answer (§II, Step 4).

#### 2. The valuation methodology triad

<div style="display:flex;flex-direction:column;align-items:center;gap:0.5rem;margin:1rem 0">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.4rem;font-weight:600">THE VALUATION TRIAD</div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;align-items:stretch;gap:0.75rem;width:100%">
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Discounted cash flow</b><br/><span style="font-size:0.85em">DDM · FCFF with WACC · terminal value</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Relative multiples</b><br/><span style="font-size:0.85em">P/E · EV/EBITDA · capital-structure neutrality</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Asset and restructuring</b><br/><span style="font-size:0.85em">Liquidation value · LBO debt capacity</span></div>
  </div>
</div>

---

### II. Intrinsic Valuation: Discounted Cash Flow

#### Step 1 — The dividend discount model (and where it fails)

**The idea.** For a mature firm that pays out a stable share of earnings as dividends, equity value equals the present value of all future dividends:

$$\text{Equity Value} = \sum_{t=1}^{\infty} \frac{D_t}{(1 + K)^t}$$

**The Gordon constant-growth form.** If dividends grow at a constant rate $g$ forever and the required return is $K$:

$$P_0 = \frac{D_1}{K - g} = \frac{D_0(1 + g)}{K - g}$$

where $P_0$ = intrinsic share price, $D_1$ = next year's expected dividend, $K$ = cost of equity (required return), $g$ = sustainable dividend growth rate.

The model has one wonderful property and one fatal limitation. The property: it forces you to state a required return and a growth rate, and it punishes their incompatibility — if $g \geq K$, the denominator goes to zero and the "valuation" explodes to infinity. The limitation: it only works for firms that **pay dividends**, and it requires that the payout be permanent.

> [!danger] The zero that is not a valuation
> Apply the DDM to **Tesla**: the 10-K states plainly that the company *"has never declared or paid cash dividends"* and does not anticipate doing so. With $D_0 = 0$ the Gordon model returns **\$0 per share**. The DDM is not wrong about Tesla — it is answering a different question. A firm that reinvests everything and pays nothing has no dividend stream to discount, so **no dividend-based valuation exists**; the cash must be valued where it actually accrues: to the firm, as free cash flow. This is not a quirk of Tesla. It is why a 30-year-old company with enormous value can be un-valueable by the most famous valuation formula in finance, and why the next model exists.

#### Step 2 — Free cash flow to the firm (FCFF)

FCFF measures the cash generated by core operations that is **available to all providers of capital** (debt and equity) after funding operating costs, working-capital investment, and maintenance capital expenditure:

$$\text{FCFF} = \text{EBIT}(1 - t) + \text{Depreciation \& Amortization} - \text{CapEx} - \Delta\text{Working Capital}$$

Three design choices, each doing specific work:

1. **EBIT, not net income.** Net income is after interest — so it depends on the capital structure. FCFF is computed *before* financing, which makes it comparable across firms with different debt (the same neutrality that makes EV/EBITDA work, §III).
2. **Add back D&A, then subtract CapEx.** The add-back reverses a non-cash charge; the subtraction pays for the assets that consume the cash. A company whose CapEx runs far above D&A is investing — its FCFF is smaller than its earnings, and any valuation that ignores CapEx overstates value.
3. **Subtract the change in working capital.** Growth consumes cash before it produces it ([[M7-Obj-7-1]] §II, Step 3). A forecast that grows revenue without funding the receivables and inventory behind it produces FCFF that is not there.

#### Step 3 — Discounting: the WACC

$$\text{Total Enterprise Value} = \sum_{t=1}^{N} \frac{\text{FCFF}_t}{(1 + \text{WACC})^t} + \frac{\text{Terminal Value}_N}{(1 + \text{WACC})^N}$$

The **weighted average cost of capital** is the blended cost of the firm's financing:

$$\text{WACC} = w_E \cdot K_E + w_D \cdot K_D \cdot (1 - t)$$

with equity weight $w_E$ at **market value** (not book value), debt weight $w_D$, cost of equity $K_E$ built from a risk-free rate plus a risk premium for the business, and after-tax cost of debt $K_D$.

> [!danger] No financial statement contains a discount rate
> The 10-K gives you cash flows, not a required return. Every WACC in this note — and in every DCF you will ever build — is an **assumption set by the analyst**, and it must be disclosed, defended, and stressed. Two analysts can produce valuations of the same company that differ by 40% on the discount rate alone (§IV shows the range). A valuation presented without a discount-rate sensitivity is a single opinion dressed as a calculation.

#### Step 4 — Terminal value, and why it dominates

For a firm expected to grow at a constant rate $g_n$ beyond year $N$:

$$\text{Terminal Value}_N = \frac{\text{FCFF}_{N+1}}{\text{WACC} - g_n} = \frac{\text{FCFF}_N \times (1 + g_n)}{\text{WACC} - g_n}$$

Three things to hold onto:

1. **The denominator is a small difference of large numbers.** With WACC at 9% and terminal growth at 3%, the denominator is 6 cents; shift either input and the terminal value moves violently (the grid in §V).
2. **Terminal growth cannot approach the discount rate.** If $g_n \geq$ WACC, the perpetuity is undefined and the model is nonsense — a mathematical statement of the fact that growth cannot be perpetual at a rate exceeding the cost of capital.
3. **Terminal value is usually most of the answer.** In the Aegis case below, the terminal value is **79.9%** of enterprise value; in the Tesla illustration, **84.8%**. That is normal — it is also why DCFs must be read as *conditional statements about the terminal period*.

#### Step 5 — From enterprise value to a per-share number

$$\text{Equity Value} = \text{Total Enterprise Value} + \text{Cash and Investments} - \text{Total Debt}$$

$$\text{Intrinsic Share Price} = \frac{\text{Equity Value}}{\text{Shares Outstanding}}$$

Two mechanical points that are routinely botched:

- **The bridge is a balance-sheet fact, not a plug.** Adding cash and subtracting debt converts the *enterprise* claim into the *equity* claim. For Tesla, cash and investments of \$44,059M less debt of \$8,376M is a **net cash position of \$35,683M** — a large *addition* to equity value, because Tesla's balance sheet is not a burden on the equity holder but a claim the equity holder owns.
- **State the share basis.** Tesla had **3,751M shares issued and outstanding** at December 31, 2025 but only **3,528M diluted weighted-average shares** in the FY2025 EPS computation. The two differ because unvested restricted stock awards are issued but not yet in the diluted denominator. Using the wrong one moves a per-share number by roughly 6%.

---

### III. Relative Valuation: Market Multiples

#### A. Price-to-earnings (P/E)

$$\text{P/E} = \frac{\text{Market Price per Share}}{\text{Earnings per Share}}$$

Substituting the Gordon growth model into the P/E definition produces the identity that makes the multiple interpretable:

$$\text{P/E} = \frac{\text{Dividend Payout Ratio}}{K - g}$$

The multiple is therefore a *statement about three variables*: the payout policy, the expected growth rate, and the required return. A high P/E means the market expects superior growth $g$ or perceives low risk $K$; a low P/E signals cyclical vulnerability, poor earnings quality, or management instability — the three conditions Module 5 and Module 6 taught you to look for.

**Earnings normalization comes first.** Applying a peer multiple to an unnormalized EPS imports the peer's assumptions about growth and risk into a number that does not deserve them. Module 5's core stack and Module 6's distortion tests are the preparation for this step: strip windfalls and "big bath" charges, then multiply. If you skip it, the multiple does the wrong work.

#### B. Enterprise value to EBITDA (EV/EBITDA)

$$\text{Total Enterprise Value} = \text{Equity Market Cap} + \text{Total Debt} + \text{Preferred Stock} - \text{Cash and Investments}$$

$$\text{EV/EBITDA} = \frac{\text{Total Enterprise Value}}{\text{EBITDA}}$$

**The comparability advantage.** Using P/E to compare two firms with different capital structures or different depreciation policies manufactures false valuation gaps: the more leveraged, more heavily depreciating firm looks *cheaper* on earnings while owning a *different* set of operating assets. Valuing the enterprise as a multiple of **EBITDA** — the operating cash proxy before depreciation, interest, and tax — neutralizes both differences and lets the comparison run at the operating-asset level. The equity claim is then recovered by subtracting each firm's own net debt, which is exactly where the two firms should differ.

#### C. LBO and restructuring value (brief illustration)

The third branch of the triad asks a different question: **how much debt can this business service?** A sponsor sizes the debt from the target's EBITDA against a minimum coverage constraint (the course reference's case uses a **1.5× EBITDA coverage floor** and a **13% borrowing rate**), adds a sponsor equity contribution (the reference case uses **10%**), and works back to a maximum offer per share.

We keep this as an illustration only — it is a *debt-capacity* framework, not a valuation framework, and it applies to a business being taken over rather than one being analyzed. Two cautions: the same coverage arithmetic is what a lender uses to test *your* covenant headroom ([[M6-Obj-6-1]] §I.3), and a leveraged bid converts operating risk into a fixed obligation, which is precisely the risk Module 6 spent a module mapping.

---

### IV. Worked Calculations

> [!tip] Before you flip any answer
> Attempt each case before opening the solution. Both are self-contained: all inputs are given.

#### Case A — Aegis Technologies: a two-stage FCFF/WACC valuation

**Scenario.** You are an equity research analyst valuing **Aegis Technologies**. You build a 4-year pro forma projection of free cash flow to the firm (\$M): Year 1 \$20.0M, Year 2 \$24.0M, Year 3 \$28.0M, Year 4 \$32.0M.

**Parameters.** WACC = **10.0%**; beyond year 4, FCFF grows at a constant **3.0%**; cash = **\$15.0M**; total debt = **\$65.0M**; diluted shares outstanding = **10.0M**.

**Tasks.** (1) Calculate the present value of explicit FCFF for years 1–4. (2) Calculate the terminal value at year 4 and its present value. (3) Calculate total enterprise value and equity value. (4) Calculate the intrinsic share price.

> [!success]- Solution
> **(1) PV of explicit cash flows at 10%**
> - Year 1: 20.0 / 1.10 = **18.18**
> - Year 2: 24.0 / 1.21 = **19.83**
> - Year 3: 28.0 / 1.331 = **21.04**
> - Year 4: 32.0 / 1.4641 = **21.86**
> - **Sum of explicit PV = 80.91**
>
> **(2) Terminal value**
> - Year-5 FCFF = 32.0 × 1.03 = **32.96**
> - TV₄ = 32.96 / (0.10 − 0.03) = **470.86**
> - PV of TV = 470.86 / 1.4641 = **321.60**
>
> **(3) Enterprise and equity value**
> - TEV = 80.91 + 321.60 = **402.51**
> - Equity = TEV + cash − debt = 402.51 + 15.0 − 65.0 = **352.51**
>
> **(4) Intrinsic share price** = 352.51 / 10.0 = **\$35.25 per share**
>
> **Note the concentration:** the terminal value is **79.9%** of enterprise value. Four years of explicitly forecast cash flow produced \$80.91M; the perpetuity after them produced \$321.60M. The model is mostly an opinion about the terminal period.

#### Case B — Solon Corp. vs. Vesta Inc.: capital-structure neutrality

**Scenario.** You are an M&A analyst evaluating two target firms in the precision-tools sector. Both generate identical net revenues of **\$200.0M** and identical operating expenses before depreciation. A peer acquisition just closed at **8.0× EV/EBITDA**.

- **Solon Corp:** debt-free. Accelerated depreciation: D&A = **\$20.0M**, EBIT = **\$30.0M**.
- **Vesta Inc:** **\$50.0M** of debt (annual interest \$4.0M). Slow straight-line depreciation: D&A = **\$10.0M**, EBIT = **\$40.0M**.

**Tasks.** (1) Calculate EBITDA for both firms. (2) Calculate TEV for both at 8.0× EBITDA. (3) Calculate equity value for both. (4) In two sentences, explain why a P/E or net-income multiple would misprice these firms while EV/EBITDA does not.

> [!success]- Solution
> **(1) EBITDA**
> - Solon: 30.0 + 20.0 = **\$50.0M**
> - Vesta: 40.0 + 10.0 = **\$50.0M**
>
> **(2) Enterprise value at 8.0×** — Solon: 50.0 × 8.0 = **\$400.0M**; Vesta: 50.0 × 8.0 = **\$400.0M**
>
> **(3) Equity value** — Solon: 400.0 − 0 = **\$400.0M**; Vesta: 400.0 − 50.0 = **\$350.0M**
>
> **(4) Why the methods differ**
> *The distortion of net income:* Vesta reports **higher** EBIT (\$40M vs. \$30M) purely because it depreciates more slowly (\$10M vs. \$20M). Its net income is flattered by an accounting policy, not by better operations. A P/E or net-income multiple would therefore hand Vesta the *higher* value while the two firms own the same operating assets.
> *The EBITDA advantage:* adding back non-cash depreciation and valuing the firm before interest assigns both businesses the same **\$400.0M enterprise value** — the correct statement, since they generate identical operating cash flow. The capital structure then does its job: it takes \$50.0M off Vesta's equity claim and leaves Solon's intact.

---

### V. Applying Valuation to Tesla

Two routes to the same question: what is Tesla worth?

#### Route 1 — Relative: what the market is paying (all figures from the FY2025 10-K and the Dec 31, 2025 close)

| Measure | Calculation | Result |
|---|---|---:|
| Equity market capitalisation | 3,751M shares × \$449.72 | **\$1,686,900M** |
| Total enterprise value | 1,686,900 + debt 8,376 − cash and investments 44,059 | **\$1,651,217M** |
| EBITDA (FY2025) | EBIT 4,355 + D&A 6,148 | **\$10,503M** |
| EV/EBITDA | 1,651,217 ÷ 10,503 | **157.2×** |
| P/E on reported diluted EPS | \$449.72 ÷ \$1.08 | **416.4×** |
| Core EPS (credits stripped at the 27.0% tax rate) | (3,855 − 1,993 × 0.73) ÷ 3,528 = \$2,399M ÷ 3,528 | **\$0.68** |
| **P/E on core EPS** | \$449.72 ÷ \$0.68 | **661.3×** |
| DDM (Gordon growth) | no dividend has ever been paid → \$0 ÷ (\$K − \$g) | **\$0.00 — inapplicable** |

Three readings, in order of usefulness:

1. **The DDM says zero, and the DDM is answering the wrong question.** No dividend has ever been paid, so the dividend stream is empty. Value has to be captured in the firm's cash flow instead.
2. **The multiples are outputs, not anchors.** At 157× EV/EBITDA and 416× reported P/E, the "comparable multiple" has no comparable to anchor to — a 1% change in the multiple moves enterprise value by \$16.5B. Applying a peer multiple here would import someone else's expectations and present them as an analysis.
3. **Normalization makes it worse, which is the honest direction.** Stripping the policy-dependent regulatory credits (1,993 of revenue) lowers core EPS from \$1.08 to \$0.68 and lifts the P/E from 416× to **661×**. The Module 5–6 discipline — do not capitalize windfalls — makes the multiple *more* extreme, because the windfall was flattering the denominator.

#### Route 2 — Intrinsic: an illustrative FCFF DCF

The forecast starts from the FY2026 base case of [[M7-Obj-7-1]] §IV and extends it with instructor-set assumptions (revenue growth 15% / 12% / 10% / 8%; EBIT margin 5.5% → 9.5%; D&A 6.0% of sales; CapEx 6.5% of sales; working capital 3.0% of the revenue increase; tax 27%; **WACC 9.0%**; terminal growth **3.0%**):

| Year | Revenue | EBIT | D&A | CapEx | ΔWC | FCFF | PV at 9% |
|---|---:|---:|---:|---:|---:|---:|---:|
| FY2026 | 104,310 | 4,716 | 7,000 | 10,000 | 359 | **83** | 76 |
| FY2027 | 119,956 | 6,598 | 7,197 | 7,797 | 469 | **3,747** | 3,154 |
| FY2028 | 134,351 | 9,405 | 8,061 | 8,733 | 432 | **5,762** | 4,449 |
| FY2029 | 147,786 | 12,562 | 8,867 | 9,606 | 403 | **8,028** | 5,687 |
| FY2030 | 159,609 | 15,163 | 9,577 | 10,375 | 355 | **9,916** | 6,445 |
| **Sum of explicit PV** | | | | | | | **20,391** |
| Terminal value (g = 3.0%) | | | | | | 170,227 | |
| **PV of terminal value** | | | | | | **110,636** | |
| **Total enterprise value** | | | | | | **130,447** | |
| Equity value (EV + 44,059 cash − 8,376 debt) | | | | | | **166,130** | |
| **Intrinsic value per share** (3,751M shares) | | | | | | **\$44.29** | |

**Read the result carefully — it is not a price target.** Our illustrative EV of \$130,447M is **12.7×** below the market's \$1,651,217M, and our per-share \$44.29 is far below the \$449.72 close. The correct conclusion is *not* "the stock is cheap" or "the stock is expensive." It is:

1. **The market's price embeds assumptions we did not make.** A price of \$449.72 is a statement about the terminal period — and about the terminal period of a business whose near-term free cash flow is currently tiny (\$83M of FCFF on \$1.69 trillion of market cap).
2. **Terminal value carries the whole model.** Here it is **84.8%** of enterprise value — even more concentrated than the Aegis case (79.9%).
3. **The discount rate alone can double the answer.** Holding the operating forecast fixed and varying only WACC and terminal growth:

| Enterprise value (\$M) | g = 2.0% | g = 3.0% | g = 4.0% |
|---|---:|---:|---:|
| **WACC 8.0%** | 135,242 | 159,537 | 195,981 |
| **WACC 9.0%** | 113,721 | **130,447** | 153,863 |
| **WACC 10.0%** | 97,645 | 109,739 | 125,865 |

The range across discount-rate and terminal-growth choices alone is **97,645 to 195,981** — a **2.0×** spread with no change to the operating forecast. Any valuation that quotes one number from this grid without the grid has misrepresented its own uncertainty.

> [!danger] What this illustration is, and what it is not
> **It is**: a demonstration of the mechanics — FCFF construction, discounting, terminal value, the enterprise-to-equity bridge, the per-share arithmetic — on real filing data, with every assumption labeled as instructor-set.
> **It is not**: a valuation opinion on TSLA, a price target, or investment advice. The operating assumptions (growth, margin path, capital intensity) were invented for teaching; a serious valuation would require a multi-year operating model built from segment detail, a defended discount rate, and scenario weights — the machinery of [[M7-Obj-7-1]] and [[M7-Obj-7-2]] applied at full scale.
> **The intellectually honest exercise is the reverse one**: the *reverse DCF*. Rather than asking "what is Tesla worth?", ask "**what must be true** for the market's \$1,651,217M enterprise value to be right?" — what revenue path, margin path, and terminal assumptions justify it? A valuation is not an answer; it is a set of assumptions with a price attached, and the reverse DCF is how you compare that set to your own.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Intrinsic value** | Present value of the cash flows the business can be expected to generate for its capital providers |
| **DDM (Gordon growth)** | \(P_0 = D_1/(K-g)\); applicable only where dividends are paid and sustainable |
| **FCFF** | EBIT(1 − t) + D&A − CapEx − ΔWC; cash available to all capital providers |
| **FCFE** | Cash available to equity after debt service; values the equity claim directly |
| **WACC** | Weighted average cost of capital; equity at market-value weights plus after-tax debt cost |
| **Terminal value** | Perpetuity value of cash flows beyond the explicit forecast; usually the majority of a DCF |
| **Enterprise value (TEV)** | Equity market cap + debt + preferred − cash and investments |
| **Equity value** | TEV + cash and investments − total debt |
| **EV/EBITDA** | Enterprise value ÷ EBITDA; capital-structure- and depreciation-neutral comparison multiple |
| **P/E = payout / (K − g)** | The identity that makes the P/E interpretable as a statement about payout, growth, and required return |
| **Normalized earnings** | Earnings stripped of windfalls and one-off charges before a multiple is applied |
| **Reverse DCF** | Solving for the assumptions implied by a market price, instead of valuing against your own |
| **Valuation range** | The span produced by defensible assumption choices; the honest unit of a valuation output |

---

> [!danger] Red Flags — Valuation Discipline
> - A point estimate with no sensitivity table attached
> - A terminal growth rate approaching or exceeding the discount rate
> - Net income used as a proxy for cash flow (interest and CapEx both distort it)
> - D&A added back without CapEx subtracted — the most common FCFF error
> - A multiple applied to unnormalized earnings, importing windfalls into a permanent base
> - P/E used to compare firms with different leverage or depreciation policies
>- An equity value computed without the cash-and-debt bridge, or with book equity in the denominator
> - Shares outstanding confused with diluted weighted-average shares
> - A WACC with no stated components, or a discount rate asserted rather than defended
> - A per-share number presented as a target rather than as one point in a range

---

### Review Questions

> [!question]- Q1: Why does the DDM return \$0 for Tesla, and why is that not a valuation failure?
> Because Tesla has never declared or paid a cash dividend, so the dividend stream the model discounts is empty: \$0 ÷ (\$K − \$g) = \$0. The formula is answering a question — "what are the dividends worth?" — that does not apply to a firm that reinvests everything. Value must be captured in the firm's cash flow instead, which is why FCFF-based methods exist for non-dividend payers.

> [!question]- Q2: Why does FCFF start from EBIT rather than net income, and why does that matter when comparing two firms?
> Net income is after interest, so it depends on how the firm is financed; FCFF is computed before financing and therefore measures the operating cash available to all capital providers. Two firms with identical operations but different debt produce identical FCFF and identical enterprise value — and the difference in equity value comes from the debt, correctly. Using net income instead would entangle operating performance with capital structure.

> [!question]- Q3: In the Aegis case, the terminal value is 79.9% of enterprise value. What does that tell you about how to read a DCF?
> That most of the "value" is an assumption about the perpetual period rather than a calculation on the explicit forecast. It does not make the DCF wrong, but it changes how it must be read: the answer is essentially "what will this business look like in year N and forever after, discounted at a rate I chose." Hence terminal-value and discount-rate sensitivities are mandatory, and the enterprise value must never be quoted without them.

> [!question]- Q4: Why does EV/EBITDA assign the same enterprise value to Solon and Vesta, and what does that imply for the equity holders?
> Both generate identical operating cash flow (\$50.0M of EBITDA) because Vesta's higher EBIT is purely an artifact of slower depreciation. Valuing the operating asset base the same way assigns each firm the same \$400.0M enterprise value; the capital structure then correctly removes \$50.0M from Vesta's equity claim. The lesson is that accounting policy changes the earnings line, and a neutral multiple refuses to price it.

> [!question]- Q5: Tesla's EV/EBITDA is 157× and its P/E on core EPS is 661×. What do you do with a peer multiple in this situation?
> You cannot use it as an anchor: there is no peer set trading at those multiples, and a 1% change in the multiple moves enterprise value by \$16.5B. The multiple is an *output* of market expectations, so the analytical move is the reverse one — solve for what the price implies (reverse DCF) rather than importing someone else's expectations as if they were comparable analysis.

> [!question]- Q6: Our illustrative Tesla DCF produces \$44.29 per share against a \$449.72 market price. State three conclusions this comparison supports, and one it does not.
> Supports: (i) the market price embeds operating assumptions far beyond the ones we made; (ii) terminal value carries the model (84.8% of EV), so the valuation is mostly a terminal-period statement; (iii) discount-rate and terminal-growth choices alone span a 2.0× range of enterprise value (97,645–195,981). Does not support: any claim that the stock is mispriced by a factor of ten — our assumptions were invented for teaching, and a real valuation requires a defensible operating model, not a single illustrative path.

---

### Practice Activity

> [!tip] Warm-up path
> New to the material? Do tasks 1–3 with §II's formulas in front of you; tasks 4–5 belong after the Module 7 quiz.

You are the analyst valuing Tesla for an internal capital-allocation review, using the FY2025 10-K and the FY2026 base case from [[M7-Obj-7-1]]:

1. **Build the FCFF bridge.** From the FY2026 base case, compute FY2026 FCFF (EBIT × (1 − t) + D&A − CapEx − ΔWC) and state which term does the most damage to free cash flow — and why. (Compare with FY2025 actual CFO of \$14,747M and CapEx of \$8,527M.)
2. **Value it on multiples.** Recompute market capitalisation, enterprise value, EV/EBITDA, and P/E on both reported and core EPS. Then compute the implied enterprise value if the market applied the *Aegis* peer context of an 8.0× EV/EBITDA multiple, and state in two sentences what that comparison tells you about borrowing multiples from a different industry.
3. **Do the bridge correctly.** Compute enterprise value from the §V illustrative DCF, then add cash and investments and subtract debt, and divide by **both** share counts (3,751M outstanding and 3,528M diluted weighted average). State which basis you would use for a takeover offer and why the difference matters.
4. **Test the terminal assumption.** Recompute the §V terminal value at WACC 8.0% and terminal growth 4.0%, then compute the resulting enterprise value from the grid. State in one sentence what the exercise proves about the model's usefulness.
5. **Run the reverse DCF (the real assignment).** State what the market's \$1,651,217M enterprise value requires: begin from your FY2030 FCFF, and solve for the terminal growth rate (at WACC 9.0%) that makes the DCF equal the market's enterprise value. Report the number, then state in two sentences whether that required assumption is *plausible*, and what would have to be true in the operating forecast for it to hold.

---

### Related Notes

- [[M7-Overview]] — Module 7 overview
- [[M7-Obj-7-1]] — the forecast that produces the cash flows valued here; the pro-forma mirage warning in [[M6-Obj-6-2]] applies to any "adjusted" earnings used as a valuation base
- [[M7-Obj-7-2]] — the stress set; a valuation built on an unstressed forecast inherits its optimism
- [[M5-Obj-5-3]] — the core-earnings stack; normalization is a precondition for applying any multiple
- [[M5-Obj-5-2]] — cash-flow quality: the difference between earnings and the cash a DCF discounts
- [[M6-Obj-6-1]] — the equity cushion and covenant tripwires; LBO debt capacity is the lender's arithmetic run in reverse
- [[M6-Obj-6-2]] — Altman Z and the "almost meaningless as a ranking tool" lesson; the same honesty applies to a 157× multiple
- [[M3-Obj-3-1]] — margin and return ratios; EBITDA and margin math used throughout §III

---

> [!info] Sources
> - Tesla, Inc. FY2025 Form 10-K (filed Jan 2026), SEC EDGAR (accession `0001628280-26-003952`) — income statement, balance sheet, cash-flow statement; dividend policy; share counts (3,751M issued and outstanding; 3,528M diluted weighted average)
> - Market data: TSLA close \$449.72 (Dec 31, 2025), Yahoo Finance / StatMuse (verified source — see instructor key)
> - Aegis Technologies and Solon/Vesta worked cases compiled from the course reference: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed), Part IV (Ch. 12 & 14, "Forecasts and Security Analysis"); the LBO illustration (1.5× coverage floor, 13% borrowing rate, 10% sponsor equity) is from the same source and is presented without case data
> - All WACC, terminal-growth, and operating assumptions in §V are instructor-set for teaching; the §V illustration is not a valuation opinion or price target
> - Cross-referenced Tesla figures validated in [[M5-Obj-5-2]], [[M5-Obj-5-3]], and [[M6-Obj-6-1]]
