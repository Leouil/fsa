---
title: M8-Obj-8-2 - Tailor Financial Reports to the Reader and Deliver the Capstone
created: 2026-11-12
date: 2026-11-12
tags:
  - FSA
  - M8
  - Objective-8-2
  - Capstone
aliases:
  - stakeholder-tailoring
  - credit-memo
  - equity-research-thesis
  - course-capstone
---

# Learning Objective 8.2

## Tailor Financial Reports to the Reader and Deliver the Capstone

**By the end of this note, you can:**
- Map the four institutional audiences of financial analysis — equity research, lenders, board/management, and M&A — to their objectives, metrics, and characteristic blind spots
- Take one body of evidence and write **four different, defensible documents** from it, changing the lead metric, the risk framing, the recommendation type, and what you leave out
- Produce a lender-grade credit memo on Tesla from FY2025 filings — liquidity, coverage, payback, and a facility decision with a price
- Produce an investor-grade thesis on the same company from the same filings, and explain why the two documents disagree without contradicting each other
- Specify and defend the **course capstone deliverable**, with an evidence standard and a grading rubric

> [!tip] How to read this note
> Read §I–II for the stakeholder map and the capstone anchor, then build the two-pack exercise in §III with the model numbers collapsed, then use §IV's rubric to scope the capstone project. In §III and the Review Questions, **attempt each task before expanding a solution**.

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc. (FY2025 Form 10-K) — the same company, four audiences, two documents
> Every number in this objective comes from Tesla's FY2025 Form 10-K and the verified layers of Modules 2–7. Nothing new has to be computed from scratch: the analysis is done, and the work is **presentation** — deciding what to lead with, what to call the risk, what to recommend, and what to leave on the table.
>
> That is the module's real skill. Any analyst can produce the numbers; the professional distinction is in *framing the same numbers for readers whose incentives differ*. A lender who reads an equity-research thesis will find it unusable, not because it is wrong, but because it is answering a different question.

The stakeholder map, and where each audience's evidence comes from:

| Audience | Primary objective | Lead metrics | Characteristic blind spot |
|---|---|---|---|
| **Equity research** | Estimate intrinsic value and prospective growth | FCF, DCF value, ROE (Du Pont), P/E, EV/EBITDA, revenue CAGR | Tolerates leverage when ROE is magnified; upside-oriented, so downside asymmetry goes unexamined |
| **Lenders & creditors** | Evaluate payback probability and default risk | Quick ratio, cash-flow liquidity, debt/CFO payback, fixed-charge coverage, Altman Z | Asymmetric payoff: no upside beyond interest, ~100% loss in default — so they discount the equity story entirely |
| **Board & management** | Assess operating efficiency and capital allocation | Segment margins, asset turnover, working-capital velocity, EFN, ROIC | Natural incentive to present optimistic projections that lower the cost of capital |
| **M&A analysts** | Value the target, size the leverage, price the synergies | TEV, normalized EV/EBITDA, LBO debt capacity, impairment risk | "P/E multiple alchemy" — paying for synergies that the target's own numbers cannot fund |

<div style="display:flex;flex-direction:column;align-items:center;gap:0.5rem;margin:1rem 0">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.4rem;font-weight:600">ONE EVIDENCE BASE · FOUR DECISIONS</div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;align-items:stretch;gap:0.75rem;width:100%">
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Equity research</b><br/><span style="font-size:0.85em">Focus: upside growth<br/>FCF &middot; ROE &middot; P/E &middot; DCF<br/><b>Decision:</b> buy / hold / sell</span></div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Credit memo</b><br/><span style="font-size:0.85em">Focus: downside protection<br/>liquidity &middot; coverage &middot; payback<br/><b>Decision:</b> approve / deny / reprice</span></div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>Board briefing</b><br/><span style="font-size:0.85em">Focus: strategic fit &amp; allocation<br/>ROIC &middot; asset turnover &middot; CCC<br/><b>Decision:</b> proceed / defer / reallocate</span></div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 0.9rem;flex:1 1 180px;max-width:260px;text-align:left"><b>M&amp;A / buy-side</b><br/><span style="font-size:0.85em">Focus: price &amp; leverage<br/>TEV &middot; normalized EV/EBITDA<br/><b>Decision:</b> bid / pass / structure</span></div>
  </div>
</div>

---

### I. Stakeholder Orientation: Customizing the Narrative

#### 1. The same facts, four stories

Take Tesla's FY2025 facts — every one of them verifiable in the 10-K:

| Fact (FY2025)                                |                        Figure |
| -------------------------------------------- | ----------------------------: |
| Revenue                                      |                        94,827 |
| EBIT                                         |          4,355 (4.59% margin) |
| Of which policy-dependent regulatory credits |         1,993 (45.8% of EBIT) |
| EBIT ex-credits (normalized)                 |          2,362 (2.49% margin) |
| CFO                                          |                        14,747 |
| CapEx                                        |                         8,527 |
| Free cash flow (CFO − CapEx)                 |                         6,220 |
| Cash and short-term investments              |                        44,059 |
| Total debt and finance leases                |                         8,376 |
| Net cash                                     | **35,683** (\$9.51 per share) |
| EBIT interest coverage                       |                         12.9× |
| Debt/CFO payback                             |                    0.57 years |
| Debt-to-capital                              |                          9.2% |
| Quick ratio / cash-flow liquidity            |                 1.53× / 2.00× |
| Altman Z (M6 work)                           |             19.93 → Safe zone |
| EBITDA                                       |                        10,503 |
| EV / EV-to-EBITDA                            |        1,651,217 / **157.2×** |
| P/E on reported / core EPS                   |               416.4× / 661.1× |
| Market capitalisation                        |                     1,686,900 |

Read those facts as four different professionals, and you get four different reports:

- **The equity analyst** leads with the 157.2× EV/EBITDA and the 661.1× core P/E and concludes that the price is an *output of expectations*, not an anchor: the whole case rests on a growth and margin path far beyond FY2025's 2.49% normalized EBIT margin. **Recommendation: hold — the multiple is a statement about the future, and the future must be underwritten explicitly.**
- **The lender** never reaches the multiples. She leads with net cash of \$35,683M, 12.9× coverage, and 0.57-year payback, and asks the question the equity analyst skipped: what happens if the 45.8% of EBIT that comes from credits that phase out by law actually goes to zero? **Recommendation: approve the facility, and price the covenant against normalized, not reported, EBIT.**
- **The board member** asks about capital allocation: \$8,527M of CapEx against \$6,220M of free cash flow, a 107→13-day working-capital cycle that keeps releasing cash, and 535M shares issued during 2025 (+16.6%) while stock-based compensation of \$2,825M consumed 73% of net income. **Recommendation: fund the next leg without further equity, and explain the dilution.**
- **The acquirer's analyst** computes that a peer 8.0× EV/EBITDA would value Tesla's operating assets at \$84,024M — **19.7× below** the \$1,651,217M the market pays — and then finds the leverage ceiling: at a 1.5× EBITDA coverage floor and a 13% cost of debt, only about \$53,862M of debt is serviceable, so a strategic buyer at the market price funds with equity. **Recommendation: no bid at peer multiples; the target is priced for a plan, and diligence should test the plan, not the earnings.**

> [!danger] Tailoring is not spin
> All four readings above are **true of the same company** — that is what makes them defensible. What separates tailoring from spin is that the analyst's *evidence* does not change with the audience, only the **question answered, the order of presentation, the risk emphasized, and the decision requested**. If the numbers change when the audience changes, the analyst is not tailoring a report — they are writing two different stories and calling one of them analysis.

#### 2. What actually changes when you tailor

| Dimension | Equity research | Credit memo | Board / M&A |
|---|---|---|---|
| The question | What is it worth, and what is the upside? | Can it pay, and what is the loss if it cannot? | Where should capital go, and what must we fix? |
| Lead metric | FCF and forward margin path | Liquidity, coverage, payback | ROIC, working-capital velocity, EFN |
| Risk emphasized | Terminal-value and multiple risk | Downside, covenant, refinancing | Execution, competitive, allocation |
| Recommendation type | Buy / hold / sell | Approve / decline / reprice | Proceed / defer / reallocate |
| What to omit | Nothing material — but lead with the thesis | Equity optionality and the upside case | The committee politics and defensive framing |
| Length & tone | Narrative, thesis-driven, 1 page summary | Terse, evidence-table, conditional | Decision-first, options and consequences |

#### 3. The report that does not fit its reader

A credit memo that opens with the revenue CAGR is a company overview, not a credit memo. An equity thesis that buries the multiple is a prospectus, not a thesis. A board memo that omits the downside is an advocacy document. The test is simple: **would this reader's decision change if this sentence moved?** If not, it does not belong in their document.

---

### II. The Capstone Anchor: Eight Modules on One Company

Applying the whole course to **Tesla, Inc.** is the capstone experience. Each module supplies one layer of the same file; a professional report on Tesla is the assembly of all of them.

| Module | What it contributes to the Tesla file |
|---|---|
| [[M1-Obj-1-1]] – [[M1-Obj-1-3]] | Adversarial reading: what a filing can and cannot be made to say; the assumptions behind "reported" numbers |
| [[M2-Obj-2-1]] – [[M2-Obj-2-3]] | Statement mechanics: the classified balance sheet, income-statement anatomy, and the cash-flow statement that explains the earnings |
| [[M3-Obj-3-1]] – [[M3-Obj-3-3]] | Common-sizing, trends, and the Du Pont decomposition of the return |
| [[M4-Obj-4-1]], [[M4-Obj-4-2]] | Industry structure and Tesla's strategic position (vertical integration, FSD, charging network) against global automotive economics |
| [[M5-Obj-5-1]] – [[M5-Obj-5-3]] | Earnings quality: the credit windfall and the tax effects stripped out to reach core earnings |
| [[M6-Obj-6-1]], [[M6-Obj-6-2]] | Risk: liquidity and coverage, operating leverage, the distortions (leases, guarantees), and the distress-model read |
| [[M7-Obj-7-1]] – [[M7-Obj-7-3]] | The forward view: pro forma statements and the financing gap, stress cases and switch points, and the valuation with its assumption set |
| **This module** | The report: the seven steps, the audience, the decision, and the recommendation |

**Why Tesla is the right capstone subject.** It is the rare company where every analytical muscle finds something: a cash fortress that makes the credit trivial; a profit line where 45.8% comes from a legally scheduled windfall; a 157× multiple that forces the reverse-DCF question; an 8.53B capex program against 6.22B of free cash flow; a 535M-share issuance; and a product strategy that the numbers cannot yet settle. There is no boring part of the file.

---

### III. Worked Calculation: The Two-Pack (Credit Memo and Equity Thesis)

> [!tip] Before you flip any answer
> Attempt both documents before opening the model. Each must be two sentences of recommendation plus the supporting table, and each must be *independently* defensible to its own reader.

#### Scenario

You are at an institutional investor. The same analyst team must produce two documents on **Tesla, Inc.** from the FY2025 Form 10-K and the Dec 31, 2025 close of **\$449.72**:

- a **credit memo** supporting a request for a **\$2.0 billion revolving credit facility**, and
- an **equity research thesis** with a rating.

#### Task 1 — The credit memo (lender's view)

Compute from the data pack: **net debt**, **quick ratio**, **cash-flow liquidity ratio**, **EBIT interest coverage**, **debt/CFO payback**, and **debt-to-capital**. Then write a **two-sentence** credit recommendation for the \$2.0B facility, including the pricing basis and the one covenant condition you would require.

> [!success]- Solution (model)
> **Credit metrics:** net debt = 8,376 − 44,059 = **−\$35,683M (net cash)**; quick ratio = (44,059 + 4,576) ÷ 31,714 = **1.53×**; cash-flow liquidity ratio = (44,059 + 4,576 + 14,747) ÷ 31,714 = **2.00×**; EBIT interest coverage = 4,355 ÷ 338 = **12.9×**; debt/CFO payback = 8,376 ÷ 14,747 = **0.57 years**; debt-to-capital = 8,376 ÷ (8,376 + 82,137 + 728) = **9.2%**.
>
> **Credit recommendation (model):** *Approve the \$2.0 billion revolver at prime plus a nominal spread: the credit is cash-backed, with \$35,683M of net cash covering the facility roughly eighteen times over, 12.9× interest coverage, and a 0.57-year payback of all debt. Condition the facility on an EBIT-based covenant measured on **normalized** earnings — reported EBIT of \$4,355M includes \$1,993M (45.8%) of regulatory credits that phase out by law, and a lender should never covenant against an input with a sunset clause.*
>
> **Grading note:** credit-quality answers earn full marks only if the lender's own lens is respected — no equity optionality, no price target, and the risk stated as a **downside** (what is lost if the windfall ends and the capex continues). A memo that says "the stock is expensive" has been written to the wrong reader.

#### Task 2 — The equity thesis (investor's view)

Compute **free cash flow** (CFO − CapEx), **normalized operating income** (EBIT excluding regulatory credits), the **reported P/E** and the **normalized core P/E** at the \$449.72 close, and the implied **EV/EBITDA**. Then write a **two-sentence** thesis with a rating (buy / hold / sell) and the single condition that would change it.

> [!success]- Solution (model)
> **Metrics:** FCF = 14,747 − 8,527 = **\$6,220M** (6.56% of revenue); normalized EBIT = 4,355 − 1,993 = **\$2,362M (2.49% margin)**; reported EPS \$1.08 → **P/E 416.4×**; core net income = 3,855 − 1,993 × 0.73 = \$2,400M → core EPS \$0.68 → **core P/E 661.1×**; EV \$1,651,217M ÷ EBITDA \$10,503M = **157.2×**.
>
> **Investment thesis (model):** *Hold — the cash generation is real (\$6,220M of free cash flow, a fortress balance sheet, and 0.57-year debt payback), but at 416× reported and 661× core earnings the price is an output of expectations rather than an anchor, and the operating base supporting it is a 2.49% normalized EBIT margin. We would upgrade on evidence that normalized margin can scale toward the mid-teens, and downgrade if the credit's phase-out arrives without that scale.*
>
> **Grading note:** the thesis earns full marks for **naming the conditional structure of the valuation** — that the multiple is underwritten by a future, not by FY2025 — and for stating what would change the call. It loses marks if it declares the stock "overvalued" or "undervalued" without the assumption set behind the claim: the 12.7× gap between the market's enterprise value and a three-year illustrative DCF is a fact about assumptions ([[M7-Obj-7-3]] §V), not a verdict.

#### The reconciliation question (do not skip)

**A lender approves a \$2.0B facility; an equity analyst rates the stock Hold.** Are they contradicting each other? Explain in three sentences. (Model answer: *No — they answer different questions with the same evidence. The lender is paid interest with limited downside given \$35,683M of net cash and 0.57-year payback, so an approval is a low-risk decision at an unattractive but irrelevant price; the equity holder's payoff is entirely the residual after a 661× multiple, so the position is high-variance. The documents disagree only if one of them imports the other's conclusion — which is why the memo must not contain a price target and the thesis must not contain a facility recommendation.*)

---

### IV. The Course Capstone Project

> [!tip] The capstone is AI-assisted, and that is the point
> Module 8's project is **"The AI Analyst"**: students design the prompt chain that makes Microsoft Copilot draft Tesla's full initiation report, then they **audit every number the model produced** and own the four judgments that make the report a report. The brief, the full prompt chain, the grading rubric, and the AI-use disclosure live in [[PROJECT-M8-AI-Analyst-Prompt-Pack]]; the instructor key with the reference numbers lives beside it. What follows is the assignment's logic, not its mechanics.

#### 1. The deliverable

A **professional initiation report on Tesla, Inc.** (FY2025 Form 10-K base) in two forms:

1. **The report** — executive summary plus the seven steps (per [[M8-Obj-8-1]] §II), with every figure traced to the 10-K or to a lecture citation, and an explicit recommendation.
2. **The adapted pack** — the same evidence recast as (a) a one-page **credit memo** and (b) a **one-page equity thesis** (per §I and §III of this note), plus a short note of **what you changed and why** when you adapted them.

#### 2. Who does what

The model drafts; the students decide. The graded objects are the **audit trail** (verification log + AI error log, 45 points), the **four judgments** (20 points), and the **quality of the prompt chain** (10 points) — not the prose the model produced. That is why the project is a learning exercise rather than a typing exercise: a report Copilot writes without supervision fails the audit phase, and the failures are visible in the numbers.

#### 3. Evidence standards (non-negotiable)

- Every number traces to the FY2025 10-K (or the FY2023 10-K where a three-year series is used) or to a named lecture note and section — and to the verified **Tesla Capstone Data Pack**, which is the grounding file students hand to the model.
- Earnings are **normalized** before any multiple, trend, or return is quoted ([[M5-Obj-5-3]]).
- Forecasts disclose the assumption set and the single most sensitive assumption ([[M7-Obj-7-1]], [[M7-Obj-7-2]]) — and confront management's own capital-expenditure expectation, which the model will never volunteer unprompted.
- Valuation is quoted as a **range with its assumption set**, never a single number ([[M7-Obj-7-3]]).
- Where the report states a recommendation, it states the **conditions that would invalidate it**, and it presents **no price target**.

#### 4. Grading at a glance

| Criterion | Points | Full marks in one line |
|---|---:|---|
| Verification quality | 30 | Every figure logged with a source, a method, and a result; nothing unresolved |
| AI error diagnosis | 15 | Errors named, classified, explained, corrected — including consequential ones |
| Analytical judgment | 20 | Causal thesis; the four judgments are the student's, with reasons |
| Report structure & communication | 15 | Seven steps in argument order; executive summary stands alone |
| Audience fit | 10 | Framing and decision type change; evidence stays invariant |
| Prompt engineering | 10 | Grounded, chained, self-checking prompts; versioned log |
| Ethics & disclosure | 5 | Honest AI-use statement; limitations acknowledged |

#### 5. Suggested schedule

- **Week 1:** the brief, the thesis memo with its five claims, and the audit log opened.
- **Week 2:** Steps 1–4 drafted (industry, strategy, quality, diagnosis) with the first verification pass.
- **Week 3:** Steps 5–7 (forecast, valuation, recommendation) plus the executive summary.
- **Week 4:** the audit phase, the red-team phase, repairs, the adapted pack, and the pre-submission checklist from [[M8-Obj-8-1]] §IV.
- **Submit:** report; adapted pack; change log; verification log; AI error log; prompt pack; AI-use disclosure.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Stakeholder orientation** | Deliberately shaping the same evidence to the decision the reader must make |
| **Equity research thesis** | Buy/hold/sell document leading with forward cash flow, returns and valuation |
| **Credit memo** | Approve/decline document leading with liquidity, coverage, payback and downside |
| **Board briefing** | Decision document leading with operating efficiency, capital allocation and consequences |
| **Institutional bias** | The structural incentive that makes each audience's reading asymmetric — lenders have no upside beyond interest |
| **Multiple alchemy** | Concocting a P/E multiple from adjusted earnings to justify a price the business cannot fund |
| **Downside asymmetry** | For a creditor, recovery beyond interest is nil while loss on default approaches the whole claim |
| **Change-log note** | A short document stating what was changed when adapting evidence to a new audience, and why |
| **Falsifiable recommendation** | A recommendation with stated conditions that would reverse it |
| **Evidence standard** | The rule that every number in a professional document must be traceable to a filing or a cited note |

---

> [!danger] Red Flags — Professional Reporting
> - A recommendation whose evidence would not change if the call reversed
> - Management's MD&A framing repeated as the analyst's conclusion
> - A credit memo containing a price target, or an equity thesis containing a facility recommendation
> - Multiples quoted on unnormalized earnings, or a valuation quoted as a single number
> - A forecast with no assumption list, or with no statement of the most sensitive assumption
> - Numbers that appear in the summary but cannot be found in the body
> - An executive summary that depends on a page the reader has not reached
> - Audience tailoring that changes the *evidence* rather than only the framing
> - A report that describes the company instead of deciding for it

---

### Review Questions

> [!question]- Q1: What distinguishes tailoring from spin, given that both change the presentation of the same evidence?
> Tailoring changes the question answered, the order of presentation, the risk emphasized and the decision requested — while the evidence and the arithmetic stay identical. Spin changes the evidence itself: a different (usually more flattering) definition, a window that hides the bad year, a denominator chosen to flatter. The test: could an informed reader reconstruct the same numbers from your document? If yes, you tailored. If no, you spun.

> [!question]- Q2: Why does a lender's reading of Tesla's equity story not matter to the lender — and why is that a discipline, not a limitation?
> Because the lender's payoff is bounded above by the interest and bounded below by the claim, so the equity's optionality is not the lender's asset. The upside is irrelevant and the downside is everything, so the lender prices the loss scenarios and ignores the growth case. That discipline protects the lender from paying for a narrative she cannot be repaid by.

> [!question]- Q3: A credit analyst approves a \$2.0B revolver while the equity analyst rates the stock Hold. How can both be right?
> They answer different questions from the same evidence. The facility is repaid from cash generation and net cash that dwarfs the commitment, so approval is a low-risk decision at an unattractive price. The equity holder's residual payoff depends entirely on a 661× multiple being underwritten by a future margin path. The documents conflict only if one imports the other's conclusion — which is why the memo carries no price target and the thesis carries no facility recommendation.

> [!question]- Q4: In the credit memo, why covenant against normalized EBIT rather than reported EBIT?
> Because reported EBIT of \$4,355M includes \$1,993M (45.8%) of regulatory credits that phase out by law. A covenant measured on reported EBIT would tighten automatically as the credit disappears — through no change in the borrower's conduct — and would then trigger precisely when the lender most needs the borrower to keep performing. Covenant on the sustainable base.

> [!question]- Q5: Why does Tesla make a better capstone subject than a company with a clean, unremarkable file?
> Because a capstone should test the whole toolkit, and Tesla exercises every part of it: a cash fortress that trivializes the credit question; a profit line where nearly half comes from a windfall with a statutory sunset; a 157× multiple that forces the reverse-DCF question; capex far above free cash flow; a 535M-share issuance; and a strategy the current numbers cannot settle. A clean company would let a student submit the numbers and call it analysis.

> [!question]- Q6: What is the change-log note in the capstone pack for?
> It makes the tailoring auditable. Without it, a reader cannot distinguish deliberate audience adaptation from inconsistent or opportunistic analysis — and the document's credibility depends on the evidence being visibly invariant while the framing visibly changes.

---

### Practice Activity

> [!tip] Warm-up path
> New to the material? Do tasks 1–2 with §I's four readings open; tasks 3–4 belong after the Module 8 quiz.

Using the FY2025 Tesla data pack in §I:

1. **Write the four leads.** For each of the four audiences, write the single sentence you would put first. Then underline the figure each sentence leads with.
2. **Tailor one paragraph.** Take the paragraph you just wrote for the equity analyst and rewrite it for the board: same evidence, different lead, different risk emphasis, different decision requested. Underline what you changed and why.
3. **Draft the credit memo.** Compute the six credit metrics, then write the two-sentence recommendation and the covenant condition. Check it against the §III solution and note any metric you would have preferred but the data pack does not support.
4. **Draft the equity thesis.** Compute FCF, normalized EBIT, reported and core P/E, and EV/EBITDA, then write the two-sentence thesis with its rating and invalidation condition. Then answer the reconciliation question in one paragraph: why do the two documents not contradict each other?

---

### Related Notes

- [[M8-Overview]] — Module 8 overview
- [[M8-Obj-8-1]] — the seven-step architecture, the Sage initiation exercise, and the pre-submission checklist
- [[PROJECT-M8-AI-Analyst-Prompt-Pack]] — the capstone brief: the full Copilot prompt chain, the graded artifacts, and the AI-use disclosure
- [[M7-Obj-7-3]] — the valuation evidence behind the equity thesis, including the reverse DCF
- [[M7-Obj-7-1]] — the forecast evidence behind the credit memo (EFN, working capital) and the stress cases
- [[M6-Obj-6-1]] — the risk diagnostics behind both documents (coverage, payback, operating leverage)
- [[M6-Obj-6-2]] — the Altman Z read and the distortion map used in the equity document's risk section
- [[M5-Obj-5-3]] — the core-earnings stack: normalization before any multiple appears in either document
- [[M4-Obj-4-1]] — industry and strategy material for Steps 1–2 of the capstone report

---

> [!info] Sources
> - Tesla, Inc. FY2025 Form 10-K (filed Jan 2026), SEC EDGAR (accession `0001628280-26-003952`) — income statement, balance sheet, cash-flow statement, share counts, regulatory-credit revenue, dividend policy; TSLA close \$449.72 (Dec 31, 2025) per the verified source log in the instructor keys
> - Stakeholder frameworks and reporting architecture compiled from the course reference: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed) — Preface and case studies (Sunbeam; Oxford Health Plans)
> - Analytical frameworks carried forward from earlier modules: Du Pont decomposition, cash conversion cycle, Altman Z-score, Beaver debt/CFO payback, FCFF/WACC DCF, EV/EBITDA, and LBO debt-capacity arithmetic
> - Cross-referenced Tesla figures validated in [[M2-Obj-2-1]], [[M3-Obj-3-3]], [[M5-Obj-5-3]], [[M6-Obj-6-1]], and [[M7-Obj-7-3]]
