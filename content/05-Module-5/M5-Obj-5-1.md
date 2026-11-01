---
title: M5-Obj-5-1 - Detecting Aggressive Revenue and Expense Recognition
created: 2026-10-16
date: 2026-10-16
tags:
  - FSA
  - M5
  - Objective-5-1
  - Earnings-Management
aliases:
  - aggressive-recognition
  - revenue-recognition-abuse
  - expense-capitalization
---

# Learning Objective 5.1

## Detect Aggressive Revenue and Expense Recognition Techniques

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc. — and the Detective's First Tool
> Module 4 closed the *context* gap: we know where a company competes and whom to compare it against. Module 5 turns inward and begins from a blunt premise — **reported net income is an accounting estimate, not an economic fact.** Management chooses the estimates, allocations, and transaction timing behind every accrual; those choices can move earnings by billions without changing the underlying business.
>
> This objective builds the detective's first tool: line-item tests for **aggressive revenue and expense recognition**. The running company remains **Tesla, Inc.** (FY2025 Form 10-K). Because Tesla is a comparatively clean reporter, each technique is introduced through the classic abuse cases compiled in the course reference (Fridson & Alvarez), then stress-tested against Tesla's own disclosures.

Two families of manipulation, one motive — to make reported performance look better than economic reality:

| Family | What it moves | Typical mechanisms |
|---|---|---|
| **Revenue recognition abuse** | Sales *into the present* from the future | Channel stuffing, side agreements/returns, bill-and-hold, premature booking |
| **Expense recognition distortion** | Costs *out of the present* into the future | Capitalizing operating outlays, extending useful lives, hiding gains in operating lines, pension-return integration |

> [!tip] The Module 5 Arc Begins Here
> 5.1 invalidates the **income statement**. 5.2 asks whether **cash** confirms or contradicts it. 5.3 asks whether what survives is **sustainable** — separating accounting discretion and pro forma packaging from core earnings. Together the three objectives form the tests of [[M5-Obj-5-3]]'s framework: is the number **real**, **cash-backed**, and **sustainable**? Each builds on the last — a claim you cannot test at the accrual level will surface at the cash-flow level instead.

---

### I. Accrual Discretion: Where the Latitude Lives

Accrual accounting rests on two principles:

1. **Revenue recognition** — revenue is recorded when the seller satisfies its performance obligation and control of the good or service transfers to the buyer (ASC 606; see [[M2-Obj-2-2]]).
2. **Expense matching** — costs incurred to generate revenue are recognized in the *same period* as that revenue.

Neither principle is mechanical. Both depend on **estimates** (how long is a useful life? how large a warranty reserve?), **allocations** (how much of a bundled price belongs to the car versus the software?), and **timing** (when exactly did control transfer?). That judgment space is where earnings management lives.

And the incentives are real: executives are judged against quarterly consensus estimates and paid on performance metrics. When a gap opens between economic reality and the target, the pressure is to close it through accounting choice rather than operations.

<div style="display:flex;flex-direction:column;align-items:center;gap:0.5rem;margin:1rem 0">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.4rem;font-weight:600">EARNINGS-MANAGEMENT DISCRETION</div>
  <div style="display:flex;width:100%;align-items:center;justify-content:center;gap:0.5rem;color:var(--secondary)">
    <div style="height:2px;flex:0 0 33%;background:var(--gray)"></div>
    <div style="font-size:0.85rem">&#9660;</div>
    <div style="height:2px;flex:0 0 33%;background:var(--gray)"></div>
  </div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;gap:1.5rem;width:100%">
    <div style="flex:1 1 260px;max-width:440px;text-align:center">
      <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1rem;font-weight:600">REVENUE RECOGNITION</div>
      <div style="width:2px;height:0.9rem;background:var(--gray);margin:0 auto"></div>
      <ul style="text-align:left;margin:0.4rem 0 0;padding-left:1.2rem">
        <li>&rarr; Channel stuffing &amp; distribution loading</li>
        <li>&rarr; Side agreements / return contingencies</li>
        <li>&rarr; Bill-and-hold &amp; premature booking</li>
        <li>&rarr; Unbilled receivables (DSO divergence)</li>
      </ul>
    </div>
    <div style="flex:1 1 260px;max-width:440px;text-align:center">
      <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1rem;font-weight:600">EXPENSE RECOGNITION</div>
      <div style="width:2px;height:0.9rem;background:var(--gray);margin:0 auto"></div>
      <ul style="text-align:left;margin:0.4rem 0 0;padding-left:1.2rem">
        <li>&rarr; Capitalizing operating outlays</li>
        <li>&rarr; Useful-life &amp; salvage extension</li>
        <li>&rarr; Nonoperating gains inside SG&amp;A</li>
        <li>&rarr; Pension-return integration</li>
      </ul>
    </div>
  </div>
</div>

> [!warning] "Aggressive" Is Not Always "Illegal"
> Most techniques below sit within GAAP. The analyst's job is not to find fraud on every page; it is to separate **earnings that reflect the business** from **earnings that reflect a reporting choice** — and to price the difference.

---

### II. Revenue-Recognition Abuses and Their Red Flags

#### 1. Channel Stuffing and Distribution Loading

**Mechanism.** Inducing wholesalers or dealers to accept more inventory than end-customers will absorb — through deep period-end discounts, extended payment terms, or informal promises to take goods back.

**Impact.** Future sales are pulled into the present. Because real demand has not grown, the following period's revenue collapses as the channel works off the glut — a "borrowed" quarter repaid with interest.

**Classic cases (from Fridson & Alvarez book).** *Bausch & Lomb* gave distributors undisclosed side agreements promising payment was not due until the lenses sold through to consumers. *Sunbeam* paid distributors roughly 1% per month to store unneeded product in rented warehouses — revenue recognized with no genuine sale.

#### 2. Side Agreements and Return Contingencies

**Mechanism.** Executing a formal sales contract while quietly granting verbal or undisclosed written terms that remove the customer's obligation to pay.

**Impact.** A conditional shipment that should not yet be revenue becomes an immediate top-line entry — a direct violation of the "control transferred" test.

**Classic case.** *Informix* overstated revenue by roughly **\$244 million** across three years by granting resellers undisclosed agreements permitting returns, stretching payment terms beyond 90 days, and guaranteeing funding.

#### 3. Premature Booking, Bill-and-Hold, and Unbilled Receivables

**Mechanism.** Recording sales before shipment, treating non-binding letters of intent as firm orders, or invoicing work before it is performed.

**The diagnostic — revenue vs. receivable divergence.** When receivables grow much faster than sales, or **Days Sales Outstanding (DSO)** surges, revenue is being recognized before cash collection is reasonably assured. This is the single most reliable quantitative tell for premature recognition.

**Classic case (Fridson & Alvarez).** *KnowledgeWare*'s sales fell 15.5% in Q1 1994 while receivables kept rising: DSO marched from **83 → 98 → 100 → 117 days** before a roughly \$19 million restatement erased previously reported profits.

> [!danger] The Revenue Red-Flag Test
> Compute the growth rates side by side: **net sales vs. accounts receivable**, and the **DSO trend**. A widening gap is the fingerprint of recognized-but-uncollected revenue — channel loading, bill-and-hold, or a deteriorating customer base. (This is the horizontal-analysis detector introduced in [[M3-Obj-3-2]].)

---

### III. Expense-Recognition and Cost Manipulation

#### 1. Capitalization of Operating Outlays

**Mechanism.** Reclassifying routine, recurring operating costs (marketing, customer acquisition, line-access fees) as long-lived assets rather than current expenses.

**The double distortion.** (i) *Income statement* — current profit is inflated because the cost is amortized over future periods. (ii) *Cash-flow statement* — **operating cash flow is inflated** because the cash outlay is pushed into investing as "capital expenditure."

**Classic case.** *America Online* capitalized roughly **\$385 million** of direct-mail subscriber-acquisition costs as an asset, reporting artificial profits until the SEC forced a single write-off.

<div style="display:flex;flex-direction:column;align-items:center;gap:0.5rem;margin:1rem 0">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.4rem;font-weight:600">CAPITALIZING AN OPERATING COST &mdash; THE DOUBLE DISTORTION</div>
  <div style="display:flex;width:100%;align-items:center;justify-content:center;gap:0.5rem;color:var(--secondary)">
    <div style="height:2px;flex:0 0 33%;background:var(--gray)"></div>
    <div style="font-size:0.85rem">&#9660;</div>
    <div style="height:2px;flex:0 0 33%;background:var(--gray)"></div>
  </div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;gap:1.5rem;width:100%">
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 1rem;flex:1 1 240px;max-width:400px;text-align:center"><b>Income statement</b><br/><span style="font-size:0.9em">cost amortized over future periods<br/><b>&rarr; current profit overstated</b></span></div>
    <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.6rem 1rem;flex:1 1 240px;max-width:400px;text-align:center"><b>Cash-flow statement</b><br/><span style="font-size:0.9em">outlay reclassified as investing (CapEx)<br/><b>&rarr; operating cash flow overstated</b></span></div>
  </div>
</div>

#### 2. Depreciation and Useful-Life Extensions

**Mechanism.** Lengthening the estimated useful life (or raising salvage value) of PP&E. Annual depreciation falls; earnings rise — with no change to cash flows or taxes.

$$\text{Depreciation Expense} = \frac{\text{Historical Cost} - \text{Salvage Value}}{\text{Useful Life}}$$

Extending the denominator lowers the annual charge and raises operating margin by pure assumption.

#### 3. Reclassifying Nonoperating Gains into Operating Lines

**Mechanism.** Recording a material, nonrecurring gain — typically an asset sale — as a *reduction of an operating expense* (often SG&A) instead of showing it below operating income.

**Classic case.** In 1999 *IBM* recorded a **\$4.057 billion** pretax gain from selling its Global Network business to AT&T as a reduction of SG&A. The move masked an *increase* in underlying SG&A (20.4% → 21.4% of revenue) and manufactured the appearance of cost discipline.

#### 4. Pension-Return Integration

**Mechanism.** Accounting rules allowed expected returns on pension-plan assets to flow through operating income, reducing COGS or SG&A. In strong bull markets these non-operational returns can dwarf core profit.

**Classic case.** In 1999 roughly **\$799 million** — about **6.7%** of IBM's reported \$11.9 billion operating income — came from pension-plan asset returns. Stripping them, IBM's "core" operating-income CAGR fell from a reported **97%** to about **38%**.

> [!danger] The Expense Red-Flag Test
> Read the notes, not just the face of the statement. Four questions catch most distortions: **(1)** Are recurring costs being capitalized? (compare CapEx growth against the operating expense it replaced.) **(2)** Have depreciation lives or salvage assumptions changed? **(3)** Is a large gain buried inside an operating expense line, or a pension return inflating operating profit? **(4)** Is a reserve — warranty, returns, buyback obligations — growing much faster than revenue? Reserves are management estimates embedded in an expense line; when the reserve compounds while the business runs flat, "smoothing" has somewhere to hide (this is the pattern in Tesla's warranty work below, in §IV).

---

### IV. Applying the Tests to Tesla (FY2025)

Tesla is a useful application precisely because it is **not** a fraud case: it lets us calibrate what a *clean* fingerprint looks like — and still find the soft spots that deserve a monitoring slot.

#### Revenue side

| Test | Tesla evidence (FY2023 → FY2025) | Read |
|---|---|---|
| Revenue vs. receivables divergence | AR net **\$3,508M → \$4,576M (+30.4%)** while revenue **\$96,773M → \$94,827M (−2.0%)** | Mild divergence — but see DSO |
| DSO | **12.2 → 17.3 days** (average balances; [[M3-Obj-3-2]]) | World-class short; the *direction* earns a monitoring slot |
| Recognition basis | Automotive sales on **delivery** (point in time); FSD/connectivity over the **expected ownership life** (stand-ready) | Low premature-recognition risk |
| Deferred revenue (FSD/connectivity) | Balance **\$3,599M → \$3,867M** (2024 → 2025) | Legitimate upfront cash; watch take-rate |

Deferred revenue related to connectivity, FSD (Supervised), free Supercharging, and over-the-air updates (\$M):

| Item | 2025 | 2024 |
|---|---:|---:|
| Beginning balance | \$3,599 | \$3,536 |
| Additions | \$1,083 | \$1,343 |
| Net changes, pre-existing (incl. FX) | \$141 | (\$92) |
| Revenue recognized | (\$956) | (\$1,188) |
| **Ending balance** | **\$3,867** | **\$3,599** |

> [!tip] Verdict — Revenue Side
> Tesla shows none of the classic revenue abuses: direct-to-consumer sales, DSO around three weeks, and point-in-time delivery recognition. The monitor-worthy items are the **+5.1-day DSO drift** and the **resale-value guarantees** (maximum exposure **\$1.45B → \$3.45B**) — a contingent liability that behaves like a put on used-car prices. Clean, but not unexamined.

#### Expense side

**Warranty reserve (embedded in COGS)** — the estimate most likely to move Tesla's gross margin (\$M):

| Accrued warranty activity | 2025 | 2024 | 2023 |
|---|---:|---:|---:|
| Beginning balance | \$6,716 | \$5,152 | \$3,505 |
| Costs incurred | (\$1,723) | (\$1,453) | (\$1,225) |
| Net changes, pre-existing (incl. FX) | \$1,127 | \$287 | \$539 |
| Provision | \$2,487 | \$2,730 | \$2,333 |
| **Ending balance** | **\$8,607** | **\$6,716** | **\$5,152** |

The reserve is up **~146%** in two years against flat revenue, with the annual provision steady at 2.4–2.8% of revenue. A growing fleet and recall activity explain much of it — but reserve estimates are exactly where "smoothing" hides.

**Depreciation policy (PP&E useful lives, FY2025 10-K):**

| Asset class | Estimated useful life |
|---|---|
| Machinery, equipment, vehicles, office furniture | 3–15 years |
| Tooling | 4–7 years |
| Buildings and improvements | 15–30 years |
| Computer equipment and software | 3–6 years |
| AI infrastructure (owned data centers) | 5–30 years |

Tesla reviews useful lives **annually**. It does **not** capitalize R&D — research costs are expensed as incurred, and even internally developed software is capitalized only after technological feasibility.

> [!warning] Verdict — Expense Side
> The two classic abuses that would be easiest to hide are absent or modest: R&D is expensed (not capitalized), and non-operating items sit *below* operating income rather than inside SG&A. The live questions are **(1)** the rapidly growing **warranty reserve**, **(2)** useful-life assumptions on new asset classes (AI infrastructure: 5–30 years), and **(3)** regulatory credits — **\$1,993M** of 100%-margin revenue equal to **~46% of FY2025 operating income** — which sit *inside* automotive revenue, not below the line ([[M2-Obj-2-2]], [[M4-Obj-4-2]]).

> [!example] The Analyst's Takeaway
> The purpose of 5.1 is not to convict — it is to **locate the judgment**. On Tesla, the judgment concentrates in three estimates: **warranty reserves, depreciation lives, and regulatory-credit revenue**. Everything else screens clean.

---

### V. Worked Calculations

#### Calculation 1: Detecting Revenue–Receivable Divergence

> [!example] Scenario — Apex Software Systems
> Apex expanded its distributor program. Quarterly filings (\$ thousands):
>
> | Metric | Q1 2024 | Q2 2024 | Q3 2024 | Q4 2024 |
> |---|---:|---:|---:|---:|
> | Net revenues | \$50,000 | \$52,000 | \$51,000 | \$48,000 |
> | Accounts receivable (end) | \$45,000 | \$54,000 | \$62,000 | \$72,000 |
>
> Use a 91-day quarter.

**Tasks.** (1) Compute DSO for each quarter. (2) Compute Q1→Q4 growth in revenue and in AR. (3) Identify the red flag and estimate the revenue restatement if Q4 DSO had held at Q1's level.

> [!success]- Solution
> **(1) DSO** = (AR ÷ quarterly revenue) × 91
> - Q1: (45,000 / 50,000) × 91 = **81.9 days**
> - Q2: (54,000 / 52,000) × 91 = **94.5 days**
> - Q3: (62,000 / 51,000) × 91 = **110.6 days**
> - Q4: (72,000 / 48,000) × 91 = **136.5 days**
>
> **(2) Growth, Q1 → Q4**
> - Revenue: (48,000 − 50,000) / 50,000 = **−4.0%**
> - AR: (72,000 − 45,000) / 45,000 = **+60.0%**
>
> **(3) Red flag and restatement**
> Revenue fell 4% while receivables rose 60% and DSO nearly doubled — the classic premature-recognition fingerprint (channel loading, bill-and-hold, or reseller credit trouble).
> - Normalized Q4 AR at 81.9 days: 48,000 × (81.9 / 91) = **\$43,200**
> - Excess AR: 72,000 − 43,200 = **\$28,800 thousand** — the potential overstated revenue.

#### Calculation 2: Capitalization and Useful-Life Manipulation

> [!example] Scenario — Vertex Logistics
> On Jan 1, 2024 Vertex bought **\$100M** of delivery equipment and spent **\$20M** on routine fleet maintenance. Management (i) **capitalized** the maintenance into PP&E and (ii) depreciated the resulting \$120M over **10 years** (straight-line, zero salvage) versus a peer benchmark of **5 years**.

**Tasks.** Compute (1) reported depreciation and total operating expense under management's approach; (2) depreciation and total expense under a conservative benchmark (maintenance expensed; 5-year life on the \$100M); (3) the resulting pre-tax income inflation.

> [!success]- Solution
> **(1) Aggressive**
> - Capitalized base = 100M + 20M = \$120M → depreciation = 120M / 10 = **\$12M**
> - Maintenance expense = **\$0** (capitalized); total IS expense = **\$12M**
>
> **(2) Conservative**
> - Depreciation = 100M / 5 = **\$20M**; maintenance expensed = **\$20M** → total = **\$40M**
>
> **(3) Inflation** = 40M − 12M = **\$28M** of pre-tax operating income created by accounting choice alone.

#### Calculation 3: Unmasking Operating-Margin Distortion

> [!example] Scenario — Global Tech Corp (FY2024)
> Revenue \$10,000,000; reported SG&A \$1,500,000; reported operating income \$2,500,000. The 10-K notes reveal (i) SG&A was reduced by a **\$500,000** pretax gain on a real-estate sale and (ii) operating income includes **\$300,000** of net pension-plan benefit.

**Tasks.** Compute (1) reported operating margin; (2) adjusted SG&A and adjusted operating income; (3) adjusted margin and the percentage-point overstatement.

> [!success]- Solution
> **(1)** 2,500,000 / 10,000,000 = **25.0%**
> **(2)** True operating SG&A = 1,500,000 + 500,000 = **\$2,000,000**; adjusted operating income = 2,500,000 − 500,000 − 300,000 = **\$1,700,000**
> **(3)** 1,700,000 / 10,000,000 = **17.0%** → overstated by **8.0 points** (≈47% of true core operating profit).

---

### Key Terms

| Term | Definition |
|------|------------|
| **Revenue recognition** | Recording revenue when the performance obligation is satisfied and control transfers (ASC 606) |
| **Matching principle** | Recognizing expenses in the same period as the revenue they helped generate |
| **Channel stuffing / loading** | Pushing excess inventory onto distributors to inflate current-period sales |
| **Side agreement** | Undisclosed terms that remove the customer's obligation to pay, making a "sale" conditional |
| **Bill-and-hold** | Booking revenue before shipment, when control has not actually transferred |
| **DSO divergence** | Receivables (or DSO) growing faster than sales — the signature of uncollected revenue |
| **Expense capitalization** | Recording recurring operating costs as assets, inflating both profit and operating cash flow |
| **Useful-life extension** | Lengthening depreciable life to lower annual depreciation and raise earnings |
| **Gain reclassification** | Hiding a nonoperating gain inside an operating expense line |
| **Pension-return integration** | Flowing expected pension-asset returns through operating income |
| **Quality of earnings** | The degree to which reported income reflects sustainable, cash-generative economic performance |

---

> [!danger] Red Flags — Aggressive Recognition
> - Receivables or DSO climbing while revenue is flat or falling
> - Large quarter-end revenue spikes followed by reversals (channel loading)
> - Recurring costs migrating from the income statement to the balance sheet (capitalization)
> - Depreciation lives or salvage values changed without an economic rationale
> - Material asset-sale gains netted inside SG&A or COGS
> - Operating income that depends on pension-asset returns or other non-core items
> - Non-GAAP "core" earnings diverging further from GAAP every year

---

### Review Questions

> [!question]- Q1: Why does accrual accounting create room for earnings management?
> Both revenue recognition and expense matching depend on estimates, allocations, and timing judgments rather than cash movements. Management controls those judgments, so reported income can be steered within GAAP — often motivated by consensus estimates and performance-based pay.

> [!question]- Q2: What is the most reliable quantitative signal of premature revenue recognition, and why?
> A widening gap between sales growth and receivables growth (i.e., rising DSO). Revenue can be booked the moment control is claimed to transfer, but cash arrives later — so recognized-but-uncollected sales surface first as ballooning receivables.

> [!question]- Q3: Explain the "double distortion" of capitalizing an operating expense.
> (1) Current profit rises because the cost is amortized over future periods instead of expensed now, and (2) operating cash flow rises because the cash outflow is reclassified from operating to investing as CapEx. Both the earnings and cash-flow pictures flatter the firm at once.

> [!question]- Q4: IBM's 1999 operating income included \$799M of pension returns. Why did that make its reported growth misleading?
> The pension return is non-operational and market-dependent, not a product of selling goods or services. Removing it dropped the reported 97% operating-income CAGR to roughly 38% — headline growth was largely a bull-market artifact, not operating improvement.

> [!question]- Q5: Tesla's DSO rose from 12.2 to 17.3 days. Does that make Tesla a channel-stuffing concern? Defend your answer.
> No. At two to three weeks, Tesla's DSO remains far below any premature-recognition threshold, and Tesla sells direct rather than through loading-prone distributors. But the *direction* — plus growing AR against falling revenue — earns a monitoring slot, because horizontal analysis exists to catch gradual drift ([[M3-Obj-3-2]]).

> [!question]- Q6: Where does the real judgment lie in Tesla's expense reporting?
> In three estimates rather than obvious abuses: the **warranty reserve** (up ~146% in two years, embedded in COGS), **depreciation lives** (especially 5–30-year AI-infrastructure assets), and **regulatory credits** (\$1,993M of 100%-margin revenue, ~46% of operating income) that sit inside automotive revenue.

---

### Practice Activity

You are testing the quality of Tesla's FY2025 reported earnings, using the tables above. Four items stand out:

- the **warranty reserve** is up ~146% in two years (provision \$2,487M; ending balance \$8,607M) while revenue is roughly flat;
- **DSO** drifted from 12.2 to 17.3 days (revenue \$94,827M; AR net \$4,576M);
- **regulatory credits** of \$1,993M — 100%-margin revenue booked inside automotive revenue — equal ~46% of operating income;
- **AI-infrastructure** assets are depreciated over a 5–30-year range.

1. Classify each item as a **revenue** or **expense** recognition issue (or neither), and name the specific estimate or mechanism at work.
2. Compute the warranty provision as a percentage of FY2025 revenue. Does the *level* or the *trend* concern an analyst more, and why?
3. Which item most threatens the **sustainability** of Tesla's operating income — and explain why it is *not* a channel-stuffing-style red flag.
4. Write the one-sentence challenge you would put to Tesla's investor-relations team for the two items most material to earnings.

---

### Related Notes

- [[M5-Overview]] — Module 5 overview
- [[M5-Obj-5-2]] — Next: is EBITDA a genuine cash-flow measure? (cash verification)
- [[M2-Obj-2-2]] — income-statement mechanics, ASC 606, and regulatory credits
- [[M2-Obj-2-3]] — cash-flow statement; the capitalization detector in §V
- [[M3-Obj-3-2]] — DSO and horizontal analysis used in the receivables test
- [[M4-Obj-4-2]] — normalization of one-off items

---

> [!info] Sources
> - Tesla, Inc. FY2025 Form 10-K (filed Jan 2026), SEC EDGAR (accession `0001628280-26-003952`) — revenue-recognition policy, warranty activity, PP&E useful lives, and deferred-revenue disclosure
> - Classic abuse cases: Fridson & Alvarez, *Financial Statement Analysis: A Practitioner's Guide* (3rd Ed), Part III, Ch. 5–11 ("A Closer Look at Profits")
> - Cross-referenced Tesla figures validated in [[M2-Obj-2-2]], [[M2-Obj-2-3]], and [[M3-Obj-3-2]]
