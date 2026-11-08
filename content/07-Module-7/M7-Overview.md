---
title: Module 7 - Forecasting and Business Valuation
created: 2026-11-08
date: 2026-11-08
tags:
  - FSA
  - M7
  - Overview
aliases:
  - forecasting-and-valuation
  - pro-forma-and-dcf
---

# Module 7: Forecasting and Business Valuation

> [!abstract] Module Purpose
> Modules 2–4 taught us to *read* financial statements; Module 5 to distrust their earnings; Module 6 to map the risks hiding inside them. Module 7 turns the instrument around: we now **write** the statements forward, **break** them, and then **price** what survives. Three objectives, one connected arc: build a pro forma statement and find the external financing the plan needs (LO 7.1), stress the assumptions until the plan changes character (LO 7.2), and convert the projected cash flows into a value and a decision (LO 7.3).
>
> The running example stays **Tesla, Inc.** (FY2025 Form 10-K) — deliberately a *hard* calibration case for forward-looking work: a firm whose plan self-funds, whose dividend model returns zero, and whose market multiples are far outside any peer anchor. The textbook cases (Fridson & Alvarez) supply the clean shapes — Titan Dynamics for the percentage-of-sales model, Aegis Technologies for the DCF, Solon and Vesta for capital-structure-neutral multiples.

<div style="display:flex;flex-direction:column;align-items:center;gap:0.5rem;margin:1rem 0">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.4rem;font-weight:600">THE THREE-STAGE FORWARD ARC</div>
  <div style="display:flex;width:100%;align-items:center;justify-content:center;gap:0.5rem;color:var(--secondary)">
    <div style="height:2px;flex:0 0 33%;background:var(--gray)"></div>
    <div style="font-size:0.85rem">&#9660;</div>
    <div style="height:2px;flex:0 0 33%;background:var(--gray)"></div>
  </div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;align-items:stretch;gap:0.75rem;width:100%">
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 200px;max-width:300px;text-align:left"><b>7.1 &middot; Build the plan</b><br/><span style="font-size:0.85em">Pro forma statements<br/>the EFN plug &middot; financing choices</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 200px;max-width:300px;text-align:left"><b>7.2 &middot; Break the plan</b><br/><span style="font-size:0.85em">Scenarios &middot; interdependencies<br/>break-even switch points</span></div>
    <div style="font-size:1.1rem;color:var(--secondary);align-self:center">&rarr;</div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 200px;max-width:300px;text-align:left"><b>7.3 &middot; Price the plan</b><br/><span style="font-size:0.85em">FCFF &amp; WACC &middot; terminal value<br/>multiples &middot; reverse DCF</span></div>
  </div>
</div>

## Learning Objectives

| Objective | Full Title | Analytical Focus |
|---|---|---|
| [[M7-Obj-7-1]] | Build Pro Forma Financial Statements and Determine External Financing Needs | Percentage-of-sales cost modeling &amp; fixed/variable distortion · sales anchors and price-volume decomposition · embedded cost of debt · DSO/DSI/DPO velocity anchors · PP&amp;E and retained-earnings roll-forwards · the EFN plug and its three absorption choices (debt, equity, cash) |
| [[M7-Obj-7-2]] | Stress-Test the Forecast: Sensitivity Analysis and Interdependent Risk | Single-variable isolation vs. scenario re-runs · the four interdependencies (volume→margin, revenue→working capital, rates→plug, plug≠earnings) · sensitivity-gradient reading · break-even (switch-point) analysis · plug blindness |
| [[M7-Obj-7-3]] | Value the Firm: Intrinsic (DCF) and Relative (Multiples) Valuation | Gordon-growth DDM and where it fails · FCFF construction (EBIT(1−t) + D&amp;A − CapEx − ΔWC) · WACC and its disclosure · terminal value and its dominance · enterprise-to-equity bridge · normalized P/E and the payout/(K−g) identity · EV/EBITDA capital-structure neutrality · reverse DCF |

> [!success] Key Findings from the Tesla Application
> - **The base plan self-funds — with almost no cushion.** The FY2026 forecast (revenue +10.0%, cost of revenues 82.0% of sales, CapEx \$10,000M) produces EBIT of \$4,716M and an **EFN of −\$1,063M**: a surplus worth 0.75% of a \$142,507M balance sheet. The cash reconciliation proves it: 4,422 + 7,000 − 10,000 − 359 − 0 = 1,063.
> - **The financing need is a margin question, not a growth question.** Moving revenue growth across a 30-point range shifts EFN by only \$41M; moving the cost-of-revenues ratio from 82.0% to 83.5% flips the plan from a \$1,063M surplus to a \$60M shortfall. Break-even: **+4.8% growth** is needed at an 83.5% cost ratio, and the break-even cost ratio at +10% growth is **83.4%** — 1.4 points of margin headroom.
> - **The plug can improve while earnings collapse.** In the Titan downturn, EBIT fell 32% and net income 37%, yet the surplus *shrank* from \$650 to \$120 rather than turning negative — because slowing growth releases working capital. Read both statements, never the plug alone.
> - **The dividend model returns zero, and that is informative.** Tesla has never declared or paid a cash dividend, so the Gordon DDM prices its equity at \$0. The method is not failing; value must be captured in the firm's free cash flow.
> - **Multiples are outputs, not anchors.** At the Dec 31, 2025 close, Tesla trades at **157.2× EV/EBITDA**, **416.4× reported P/E**, and **661.3× P/E on core EPS** (credits stripped) — multiples with no peer anchor, where a 1% move in the multiple shifts enterprise value by \$16.5B.
> - **A DCF is mostly a terminal-period statement.** An illustrative five-year FCFF path (WACC 9.0%, terminal growth 3.0%) yields enterprise value of \$130,447M and \$44.29 per share against a \$449.72 close — with terminal value at **84.8%** of EV, and discount-rate and terminal-growth choices alone spanning **97,645 to 195,981** (2.0×). The honest exercise is the reverse: what must be true for the market's \$1,651,217M enterprise value to be right?

## The Module 7 Analytical Framework

| Step | Technique | Question Answered | Where Applied |
|---|---|---|---|
| 1 | Sales anchor (bottom-up volume/price, nominal vs. real) | What drives the revenue line every other line hangs on? | [[M7-Obj-7-1]] §I–II |
| 2 | Percentage-of-sales cost model + fixed/variable split | How do costs behave as volume moves? | [[M7-Obj-7-1]] §II |
| 3 | Embedded cost of debt on projected debt | What will interest cost as the plan is financed? | [[M7-Obj-7-1]] §II |
| 4 | DSO/DSI/DPO velocity anchors | How much cash will growth consume before it returns? | [[M7-Obj-7-1]] §II |
| 5 | PP&E and retained-earnings roll-forwards | What does the balance sheet look like before financing? | [[M7-Obj-7-1]] §II |
| 6 | EFN plug and its absorption choice (debt, equity, cash) | What does the plan need from the outside world? | [[M7-Obj-7-1]] §II, §IV |
| 7 | Single-variable isolation and scenario re-runs | Which assumptions does the answer actually depend on? | [[M7-Obj-7-2]] §I |
| 8 | Interdependency mapping (volume→margin, revenue→WC, rates→plug, plug≠earnings) | Why is "all else equal" never true? | [[M7-Obj-7-2]] §II |
| 9 | Break-even (switch-point) solving | How far can an assumption move before the answer changes character? | [[M7-Obj-7-2]] §IV |
| 10 | FCFF construction and WACC discounting | What are these cash flows worth to capital? | [[M7-Obj-7-3]] §II |
| 11 | Terminal value and the enterprise-to-equity bridge | What happens after the explicit forecast, and what is left for shareholders? | [[M7-Obj-7-3]] §II |
| 12 | Normalized P/E, EV/EBITDA neutrality, reverse DCF | What does the market pay, and what must be true for it to be right? | [[M7-Obj-7-3]] §III, §V |

> [!tip] From Diagnosis to a Forward Decision
> Modules 2–6 built increasingly powerful tests applied to *one company at one point in time*. Module 7 asks the two questions that follow: **what happens next** (7.1–7.2) and **what is it worth** (7.3). The discipline carries over intact. A forecast is a set of assumptions; a valuation is a set of assumptions with a price attached; both must be stressed, disclosed, and reconciled with the statements that produced them. The skeptics' habit — read the notes, then read the numbers — is what keeps a projection from becoming a promise.

---

## Prerequisites

- Tesla FY2025 Form 10-K (filed Jan 2026) — income statement, balance sheet, cash-flow statement, dividend policy, share counts; FY2023–25 comparatives
- Fluency with the ratio machinery and common-sizing ([[M3-Obj-3-1]], [[M4-Obj-4-1]]) — DSO/DSI/DPO, margins, the DuPont chain
- The Module 5 earnings-quality vocabulary ([[M5-Obj-5-2]], [[M5-Obj-5-3]]) — normalized earnings and the core stack, which any multiple must be applied to
- The Module 6 risk vocabulary ([[M6-Obj-6-1]], [[M6-Obj-6-2]]) — operating leverage, the equity cushion, covenant tripwires, and the serial-restructurer test
- Balance-sheet mechanics ([[M2-Obj-2-1]], [[M2-Obj-2-3]]) — debt schedules, leases, and the working-capital lines that the forecast must roll forward
- Note: the discount rate and terminal assumptions used in this module are **instructor-set**; no financial statement contains them

---

## Book References

> [!info] Sources
> - Part IV, Chapters 12 and 14, "Forecasts and Security Analysis" — from the course reference: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed)
> - **Titan Dynamics** (percentage-of-sales pro forma and EFN) and the **Titan downturn** (margin compression) — LO 7.1 and 7.2
> - **Sage Inc.** (store-expansion planning) and **Colossal Chemical** (sensitivity under margin compression) — planning and stress cases from the same text
> - **Aegis Technologies** (two-stage FCFF/WACC DCF) and **Solon Corp. vs. Vesta Inc.** (EV/EBITDA capital-structure neutrality) — LO 7.3
> - **Sitting Duck Corp.** (LBO debt capacity: 1.5× EBITDA coverage floor, 13% borrowing rate, 10% sponsor equity) — LO 7.3, brief illustration only
> - Tesla figures verified against the FY2025 Form 10-K (accession `0001628280-26-003952`); TSLA close \$449.72 per Yahoo Finance / StatMuse (see instructor key for the logged source)

---

## Related Notes

- [[M6-Overview]] — Module 6 overview (the risk layer this module prices)
- [[M6-Obj-6-1]] — operating leverage, the equity cushion, and the fortress balance sheet behind Tesla's stress results
- [[M6-Obj-6-2]] — the pro-forma mirage and the serial-restructurer test; both bear directly on what may be projected
- [[M5-Obj-5-3]] — the core-earnings stack; normalization before any multiple
- [[M5-Obj-5-2]] — cash-flow quality; the cash a DCF discounts versus the earnings it starts from
- [[M3-Obj-3-1]] — margin and return ratios; the cost-ratio machinery of the forecast
- [[M2-Obj-2-1]] — the classified balance sheet; the debt and lease lines the forecast rolls forward
- [[Course-Overview]] — full program map
- Next: [[M8-Overview]] — professional financial analysis reporting
