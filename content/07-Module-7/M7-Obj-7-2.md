---
title: M7-Obj-7-2 - Stress-Test the Forecast: Sensitivity Analysis and Interdependent Risk
created: 2026-11-08
date: 2026-11-08
tags:
  - FSA
  - M7
  - Objective-7-2
  - Sensitivity-Analysis
aliases:
  - scenario-analysis
  - break-even-analysis
  - forecast-stress-testing
---

# Learning Objective 7.2

## Stress-Test the Forecast: Sensitivity Analysis and Interdependent Risk

**By the end of this note, you can:**
- Distinguish three levels of forecast stress — single-variable isolation, scenario analysis, and break-even (switch-point) analysis — and know what each one answers
- Explain why "all else equal" is never true: the four interdependencies that link volume, margin, working capital, and financing in a pro forma model
- Re-run a full forecast under a downside case and interpret the movement in the financing plug — including why the plug can *improve* while earnings collapse
- Build a two-variable sensitivity grid, read its gradients, and extract the break-even point that converts a plan from self-funding to dependent on external money
- Apply the discipline to Tesla's FY2026 plan and state which assumption actually drives the financing outcome

> [!tip] How to read this note
> The mechanics first (§I–II), then a worked downturn with the solution collapsed (§III), then Tesla's stress set and grid (§IV). In §III and the Review Questions, **attempt each task before expanding a solution** — the answers are collapsed on purpose. The valuation half of Module 7 is in [[M7-Obj-7-3]].

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc. — and What the Forecast Is Actually Sensitive To
> [[M7-Obj-7-1]] built Tesla's FY2026 plan and found a **\$1,063M surplus**: the plan is self-funding. That result is conditional, and this objective exists to price the condition. A forecast without stress is a promise; a forecast with stress is an argument — and for Tesla the stress test produces a genuinely surprising answer that a banker would want on page one.
>
> The running company remains **Tesla, Inc.** (FY2025 Form 10-K base, §IV of [[M7-Obj-7-1]]). The danger shapes come from the course reference (Fridson & Alvarez): the **Titan Dynamics** downturn (margin compression with slowing growth) and **Colossal Chemical** (a forecast that breaks when the operating assumption fails). Both cases are clean teaching models: no unusual items, no leases — so every movement you compute must come from the method.

| Stress level | The question it answers | Output | Typical reader |
|---|---|---|---|
| **Single-variable isolation** | "If *this one* assumption is wrong, how wrong is the answer?" | One-variable sensitivity table | Model owner, sanity check |
| **Scenario analysis** | "If the world moves to *this* state, what does the plan do?" | Full re-run under a coherent set of assumptions | Credit committee, board |
| **Break-even (switch-point) analysis** | "How far can this assumption move before the answer *changes character*?" | The threshold value — growth needed, margin needed, price needed | Lender, covenant negotiation |

> [!tip] Where this fits in Module 7
> 7.1 built the forecast and found the financing gap ([[M7-Obj-7-1]]); 7.2 finds out how fragile that gap is; 7.3 asks what the projected cash flows are worth ([[M7-Obj-7-3]]). The three objectives answer the three questions a capital provider asks: *can you build it? can it break? is it worth building?*

---

### I. Purpose & Architecture of Sensitivity Analysis

#### 1. What stress testing is for

A forecast is a **single point on a surface**. Sensitivity analysis maps the surface around that point so the reader can see:

- **which assumptions the answer actually depends on** (and which are decorative);
- **how much error the answer tolerates** before it changes character;
- **whether the worst case is survivable** — by whom, and with what covenants.

The output is not a prediction of the future. It is a **map of the future's conditional shape**.

#### 2. The three levels, and when each is used

**Level 1 — Single-variable isolation.** Change one assumption, hold everything else, record the effect. The classic output is a small table (or tornado chart) ranking assumptions by impact:

| Assumption moved | Effect on FY2026 EBIT | Effect on EFN |
|---|---:|---:|
| Revenue growth ±5 points | ... | ... |
| Cost-of-revenues ratio ±1 point | ... | ... |
| CapEx ±\$1,000M | ... | ... |

Use it as a *sanity check* on which assumptions deserve the model's attention — and beware its central flaw, discussed in §II.

**Level 2 — Scenario analysis.** Re-run the entire model under a **coherent set** of assumptions that describes a plausible world: a recession, a price war, a capacity ramp, a regulatory change. This is what a credit committee reads, because the world does not move one variable at a time.

**Level 3 — Break-even (switch-point) analysis.** Solve for the assumption value at which the output *flips*: the growth rate at which the plan stops being self-funding; the cost ratio at which the plug turns positive; the price at which a project breaks even. This converts a table of numbers into a **decision boundary** — the single most useful form of forecast analysis, because a lender can negotiate against a number ("we are comfortable down to 4.8% growth").

> [!danger] Scenarios are not probabilities
> A stress case says "*if* the world looks like this, the plan does that." It does not say how likely that world is. The moment a scenario set is presented with likelihood weights, the analysis stops being transparent: the reader cannot separate the mechanical result from the analyst's guess about the world. Keep the worlds explicit, keep the mechanics exact, and label judgment separately from arithmetic.

---

### II. Why Single-Variable Isolation Misleads

"Isolating a single variable assumes *all other things remain equal*." In a pro forma model that assumption fails in at least four places, and the failures run in the same direction — **they make reality worse than the isolated stress suggests**.

#### 1. Volume down → margin down (operating leverage)

Fixed overhead does not shrink when volume shrinks ([[M6-Obj-6-1]] §II.2). A sales decline therefore produces a *larger-than-proportional* EBIT decline. Isolating "revenue −10%" while holding the cost ratio flat **overstates** EBIT.

#### 2. Revenue down → working capital released (the cushion)

Working capital scales with sales: receivables and inventory fall, and payables fall with them, but not proportionally — days metrics are sticky in the short run, so payables usually fall *slower* than revenue. Net effect: a contraction **releases cash**. That cash release partially offsets the earnings loss, which is why a *financing* test can look better in a downturn than in a growth year (§III).

#### 3. Rates up → interest up → retained earnings down → plug up

Interest expense is a rate times debt ([[M7-Obj-7-1]] §II, Step 2). Higher rates raise interest, lower net income, lower the retained-earnings roll-forward, and therefore raise the plug — while the borrowing needed to close the plug makes the interest assumption self-referential.

#### 4. The plug is not the earnings

The EFN measures **balance-sheet closure**, not performance. In a slowing business, working-capital release and unchanged capital spending can leave the plug intact or improved while EBIT has fallen by a third (§III). A model watched only through its financing plug can therefore announce "fine" during an earnings collapse.

> [!tip] How to run a defensible stress set
> 1. **State the world, not the variable.** "A recession in which volume growth halves and factories under-absorb fixed overhead" — not "revenue −10%".
> 2. **Move related assumptions together**, in the direction they would actually move.
> 3. **Report the earnings path and the financing path side by side.** If one improves while the other collapses, you have found the most important fact in the model.
> 4. **Then find the switch point** — the assumption value at which the plan changes character.

---

### III. Worked Calculation: The Titan Downturn

> [!tip] Before you flip any answer
> Attempt all three tasks before opening the solution. You are continuing from the FY2025 base forecast in [[M7-Obj-7-1]] §III; the only new information is the scenario below.

#### Scenario

Following the FY2025 base case, a recession hits Titan Dynamics:

1. Sales growth slows to **3.0%** (projected sales \$103,000 thousand; projected COGS \$61,800 thousand).
2. Increased competition compresses gross margin, driving SG&A up to **23.0% of sales** (\$23,690 thousand).
3. Depreciation (\$6,000), CapEx (\$10,000), interest (\$2,000), tax rate (30%), dividend payout (30%), cash target (\$5,000), and the baseline working-capital days all remain unchanged.

**Tasks.** (1) Calculate the stressed net income and the addition to retained earnings. (2) Calculate the stressed projected total assets and projected total liabilities and equity. (3) Calculate the new EFN, and explain in two sentences why the financing position looks *better* than the base case even though earnings fell by more than a third.

> [!success]- Solution
> **(1) Stressed income statement**
> - Sales = **103,000**; COGS (60%) = **61,800**; SG&A (23%) = **23,690**; depreciation = **6,000**
> - EBIT = 103,000 − 61,800 − 23,690 − 6,000 = **11,510** (margin **11.17%** vs. 14.78% in the base case)
> - Interest = 2,000 → pre-tax = **9,510**; tax at 30% = **2,853** → **Net income = 6,657**
> - Dividends (30%) = 1,997 → **addition to retained earnings = 4,660**
>
> **(2) Stressed balance sheet**
> - AR = 15,000 × 1.03 = **15,450**; inventory = 12,000 × 1.03 = **12,360**; cash = **5,000**; net PP&E = 48,000 + 10,000 − 6,000 = **52,000**
> - **Total assets = 84,810**
> - AP = 9,000 × 1.03 = **9,270**; accrued = **6,000**; debt = **25,000**; equity = 40,000 + 4,660 = **44,660**
> - **Total liabilities and equity = 84,930**
>
> **(3) Stressed EFN** = 84,810 − 84,930 = **−120** (still a surplus, but only \$120 thousand instead of \$650)
>
> **Why the financing position "improves."** Growth collapsed from +15% to +3%, so the working-capital investment fell from \$2,700 to \$540 (receivables +450, inventory +360, payables +270) while CapEx stayed at \$10,000 and the firm still earned \$6,657 of net income and \$6,000 of depreciation. Cash generation therefore fell far less than earnings: the cash reconciliation gives 6,657 + 6,000 − 10,000 − 540 − 1,997 = **+120**. The plan still balances — but at a margin of \$120 on \$84.8M of assets it is one assumption away from needing external money, while EBIT has fallen 32% and net income 37%. **The plug measures balance-sheet closure, not earnings health.**

> [!danger] The lesson the plug cannot give you
> Compare the two cases: base case EBIT \$17,000 → stressed EBIT \$11,510 (**−32%**); net income \$10,500 → \$6,657 (**−37%**); and yet the *surplus* shrank from \$650 to \$120 rather than turning negative. A committee that tracked only the financing plug would have seen the plan's surplus erode by 82% without ever hearing that earnings had fallen by a third. **Stress analysis must read both statements.**

---

### IV. Stress-Testing Tesla's FY2026 Plan

The base case ([[M7-Obj-7-1]] §IV): revenue +10.0%, cost of revenues 82.0% of sales, R&D 6.8%, SG&A 6.2%, restructuring \$500M, D&A \$7,000M, CapEx \$10,000M, cash and investments held at \$44,059M, DSO 17.61 / DSI 58.19 / DPO 62.78 days, tax 27%, no dividends.

#### Four coherent worlds

| Scenario | Revenue growth | Cost of revenues | SG&A | Revenue | EBIT | EBIT margin | Net income | EFN |
|---|---|---|---|---:|---:|---:|---:|---:|
| **Upside** | +18% | 80.5% | 6.0% | 111,896 | 6,997 | 6.25% | 6,088 | **−2,419** |
| **Base** | +10% | 82.0% | 6.2% | 104,310 | 4,716 | 4.52% | 4,422 | **−1,063** |
| **Mild (stall)** | 0% | 82.0% | 6.2% | 94,827 | 4,241 | 4.47% | 4,076 | **−1,076** |
| **Downside (price war)** | +2% | 83.5% | 6.8% | 96,724 | 2,305 | 2.38% | 2,662 | **+391** |
| **Severe (recession)** | −10% | 85.0% | 7.0% | 85,344 | 524 | 0.61% | 1,362 | **+1,246** |

All figures \$M. Note the two most instructive rows: the **mild stall** (revenue flat, ratios unchanged) produces EBIT of \$4,241 — **\$114M below the FY2025 actual of \$4,355** — purely from rounding the cost ratios (81.97% → 82.0%, 6.76% → 6.8%, 6.15% → 6.2%) and holding restructuring at \$500M. At Tesla's scale, half a point of ratio is real money, and a forecast that "changes nothing" is not the same model as the one that reproduces last year.

And note the **severe** case: EBIT collapses to \$524M — a 0.61% margin — and the plan needs **\$1,246M** of external money. The fortress that made the base case comfortable is now a **source** of the problem: Tesla's own cash pile is the thing being consumed, and the plug is the measure of how fast.

#### Two-variable sensitivity grid: EFN by revenue growth and cost of revenues

(\$M; SG&A held at 6.2%; negative = surplus, positive = external financing needed)

| Revenue growth ＼ Cost of revenues | 80.0% | 82.0% | 83.5% |
|---|---:|---:|---:|
| **−10%** | −2,314 | −1,090 | −171 |
| **0%** | −2,437 | −1,076 | −56 |
| **+10%** | −2,559 | −1,063 | +60 |
| **+20%** | −2,682 | −1,049 | +175 |

**Reading the gradients (this is the point of the grid):**

1. **Down the 82.0% column, almost nothing happens.** Moving revenue growth across a 30-point range (from −10% to +20%) shifts EFN by only \$41M. For this balance sheet, *growth is nearly irrelevant to the financing need*.
2. **Across the 83.5% row, the sign flips.** At +10% growth the plan needs \$60M; at +20% it needs \$175M — while at −10% it still shows a \$171M surplus. Margin, not volume, decides whether Tesla must go to the market.
3. **Along the 80.0% column the sign of the growth effect reverses.** Better margins *reward* growth (each point of growth adds surplus, because the fixed base is spread over more revenue — operating leverage working in reverse), while at 83.5% growth *consumes* surplus.
4. **The centre of the grid is the worst place to be.** The most likely forecast world (moderate growth, decent margin) sits near EFN = 0, where the plan is exactly self-funding and has no buffer for a bad surprise.

#### The switch points (break-even analysis)

| Question | Answer | How it is read |
|---|---|---|
| At an 83.5% cost-of-revenues ratio, what growth keeps the plan self-funding? | **+4.8% revenue growth** (EFN = 0 exactly) | A lender can say: "we lend against 4.8% growth, not 10%" |
| At +10% growth, what cost ratio keeps the plan self-funding? | **83.4%** of sales — i.e. **1.4 points of margin headroom** over the base case's 82.0% | The margin covenant the plan really needs |
| How much of the base-case surplus is cushion? | \$1,063M on \$142,507M of assets — **0.75% of the balance sheet** | Thin, because the base case is already holding cash flat at \$44,059M |

> [!danger] The finding that should change your credit view
> For most companies, the financing need is a **growth** problem: you need money because you are growing. For Tesla in this model, it is a **margin** problem: growth is nearly free (working capital and earnings roughly offset), while margin is expensive (it consumes the surplus and eventually the cash pile). The reason is the fortress itself — \$44,059M of cash and investments sitting between the plan and the market. That fortress is what buys Tesla time ([[M6-Obj-6-1]] §IV), and it is also what converts a mild operating disappointment into a *financing* event. **Do not read "self-funding" as "riskless": read it as "the margin has 1.4 points of room before the company becomes a capital-market borrower."**

---

### Key Terms

| Term | Definition |
|------|------------|
| **Single-variable isolation** | Changing one assumption at a time and recording the effect; the standard sanity check and the standard source of overconfidence |
| **Scenario analysis** | Re-running the whole model under a coherent set of assumptions describing a plausible world |
| **Break-even (switch-point) analysis** | Solving for the assumption value at which the output changes character — e.g. the growth rate at which EFN turns positive |
| **Sensitivity gradient** | The rate at which the output changes per unit of an assumption; the ranking of which assumptions actually matter |
| **Operating-leverage interaction** | Volume declines compress margin because fixed overhead does not shrink |
| **Working-capital release** | Contraction frees cash as receivables and inventory shrink — a cushion that can mask deteriorating earnings |
| **Plug blindness** | Monitoring the financing plug while ignoring the earnings path; the classic false comfort in a downturn |
| **Margin headroom** | The number of percentage points a cost ratio can deteriorate before the plan needs external money |
| **Assumption register** | The disclosed list of every assumption, so a reader can re-run the stress set themselves |

---

> [!danger] Red Flags — Stress-Test Discipline
> - A base case with no downside case attached
> - Single-variable stresses that hold cost ratios flat while revenue moves — the assumption that understates the damage
> - A stress set where related assumptions move in *opposite* directions from how they would behave in reality
> - Reading an improved EFN in a downturn as good news without reading the income statement
> - Presenting scenarios with likelihood weights, which hides judgment inside arithmetic
> - No switch point: a table of outcomes but no statement of *how far* an assumption can move
> - A grid whose two axes are not the two assumptions that actually drive the output
> - Forgetting that interest on new borrowing changes the plug that sized the borrowing

---

### Review Questions

> [!question]- Q1: What is the difference between a scenario, a sensitivity table, and a break-even analysis — and which one would you put in front of a lender?
> A scenario re-runs the whole model under a coherent description of a world; a sensitivity table shows how one output moves as one assumption moves; a break-even solves for the assumption value at which the answer flips character. The lender wants the break-even, because it is negotiable: "we are comfortable down to 4.8% growth" is a covenant conversation, whereas a scenario table is a story.

> [!question]- Q2: In the Titan downturn, why did the surplus fall from \$650 to \$120 while net income fell 37%?
> Because the plug depends on the *cash* bridge, not the earnings line. Growth collapsed from +15% to +3%, so working-capital investment fell from \$2,700 to \$540 while CapEx stayed put and the firm still earned \$6,657 of net income plus \$6,000 of depreciation. Cash generation therefore fell much less than profit.

> [!question]- Q3: Name the four interdependencies that break the "all else equal" assumption, and the direction each one pushes.
> (1) Volume down → margin down (fixed overhead under-absorbed); (2) revenue down → working capital released (a cushion that flatters the plug); (3) rates up → interest up → retained earnings down → plug up (and the plug is self-referential); (4) the plug measures balance-sheet closure rather than earnings, so the financing test can pass while the income statement collapses. Three of the four flatter the plan and one worsens it — which is why isolated stresses understate risk.

> [!question]- Q4: In Tesla's grid, EFN at +10% growth and an 83.5% cost ratio is +60, but at −10% growth it is −171. Why does *less* growth produce a *smaller* financing need at the same margin?
> Two offsetting effects: contraction releases working capital (receivables and inventory shrink faster than payables), which is a cash inflow, while lower volume also lowers the cost base and the absolute EBIT. The net effect at 83.5% is still a surplus, so the plan looks better on the financing test while its earnings capacity has deteriorated — a case of plug blindness.

> [!question]- Q5: What does the +4.8% break-even growth figure mean, and what would you negotiate with it?
> It is the growth rate at which an 83.5% cost-of-revenues ratio leaves the plan exactly self-funding (EFN = 0). Negotiated, it becomes a covenant or guidance condition: the lender can require evidence that revenue is growing at least 4.8%, or that the cost ratio is below 83.4%, because either alone keeps the plan off the capital market.

> [!question]- Q6: Why does the mild stall case (0% growth, ratios unchanged) produce EBIT of \$4,241 rather than the FY2025 actual of \$4,355?
> Because the forecast uses rounded ratios (82.0% vs. 81.97%, 6.8% vs. 6.76%, 6.2% vs. 6.15%) and holds restructuring at \$500M against an actual \$494M. Rounding in the *assumptions* is a real forecast decision with a real P&L consequence: at Tesla's scale, half a point of cost ratio is roughly \$475M of EBIT. A model that "changed nothing" is not the same model as one that reproduces last year.

---

### Practice Activity

> [!tip] Warm-up path
> New to the material? Do tasks 1–2 with §IV's grid open; tasks 3–5 belong after the Module 7 quiz.

You are the analyst presenting stress results to Tesla's credit committee, using the §IV scenario set and grid:

1. **Re-run the downside.** Compute the downside scenario's EBIT, net income, and EFN yourself (revenue +2%, cost of revenues 83.5%, SG&A 6.8%), then reconcile the EFN with a cash bridge. Confirm that the balance sheet and the cash statement agree before you show anyone a number.
2. **Build one axis of the grid.** Reproduce the 82.0% cost-of-revenues column for growth of −10%, 0%, +10%, and +20%, and state in one sentence what the column's flatness tells you about Tesla's financing risk.
3. **Find the switch point.** Solve for the revenue growth at which the plan is exactly self-funding at an 83.5% cost ratio. Then state what a lender would ask you to covenant.
4. **Name the worst world.** Construct a coherent scenario more severe than the severe case (three or more assumptions moving together) and report the EFN. Then state, in two sentences, what the \$44,059M cash pile does for the company in that world — and what it costs the company to hold.
5. **Write the committee sentence.** One sentence that quotes the base-case EFN, the downside EFN, and the switch point, and states which assumption the committee should monitor weekly.

---

### Related Notes

- [[M7-Overview]] — Module 7 overview
- [[M7-Obj-7-1]] — the forecast and plug this note stresses ([[M7-Obj-7-1]] §IV holds the base case)
- [[M7-Obj-7-3]] — Next: value the projected cash flows; stress-testing the valuation is the same discipline applied to the discount rate
- [[M3-Obj-3-1]] — margin ratios and operating leverage behind the cost-ratio assumptions
- [[M6-Obj-6-1]] — operating leverage (§II.2), the equity cushion, and the fortress balance sheet this stress set leans on
- [[M6-Obj-6-2]] — covenant tripwires and the reporting limits that can hide a deterioration
- [[M5-Obj-5-3]] — the core-earnings stack; a stress case built on reported earnings is a stress case built on the wrong base

---

> [!info] Sources
> - Tesla, Inc. FY2025 Form 10-K (filed Jan 2026), SEC EDGAR (accession `0001628280-26-003952`) — FY2025 balance sheet, income statement, and cash-flow lines used as the stress base
> - Titan Dynamics worked cases (base case and downturn) compiled from the course reference: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed), Part IV (Ch. 12 & 14, "Forecasts and Security Analysis")
> - All Tesla scenario assumptions and the grid in §IV are instructor-set for teaching; they are not Tesla guidance
> - Cross-referenced Tesla figures validated in [[M2-Obj-2-1]], [[M4-Obj-4-1]], and [[M6-Obj-6-1]]
