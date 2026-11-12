---
title: "PROJECT — Module 8 \"The AI Analyst\": Tesla Initiation Report with Microsoft Copilot"
created: 2026-11-12
date: 2026-11-12
tags:
  - FSA
  - M8
  - Project
  - Gen-AI
aliases:
  - ai-analyst-project
  - capstone-project
  - prompt-pack
---

# PROJECT M8 — "The AI Analyst": Tesla's Initiation Report, Built with Copilot
## Module 8 · the final assignment of the course · Learning Objectives 8.1 and 8.2

**Due:** the end of Module 8 (weekly checkpoints in the schedule below)
**Team size:** 2–3 students
**Tools:** Microsoft 365 Copilot (your institutional licence) + this prompt pack + the two course workbooks
**Output:** the initiation report, the adapted pack (credit memo + equity thesis), and the graded audit trail

---

## 1. What this project is

Modules 2–7 gave you instruments. Module 8 asks for the **deliverable**: a professional initiation report on **Tesla, Inc.** (FY2025 Form 10-K) built on the seven-step framework of [[M8-Obj-8-1]], plus the two adapted documents (a credit memo and an equity thesis) required by [[M8-Obj-8-2]].

The twist is who does the typing. **Copilot drafts; you decide.** You design the prompt chain, you ground the model in the filing, you audit every number it produces, and you own the four judgments that make the report a report:

| Judgment | Why it cannot be delegated |
|---|---|
| **The thesis** | A causal claim about why this company earns what it earns — and what would change it |
| **The risk** | Which exposure binds first, and through which mechanism |
| **The leading evidence** | Which figures lead the report, and which are background |
| **The recommendation** | An explicit, falsifiable call, with invalidation conditions |

Your professor grades **the trail, not the prose**: the prompt pack, the verification log, and the AI error log are 45 of the 100 points, and the *judgments* are another 20. A report Copilot wrote on its own will fail the audit phase — the numbers will not reconcile, and the errors you failed to catch are the grade.

> [!tip] The one-sentence version
> **Let the model do the drafting and the arithmetic; do the sourcing, the auditing, and the deciding.** Every number in the final report must be traceable to the Tesla Capstone Data Pack or to a filing you opened yourself.

---

## 2. What you submit (and what each artifact is worth)

| Artifact | Where | Points |
|---|---|---:|
| **A. Prompt pack** — your full prompt chain, versioned, with what you changed and why | this document, completed and submitted as a log | 10 |
| **B. Verification log** — every figure and factual claim: value, source, your check, the AI's claim, the outcome | `Tesla-Capstone-Verification-Log.xlsx` | 30 |
| **C. AI error log** — every fabrication, miscalculation, misreading and instruction failure you caught | same workbook | 15 |
| **D. The report** — executive summary + the seven steps | your Word document | 15 |
| **E. The adapted pack** — credit memo + equity thesis + one-page change-log note | same document | 10 |
| **F. Analytical judgment** — thesis, risk, leading evidence, recommendation (with reasons) | inside the report, signed by the students | 20 |
| **G. AI-use disclosure** — tool, dates, phases, limitations | same workbook | 5 |

**Rules that protect your grade.** A report without the verification log caps at **45**; without the AI error log it caps at **85**. Unverified AI output is treated as an unverified claim. If a figure cannot be verified, remove it and say so in the error log — honest removal scores higher than a confident error.

---

## 3. Setup: Copilot in ten minutes

**Where to run each phase.** Use **Copilot chat** (Microsoft 365 Copilot in Edge, or the Copilot panel in Word) for every phase except phase 7, where you assemble in Word. Keep the report in a Word document and paste one section at a time.

**How to give it the data.** Two options; use whichever your licence supports:
1. *Upload* — in Copilot chat, add the file with **Add files / paperclip** and choose `Tesla-Capstone-Data-Pack.xlsx`.
2. *Paste* — open the workbook, select the sheet you need (for example the "Income statement" sheet), copy, and paste it into the chat with a one-line header naming the sheet.

Either way, tell the model which sheet it is looking at. Copilot reads spreadsheets unreliably when you hand it a whole workbook at once — **give it one sheet per message**, and ask for a table back.

**Web grounding.** Turn web search **on** for phases 2 (industry context) and **off** for phases 3–6 (everything that touches reported company figures). The pack is authoritative for Tesla; the web is for industry and macro context, and it must be cited with a URL and an access date.

**Keep the prompt log from minute one.** A single table you paste into the prompt pack: `Phase | Date | Prompt (full text) | Model output | What I changed | Why`. The log is graded, and it is also your own defence if a reviewer asks why a prompt was written the way it was.

**Copilot's default failure mode.** It will write fluently and confidently, and it will *sometimes* produce Tesla numbers that are wrong, stale, or invented. The prompts below are written to make that failure visible (grounding rule, label requirement, self-check, and a final audit). If a prompt you are given does not contain those guards, fix it before you run it — that repair is part of the assignment.

---

## 4. The chain

Nine phases plus an audit and a red team. **Do not skip ahead.** Each phase has a *checkpoint*: something you must do yourself before the next phase starts. The carry-forward protocol: at the start of every prompt, paste the previous phase's **approved** output as context, and tell the model it is the only context it may use.

---

### Phase 0 — Write the brief (you, no model)

**Goal.** A one-page instruction set that the model will follow for the rest of the project. This page is graded (it is the first artifact in your prompt pack).

**Include:** the as-of date (Dec 31, 2025) and the price to use; the audience (an equity initiation report); the seven required sections and what each must *prove* ([[M8-Obj-8-1]] §II); the data pack's label convention; the constraint set (no price target; pack-only for reported figures; every number carries a label; if a figure is missing, write `[NEEDED: …]`); the citation style; and the instruction that the model must not use its own memory about Tesla.

**Checkpoint.** You can defend every line of the brief against the course notes, and you have pasted it into every subsequent prompt.

---

### Phase 1 — Thesis candidates (model proposes, you choose)

**Paste first:** the brief, plus the "Derived (mechanical)" and "Facts & risk inputs" sheets.

> **Prompt 1**
> You are an equity research analyst preparing an initiation report on Tesla Inc. (FY2025 Form 10-K; as-of date Dec 31, 2025; reference price $449.72).
>
> **Ground rule:** use only the figures in the attached Tesla Capstone Data Pack. Every figure you use must be printed with its pack label (for example [IS-rev]). If you need a figure that is not in the pack, write `[NEEDED: description]` instead of estimating. Do not use any knowledge of Tesla from memory, and do not cite any source outside the pack for a company figure.
>
> **Task:** propose **three** candidate one-sentence theses for the initiation report. Each thesis must be a causal claim (industry → strategy → operations → accounting quality → forward view → value), not a description. For each thesis, list: (a) the thesis sentence; (b) the **five supporting claims** the report would have to prove, each with the pack labels that support it; (c) the **single biggest risk** and its mechanism; (d) the one piece of evidence a skeptic would attack; (e) the pack facts you used.
>
> **Rules:** at least one candidate must address the fact that regulatory credits are 45.8% of FY2025 EBIT [NORM-credits] / [DER-credits], and at least one must address management's 2026 capital-expenditure expectation [FACT-04]. Do not rank them. Do not write a recommendation.
>
> **Format:** a table with one row per candidate and the five columns above, then a short paragraph per candidate. Output only the table and paragraphs — no preamble.

**Checkpoint (your judgment).** You choose one thesis, or write your own — and you can defend each of its five claims with a pack label. **You** also decide which fact is the report's lead.

---

### Phase 2 — Steps 1–2: industry and strategy

**Paste first:** the brief, the approved thesis, the "Facts & risk inputs" sheet, and your own notes on what Steps 1 and 2 must prove.

> **Prompt 2**
> Continue the Tesla Inc. initiation report (brief and approved thesis below).
>
> **Ground rule:** use only the attached pack for any Tesla figure, and print the pack label. For industry and macro context you may use external sources, but each must be cited with the source name, the URL, and the access date, and any figure you take from a source must be shown with its source label. If a Tesla figure you need is not in the pack, write `[NEEDED: …]`.
>
> **Task:** draft **Step 1 (Industry economic characteristics)** and **Step 2 (Corporate strategic positioning)**.
>
> Step 1 must: name the structural forces that set the industry's profit ceiling, using current policy and market data (for example the OBBBA consumer-credit changes and residential-storage credit expiry [FACT-03], EV market growth and subsidy regimes); state which force binds hardest for Tesla; and connect that force to Tesla's 73.3% automotive revenue mix [FACT-07].
> Step 2 must: state Tesla's competitive position (differentiation and vertical integration, brand, software and charging), assess its durability, and support the assessment with pack figures where they exist.
>
> **Rules:** each section ends with a one-sentence conclusion that states what the reader can now conclude — not a summary of what you wrote. No forecasts, no valuation, no recommendation, no price target.
>
> **Format:** markdown prose (150–250 words per section), with every Tesla figure carrying its pack label in parentheses and every external figure carrying a source tag. Output only the two sections.

**Checkpoint.** Every Tesla figure in your draft matches the pack (check each one). Every external source is real, opened, and dated. You decide which claims are yours to assert.

---

### Phase 3 — Step 3: earnings quality and the normalization

**Paste first:** the brief, the approved thesis, the "Income statement", "Cash flow" and "Normalization inputs" sheets.

> **Prompt 3**
> Continue the Tesla Inc. initiation report (brief and approved thesis below).
>
> **Ground rule:** pack figures only, with labels; `[NEEDED: …]` for anything missing.
>
> **Task:** draft **Step 3 (Financial statement examination and quality assessment)**.
>
> 1. Start from reported FY2025 EBIT [NORM-ebit] and build to normalized EBIT [NORM-nomebit], showing the adjustments as a table: item, amount, label, and the reason (recurring or non-recurring). Include regulatory credits [NORM-credits], restructuring [NORM-restr] and stock-based compensation [NORM-sbc], and state explicitly which adjustments you do **not** accept and why.
> 2. Reconcile the FY2023–FY2025 earnings trend and flag any year where the reported figure is not the right base for a trend (note the FY2023 tax benefit and the caption changes).
> 3. Cross-examine management's MD&A claims against the statements and the facts sheet — in particular [FACT-02], [FACT-03] and [FACT-04] — and state where the narrative and the filing disagree, and which one governs.
>
> **Rules:** every adjustment shown as a number; no qualitative adjustment without a number attached; no forecast, valuation or recommendation.
>
> **Format:** (a) a normalization table; (b) 150–250 words; (c) a short bulleted list of the disagreements you found.

**Checkpoint.** You agree or disagree with each adjustment the model proposed — and for each disagreement you have a reason you can write in one sentence. You decide what the report claims about earnings quality.

---

### Phase 4 — Step 4: profitability and risk diagnosis

**Paste first:** the brief, the approved thesis, the "Derived (mechanical)" sheet (the audit baseline), and the balance-sheet and cash-flow sheets.

> **Prompt 4**
> Continue the Tesla Inc. initiation report (brief and approved thesis below).
>
> **Ground rule:** pack figures only, with labels; `[NEEDED: …]` for anything missing. You may compute ratios from pack figures, but you must print the formula and the inputs used for each one.
>
> **Task:** draft **Step 4 (Profitability and risk diagnosis)** for FY2023–FY2025:
> 1. Margins (gross, operating, net) and the trend, with the driver of the FY2024–FY2025 operating-margin decline identified by arithmetic, not assertion.
> 2. The three-factor Du Pont decomposition of ROE (net margin × asset turnover × equity multiplier) — state the balance convention you used for assets and equity and note the alternative.
> 3. Liquidity and coverage: quick ratio, cash-flow liquidity ratio, EBIT interest coverage, debt-to-CFO payback, debt-to-capital.
> 4. Working capital: DSI, DSO, DPO, cash conversion cycle, and what the FY2024–FY2025 movement means for cash.
> 5. A single "fragility" paragraph: the one metric that would move first if conditions changed, and why.
>
> **Rules:** each metric in a table with columns Metric | Formula | Inputs (with labels) | FY2023 | FY2024 | FY2025; one sentence of interpretation per metric; no forecast, valuation or recommendation.
>
> **Self-check before you output:** recompute every ratio a second time by a different route (for example margins from dollars rather than percentages, and ROE from the Du Pont product). Print only the metrics where the two routes disagree, each on a line beginning `CHECK:`. If nothing disagrees, print `CHECK: all metrics reconcile`.

**Checkpoint.** You independently recompute **three** metrics by hand — pick the ones the model flagged `CHECK:` on, plus one it did not. Any metric that does not match the pack's Derived sheet goes on your error log.

---

### Phase 5 — Step 5: the forecast

**Paste first:** the brief, the approved thesis, the income-statement, balance-sheet and cash-flow sheets, and [FACT-04].

> **Prompt 5**
> Continue the Tesla Inc. initiation report (brief and approved thesis below).
>
> **Ground rule:** pack figures only for reported data, with labels; `[NEEDED: …]` for anything missing. Every forecast assumption must be listed in a table with its value and its justification (a pack label, a filing fact, or "analyst judgment — reason given").
>
> **Task:** draft **Step 5 (Pro forma forecasts)** for FY2026–FY2028:
> 1. A forecast-assumption table: revenue growth, cost-of-revenues ratio, R&D and SG&A ratios, restructuring, D&A, CapEx, working-capital days, tax rate, dividends. Anchor CapEx on management's stated expectation [FACT-04] unless you justify a different figure in one sentence.
> 2. A projected income statement and a projected balance sheet (revenue, cost lines, EBIT, net income, then AR, inventory, PP&E, payables, debt, equity).
> 3. The **EFN** plug, and a cash reconciliation (net income + D&A − CapEx − Δworking capital) that must equal −EFN. Show the reconciliation even if it does not tie, and say what is wrong.
> 4. A sensitivity of the EFN to (i) revenue growth and (ii) the cost-of-revenues ratio, as a small table.
> 5. The **switch point**: the growth rate (and the cost-of-revenues ratio) at which the plan stops being self-funding, and the direction in which each must move.
>
> **Rules:** carry rounded values forward; state the convention; disclose which single assumption the answer is most sensitive to; no valuation or recommendation in this section.

**Checkpoint.** Your cash reconciliation ties to the EFN (if it does not, the model has an error — log it). You decide which assumptions to keep, and you decide whether to accept management's capex guidance as the base case.

---

### Phase 6 — Step 6: the valuation

**Paste first:** the brief, the approved thesis, your Phase 5 output, and the "Per-share & market" and "Normalization inputs" sheets.

> **Prompt 6**
> Continue the Tesla Inc. initiation report (brief, approved thesis, and the approved forecast below).
>
> **Ground rule:** pack figures only for reported data, with labels. Every valuation assumption must be in a table with its value and justification.
>
> **Task:** draft **Step 6 (Business valuation)**, on both routes:
> 1. **Relative:** market capitalisation, enterprise value (state the bridge, including cash and short-term investments), EV/EBITDA, and the P/E on reported EPS **and** on normalized core EPS.
> 2. **Intrinsic:** FCFF for each forecast year (EBIT × (1 − t) + D&A − CapEx − ΔWC), discounted at a stated WACC, a terminal value on stated assumptions, the enterprise-to-equity bridge, and a value per share. State the share basis you use and why.
> 3. A **WACC × terminal-growth sensitivity table**, and the percentage of enterprise value carried by the terminal value.
> 4. A **reverse DCF**: the perpetual growth rate beyond the forecast that would justify the market's enterprise value, with a sentence on whether that rate is plausible.
>
> **Rules:** present values as **ranges** tied to the assumption set; never present a single point value as "the value"; do not state or imply a price target; flag explicitly where the market price and your value diverge and what that divergence is about (assumptions, not a verdict).

**Checkpoint.** Sanity-check your own numbers before you move on: a value per share in the low tens of dollars and an enterprise value far below the market's \$1.65 trillion are the expected order of magnitude for a three-year DCF on Tesla's FY2025 economics — if your output is an order of magnitude away from that, find the error before you go further (it is usually the terminal value or the discount factor). You decide whether to present a range or a point-with-range, and you write the sentence that prevents a reader from treating your number as a target.

---

### Phase 7 — Step 7 and assembly

**Paste first:** the brief, your approved thesis, and the approved outputs of phases 2–6.

> **Prompt 7**
> Continue the Tesla Inc. initiation report (brief, approved thesis, and the approved sections below).
>
> **Ground rule:** pack labels on every figure; no price target anywhere in the output.
>
> **Task:**
> 1. Draft **Step 7 (Closing remarks and recommendation)**: an explicit recommendation with the two or three risks that would invalidate it, and the monitoring items a committee should track.
> 2. Draft the **executive summary** (max 250 words): thesis, four to six supporting figures with labels, the recommendation, and the principal risk and catalyst. It must be readable on its own.
> 3. Produce a **section list** for the whole report: section, what it proves, and the pack labels it cites.
>
> **Rules:** the executive summary may not contain a claim that appears nowhere in the body; no new figures may appear in the executive summary that are not already in the body; no price target.

**Checkpoint.** You assemble the report yourself in Word (paste section by section), then check it against the **pre-submission checklist** in [[M8-Obj-8-1]] §IV — line by line, not from memory.

---

### Phase 8 — The audit (the pivot of the project)

Run this **after** the report is assembled, and keep the model away from the document while you do it (paste the report into the chat; do not let it edit your file).

> **Prompt 8 — AUDIT**
> You are auditing a finished analyst report on Tesla Inc. You are adversarial. Your job is to find errors, not to praise.
>
> **Inputs:** the attached Tesla Capstone Data Pack and the report text below.
>
> **Task:**
> 1. Extract **every** number and every factual claim from the report into a table: claim | value in report | pack label or source the report cites | the pack value | match? | note.
> 2. Recompute every derived number in the report from the pack — ratios, the Du Pont product, the cash reconciliation, the EFN, the terminal value, the per-share value. Show your own formula and result next to the report's. Flag every mismatch.
> 3. List any figure with **no** pack label or source, any arithmetic that does not reconcile, any statement that goes beyond what the filing supports, and any place the report implies a price target.
> 4. Rank the findings by materiality: which single error would most change a reader's conclusion?
>
> **Rules:** be exhaustive and literal; do not fix anything, do not rewrite, do not soften. Report only what you can point to.

**Checkpoint.** Every flagged item goes on your **AI error log** with its type (grounding / arithmetic / fabrication / misreading / instruction), how you caught it, and the correction you made. Items you cannot resolve get cut from the report, and you say so.

---

### Phase 9 — Red team your own report, then write the adapted pack

**Paste first:** the brief, your final report, and your "Facts & risk inputs" sheet.

> **Prompt 9 — RED TEAM**
> You are a skeptical reviewer (a credit committee member for a lender; a portfolio manager for an investor) reading the analyst's own report on Tesla Inc. below.
>
> **Task:**
> 1. Identify the **three weakest claims** in the report, quoting the sentence, and say precisely why each is weak (unsupported? under-evidenced? wrong audience? hidden assumption?).
> 2. Name the **one risk the report does not mention** that a reader of the facts sheet would expect it to mention.
> 3. Name the **one number most likely to be wrong**, and say how you would test it.
> 4. State what a reader should do differently after reading this report than before.
>
> **Rules:** be specific and quote; no compliments; no summary of the report.

**Then the adapted pack.** Separate prompts, run after you have fixed what the red team found:

> **Prompt 9a — CREDIT MEMO**
> Recast the report below as a **credit memo** to a lender deciding whether to approve a **$2.0 billion revolving credit facility** for Tesla Inc. Use only the evidence in the report and the pack.
> **Requirements:** lead with liquidity, coverage, payback and downside — not revenue growth; compute net debt, quick ratio, cash-flow liquidity ratio, EBIT interest coverage, debt-to-CFO payback and debt-to-capital with the labels shown; recommend approval, decline or reprice, with the price basis and one covenant condition; if you set a covenant on EBIT, say whether it is measured on reported or normalized EBIT and why; **no price target, no equity optionality, no investment rating**. Two sentences of recommendation.
>
> **Prompt 9b — EQUITY THESIS**
> Recast the report below as an **equity research thesis** for an institutional investor on Tesla Inc.
> **Requirements:** lead with forward cash flow, returns and the valuation range with its assumption set; state FCF and normalized operating income (credits removed); give the P/E on reported and on core EPS, and what the market price implies that your model does not; give a rating (buy / hold / sell) with the single condition that would change it; **no credit recommendation, no facility terms**. Two sentences of thesis.
>
> **Prompt 9c — CHANGE LOG**
> Compare the initiation report with the credit memo and the equity thesis. Produce a table: element changed | what changed | why it serves that audience | which underlying numbers are unchanged. Flag any place where a **number** changed between documents — that is a defect to report, not a tailoring choice.

**Checkpoint.** You have a change log with reasons; the two adapted documents do not contradict each other; and you have answered the red team's three weakest claims in writing (in a short "Response to review" note at the end of the report).

---

## 5. Grading

| Criterion | Points | Full credit looks like |
|---|---:|---|
| Verification quality | 30 | Every figure and factual claim logged with source, method, result; spot-checks reproduce; nothing unresolved |
| AI error diagnosis | 15 | Errors named, classified, explained, corrected — including any that would have changed a conclusion |
| Analytical judgment | 20 | Causal thesis; the four judgments are yours, with reasons; risk has a mechanism; recommendation is falsifiable |
| Report structure & communication | 15 | Seven steps in argument order; each discharges its proof obligation; executive summary stands alone |
| Audience fit | 10 | Framing and decision type change; evidence stays invariant; the two documents do not import each other's conclusions |
| Prompt engineering | 10 | Grounded, chained, working-demanding, self-checking prompts; versioned log with rationale |
| Ethics & disclosure | 5 | Honest disclosure; limitations acknowledged; no price target |

**Integrity rules.** (1) You may not submit AI output you have not verified; (2) you must submit the prompt log, the verification log and the AI error log; (3) you must not present a price target as a recommendation; (4) you must disclose which sections are AI-drafted; (5) plagiarism includes submitting a report whose numbers do not match the student's own data pack — the instructor re-verifies a random 10% of your log rows.

---

## 6. Schedule

| Week | Phases | Deliverable at the end of the week |
|---|---|---|
| 1 | 0–1 | Brief (1 page) + thesis memo with the five claims and the lead fact |
| 2 | 2–4 | Steps 1–4 drafted; first verification pass; error log started |
| 3 | 5–7 | Forecast, valuation, recommendation, executive summary; report assembled |
| 4 | 8–9 | Audit, red team, repairs, adapted pack, change log, disclosure, reflection |

---

## 7. Copilot failure modes and the fix

| Symptom | Cause | Fix prompt line to add |
|---|---|---|
| Tesla numbers that are wrong, stale, or invented | model answering from memory | "Use only the attached pack; print the pack label for every figure; write `[NEEDED: …]` if a figure is missing." |
| A table with 12 columns and unreadable cells | too much context in one request | "Output one metric per row, max 6 columns. Do not repeat the inputs." |
| Confident prose with no numbers | model wrote a summary, not analysis | "Every claim must contain a figure and its label, or it must be deleted." |
| The model adds a price target | model's own finance priors | "Do not state or imply a price target; the report presents a value range with its assumption set." |
| It refuses to use the pack | too many attachments | "Read only the sheet I pasted below; ignore any other context." |
| Numbers that do not reconcile | arithmetic drift over long outputs | Add the self-check line: "Recompute each result by a second route and print only mismatches." |
| Plausible but wrong industry claims | model blending training data with 2025 facts | "For any external fact, cite the source and access date, and state the year it refers to." |
| It rewrites your whole draft | "make it better" is too loose | "Change only the sentences I list; leave every figure and label untouched." |
| It answers the wrong question | instructions buried in a long prompt | One question per prompt; state it in the first line; put constraints last. |

---

## 8. Sources the AI may use

**Company figures (authoritative: the pack, then the filing).** SEC EDGAR — Tesla CIK 0001318605, FY2025 10-K accession `0001628280-26-003952`: `https://www.sec.gov/cgi-bin/browse-edgar?action=getcompany&CIK=0001318605&type=10-K` · machine-readable XBRL facts: `https://data.sec.gov/api/xbrl/companyfacts/CIK0001318605.json` · local copies: `materials/raw/tsla-20251231.html`, `tsla-20231231.html`

**Market data (price, share count, estimates).** Yahoo Finance TSLA · Stooq daily CSV (`stooq.com/q/d/l/?s=tsla.us&i=d`) · Nasdaq quote page — always record source and access date.

**Industry and macro (Steps 1–2 only).** IEA Global EV Outlook · EIA · BLS · Census · FRED · Damodaran (NYU Stern).

**Never cite:** Wikipedia, investing.com, Motley Fool, Seeking Alpha, retail-broker commentary, or the model's own memory of Tesla.

---

### Related notes

- [[M8-Obj-8-1]] — the seven-step architecture, the proof obligations, and the pre-submission checklist used in phase 7
- [[M8-Obj-8-2]] — the stakeholder map, the credit memo and equity thesis specifications used in phase 9, and the capstone evidence standards
- [[M7-Obj-7-1]] — the forecast mechanics behind phase 5 (percentage-of-sales, EFN, cash reconciliation)
- [[M7-Obj-7-2]] — the stress method and switch-point analysis behind phase 5
- [[M7-Obj-7-3]] — the valuation methods, the reverse DCF, and the "never present a price target" rule used in phase 6
- [[M5-Obj-5-3]] — the normalization discipline behind phase 3
- [[M6-Obj-6-1]] — the risk diagnostics behind phase 4

---

> [!info] Sources for this project brief
> Grounded in Tesla's FY2025 Form 10-K (accession `0001628280-26-003952`) and the verified course layers ([[M2-Obj-2-1]], [[M3-Obj-3-3]], [[M5-Obj-5-3]], [[M6-Obj-6-1]], [[M7-Obj-7-3]]). Grading rubric, artifact definitions, and the audit protocol are course-specific. Copilot feature behaviour (file upload, web grounding, chat surfaces) is described as of the 2025–26 Microsoft 365 Copilot release available to enrolled students; if your client differs, use the nearest equivalent and note it in the prompt log.
