---
title: M3-Obj-3-2 - Horizontal Analysis (Trend Analysis)
created: 2026-08-25
date: 2026-08-25
tags:
  - FSA
  - M3
  - Objective-3-2
  - Horizontal-Analysis
aliases:
  - horizontal-analysis
  - trend-analysis
---

# Learning Objective 3.2

## Implement Horizontal Analysis (Trend Analysis) to evaluate financial trajectories and establish operational velocity

---

## Instructional Summary

> [!info] Running Example: Tesla, Inc.
> We continue the Tesla running example across fiscal years 2022–2025. December 31, 2022 balances serve as opening values for computing averages; FY2023 serves as the index base year (100). All figures in millions of USD.
>
> **Opening balances (Dec 31, 2022)**: Total assets \$82,338 · AR \$2,952 · Inventory \$12,839 · PP&E \$23,548 · AP \$15,255

| Line Item | 2023 | 2024 | 2025 |
|-----------|-----:|-----:|-----:|
| **Total Revenues** | **\$96,773** | **\$97,690** | **\$94,827** |
| Cost of revenues | \$79,113 | \$80,240 | \$77,733 |
| **Gross Profit** | **\$17,660** | **\$17,450** | **\$17,094** |
| R&D | \$3,969 | \$4,540 | \$6,411 |
| SG&A | \$4,800 | \$5,150 | \$5,834 |
| **Operating Income** | **\$8,891** | **\$7,076** | **\$4,355** |
| **Net Income** | **\$14,974** | **\$7,153** | **\$3,855** |
| Cash Flow from Operations | \$13,256 | \$14,923 | \$14,747 |
| Capital expenditures | \$8,899 | \$11,342 | \$8,527 |
| **Total Assets** | **\$106,618** | **\$122,070** | **\$137,806** |
| Accounts receivable | \$3,508 | \$4,418 | \$4,576 |
| Inventory | \$13,626 | \$12,017 | \$12,392 |
| Property, plant & equipment, net | \$29,725 | \$35,836 | \$40,643 |
| Accounts payable | \$14,431 | \$12,474 | \$13,371 |

---

### I. Core Methodology of Horizontal (Trend) Analysis

> [!info] What Is Horizontal Analysis?
> In [[M3-Obj-3-1]], vertical analysis took a **photo** — every item measured against a single-period base, revealing internal structure at one moment. **Horizontal analysis** plays the **video**: it compares the same financial information across consecutive accounting periods, revealing the **direction**, **speed (velocity)**, and **magnitude** of financial change over time.
>
> It answers questions vertical analysis cannot: *Is this structure improving or decaying? How fast? Is the trajectory sustainable?* This makes it the foundational tool for budgets, projections, and forecasts.

Three primary techniques track history horizontally:

#### Technique 1: Comparative Dollar and Percentage Changes

$$\text{Percentage Change} = \frac{\text{Current Period Balance} - \text{Prior Period Balance}}{\text{Prior Period Balance}}$$

**Tesla's Year-over-Year Changes:**

| Item | 2024 Δ$ | 2024 Δ% | 2025 Δ$ | 2025 Δ% |
|------|--------:|--------:|--------:|--------:|
| Revenue | +\$917 | +0.9% | (\$2,863) | (2.9)% |
| Cost of revenues | +\$1,127 | +1.4% | (\$2,507) | (3.1)% |
| Gross profit | (\$210) | (1.2)% | (\$356) | (2.0)% |
| R&D | +\$571 | +14.4% | +\$1,871 | +41.2% |
| SG&A | +\$350 | +7.3% | +\$684 | +13.3% |
| Operating income | (\$1,815) | (20.4)% | (\$2,721) | (38.5)% |
| Net income | (\$7,821) | (52.2)% | (\$3,298) | (46.1)% |
| Cash flow from operations | +\$1,667 | +12.6% | (\$176) | (1.2)% |
| Total assets | +\$15,452 | +14.5% | +\$15,736 | +12.9% |
| PP&E, net | +\$6,111 | +20.6% | +\$4,807 | +13.4% |

Even at a glance, the asymmetry jumps out: revenue wobbled less than 3%, yet operating expenses surged while profits halved and halved again.

> [!warning] The Materiality Caveat
> High percentage changes in minor accounts can distract from small percentage changes in massive accounts. A 100% increase in a \$10 thousand prepaid asset (\$10K gain) matters far less than a 2% dip on a multi-billion-dollar revenue line. Always weigh percentage changes against the dollar base producing them — scan the Δ\$ column before celebrating or panicking over the Δ% column.

#### Technique 2: Index-Number Trend Analysis

Select a base year, set it to 100, and divide every subsequent year by the base:

$$\text{Index} = \frac{\text{Current Year Balance}}{\text{Base Year Balance}} \times 100$$

**Tesla Index Numbers (FY2023 = 100):**

| Item | 2023 | 2024 | 2025 | Trajectory Read |
|------|-----:|-----:|-----:|-----------------|
| Revenue | 100 | 100.9 | 98.0 | Flat |
| Cost of revenues | 100 | 101.4 | 98.3 | Tracks revenue |
| Gross profit | 100 | 98.8 | 96.8 | Slightly softer |
| R&D | 100 | 114.4 | **161.5** | Explosive divergence ↑↑ |
| SG&A | 100 | 107.3 | 121.5 | Steady creep ↑ |
| Operating income | 100 | 79.6 | **49.0** | Collapsing ↓↓ |
| Net income | 100 | 47.8 | 25.7 | Quarter of base ↓↓↓ |
| Cash flow from operations | 100 | 112.6 | **111.2** | Holding firm ✓ |
| Total assets | 100 | 114.5 | 129.3 | Growing ~30% |
| PP&E, net | 100 | 120.6 | 136.8 | Growing faster than sales |

The strategic benefit of indexing is spotting **diverging trajectories between interrelated accounts** over long horizons:

- **R&D (161.5) vs. Revenue (98.0)**: investment growing 16× faster than sales — a deliberate strategic bet on AI/robotics, funded by squeezing everything else
- **PP&E (136.8) vs. Revenue (98.0)**: the asset base outgrowing its revenue engine — capital intensity rising (consistent with the PP&E share creep found in vertical analysis)
- **Net income (25.7) vs. CFO (111.2)**: accrual profits and cash generation completely decoupled — the earnings-quality signature first flagged in [[M2-Obj-2-3]]

#### Technique 3: Compound Annual Growth Rate (CAGR)

CAGR computes the smoothed geometric annual rate needed for a beginning value to reach an ending value over $n$ years:

$$\text{CAGR} = \left( \frac{\text{Ending Value}}{\text{Beginning Value}} \right)^{\frac{1}{n}} - 1$$

Unlike YoY changes, CAGR smooths uneven paths into one level annual rate. For Tesla, 2023 → 2025 spans $n = 2$ years:

| Item | 2-Year CAGR (2023–2025) |
|------|------------------------:|
| Revenue | (1.0)% |
| R&D | **+27.1%** |
| Operating income | (30.0)% |
| Net income (reported) | (49.3)% |
| Cash flow from operations | +5.5% |
| Total assets | +13.7% |

> [!example] Worked Calculation: R&D
> $$\text{CAGR}_{R\&D} = \left( \frac{6{,}411}{3{,}969} \right)^{\frac{1}{2}} - 1 = (1.615)^{0.5} - 1 = 1.271 - 1 = 27.1\% \text{ per year}$$
>
> Tesla is compounding R&D spend at over 27% annually while revenue compounds at roughly −1%.

> [!warning] The Earnings-Quality CAGR Check
> Analysts must **strip non-operational items** from historical trends before computing a "pure" CAGR. Tesla's reported net income CAGR of −49.3% starts from a 2023 base inflated by a one-time tax benefit — the total 2023 provision was a \$5,001M *benefit*, driven chiefly by the ~\$6.5B release of the deferred-tax valuation allowance (see [[M2-Obj-2-2]]). Removing that benefit: adjusted 2023 net income ≈ \$14,974 − \$5,001 = \$9,973M, giving
> $$\text{Adjusted CAGR} = \left( \frac{3{,}855}{9{,}973} \right)^{\frac{1}{2}} - 1 = -37.8\%$$
> Still steep — but honest. A real-world parallel: IBM's reported 1999 operating income CAGR of 97% collapsed to 38% once pension investment returns were stripped out. Trend lines built on contaminated bases manufacture phantom growth (or phantom collapse).

> [!tip] Inflation-Adjusted (Real) Growth
> In inflationary environments, nominal growth can mask stagnant volume. Analysts deflate prior-year sales with price indices before computing growth rates. Example mechanic: if a company reports nominal sales up 40.9% while prices rose 5.1%, real growth is only ≈34%. For a quick sanity check on any nominal trend, ask: *how much of this growth is just price?*

---

### II. Velocity Ratios: The Operational Working Capital Cycle

Ratios become exponentially more powerful when tracked horizontally — a single year's turnover number says little; three years of it tells a story. Velocity metrics measure how fast working capital moves through the operational loop:

<div style="display:flex;flex-direction:column;align-items:center;gap:0.35rem;margin:1rem 0;text-align:center">
  <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1.6rem;font-weight:600">THE WORKING CAPITAL CYCLE</div>
  <div style="width:2px;height:1rem;background:var(--gray)"></div>
  <div style="display:flex;width:100%;align-items:center;justify-content:center;gap:0.5rem;color:var(--secondary)">
    <div style="height:2px;flex:0 0 42%;background:var(--gray)"></div>
    <div style="font-size:0.85rem">▼</div>
    <div style="height:2px;flex:0 0 42%;background:var(--gray)"></div>
  </div>
  <div style="display:flex;flex-wrap:wrap;justify-content:center;gap:2rem;width:100%">
    <div style="flex:1 1 260px;max-width:360px;text-align:center">
      <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1rem;font-weight:600">OPERATIONAL VELOCITY</div>
      <div style="width:2px;height:0.9rem;background:var(--gray);margin:0 auto"></div>
      <ul style="text-align:left;margin:0.4rem 0 0;padding-left:1.2rem">
        <li>→ Days Inventory Held (DSI)</li>
        <li>→ Days Sales Outstanding (DSO)</li>
      </ul>
    </div>
    <div style="flex:1 1 260px;max-width:360px;text-align:center">
      <div style="border:2px solid var(--secondary);border-radius:8px;padding:0.5rem 1rem;font-weight:600">FINANCIAL VELOCITY</div>
      <div style="width:2px;height:0.9rem;background:var(--gray);margin:0 auto"></div>
      <ul style="text-align:left;margin:0.4rem 0 0;padding-left:1.2rem">
        <li>→ Days Payable Outstanding (DPO)</li>
      </ul>
    </div>
  </div>
</div>

*All Tesla figures below use **average balances** — (beginning + ending) ÷ 2 — so they align with the full-year income statement flows.*

#### 1. Collection Timing: Receivables Turnover & DSO

$$\text{Receivables Turnover} = \frac{\text{Net Sales}}{\text{Average AR}} \qquad \text{DSO} = \frac{\text{Average AR}}{\text{Average Daily Sales}} = \frac{\text{Average AR}}{\text{Net Sales}/365}$$

| Metric | 2023 | 2024 | 2025 |
|--------|-----:|-----:|-----:|
| Receivables turnover | 30.0× | 24.6× | 21.1× |
| **Days Sales Outstanding (DSO)** | **12.2 days** | **14.8 days** | **17.3 days** |

**Horizontal diagnostic:** Tesla collects fast by any standard (direct-to-consumer sales mean minimal trade receivables), but the *direction* matters: DSO has stretched nearly 5 days over two years. A horizontally increasing DSO raises two possibilities — management loosening credit terms to prop up demand, or customers taking longer to pay because they are struggling. Neither is confirmed here, but the trend earns a spot on the monitoring list. (Real-world warning case: in 1994, software firm KnowledgeWare's DSO marched from 83 → 117 days across three quarters, exposing channel-loading and revenue inflation before the company's collapse.)

#### 2. Storage Timing: Inventory Turnover & DSI

$$\text{Inventory Turnover} = \frac{\text{Cost of Goods Sold}}{\text{Average Inventory}} \qquad \text{DSI} = \frac{\text{Average Inventory}}{\text{Average Daily COGS}} = \frac{\text{Average Inventory}}{\text{COGS}/365}$$

| Metric | 2023 | 2024 | 2025 |
|--------|-----:|-----:|-----:|
| Inventory turnover | 5.98× | 6.26× | 6.37× |
| **Days Inventory Held (DSI)** | **61.0 days** | **58.3 days** | **57.3 days** |

**Why COGS, not sales, in the numerator?** Inventory is carried at historical cost. Matching cost to cost avoids the price-fluctuation mismatch that inflates turnover when margin is embedded in the sales figure.

**Horizontal diagnostic:** DSI improving steadily — inventory turns over about four extra days faster than in 2023. A horizontally *rising* DSI is a classic red flag (inventory accumulating faster than sales clear it → write-downs or discounting ahead); Tesla shows the healthy inverse, confirming the favorable inventory-share signal from [[M3-Obj-3-1]]. Legitimate temporary buildups (pre-launch vehicle stock, tariff-driven pre-buying) should always be checked against footnotes before reading too much into either direction.

#### 3. Payment Timing: Payables Turnover & DPO

$$\text{Payables Turnover} = \frac{\text{Cost of Goods Sold}}{\text{Average AP}} \qquad \text{DPO} = \frac{\text{Average AP}}{\text{Average Daily COGS}} = \frac{\text{Average AP}}{\text{COGS}/365}$$

| Metric | 2023 | 2024 | 2025 |
|--------|-----:|-----:|-----:|
| Payables turnover | 5.33× | 5.96× | 6.02× |
| **Days Payables Outstanding (DPO)** | **68.5 days** | **61.2 days** | **60.7 days** |

**Horizontal diagnostic:** DPO *falling* — Tesla is paying suppliers about 8 days faster than in 2023. Recall from [[M2-Obj-2-3]] that a horizontally *rising* DPO ("stretching payables") boosts short-run CFO but signals distress and strains supplier relationships. Tesla moving the opposite direction suggests suppliers are being paid promptly — a position of strength, though it also means less free supplier financing.

#### 4. The Cash Conversion Cycle (Net Trade Cycle)

Links all three timing metrics into the net number of days capital is tied up in operations:

$$\text{CCC} = \text{DSI} + \text{DSO} - \text{DPO}$$

| Year | DSI | + DSO | − DPO | = CCC |
|------|----:|------:|------:|------:|
| 2023 | 61.0 | 12.2 | 68.5 | **4.7 days** |
| 2024 | 58.3 | 14.8 | 61.2 | **11.9 days** |
| 2025 | 57.3 | 17.3 | 60.7 | **13.9 days** |

*(Components rounded to one decimal; totals computed from unrounded values.)*

**Interpretation:** Tesla's conversion cycle remains extraordinarily short — under two weeks — meaning suppliers substantially finance its entire operating loop (DPO nearly covers DSO + DSO-side collection lag). But the *horizontal direction* has turned: +9 days in two years, driven almost entirely by slower collections (+5.1d) and faster supplier payment (−7.8d), only partly offset by leaner inventory (−3.7d). Still excellent; no longer flat. That is precisely the kind of gradual drift horizontal analysis exists to catch.

---

### III. Long-Term Asset Productivity Metrics

Velocity analysis extends beyond working capital to the long-lived asset base:

$$\text{Fixed Asset Turnover} = \frac{\text{Net Sales}}{\text{Average Net PP\&E}} \qquad \text{Total Asset Turnover} = \frac{\text{Net Sales}}{\text{Average Total Assets}}$$

| Metric | 2023 | 2024 | 2025 |
|--------|-----:|-----:|-----:|
| Fixed asset turnover | 3.63× | 2.98× | 2.48× |
| Total asset turnover | 1.02× | 0.85× | 0.73× |

**Horizontal diagnostic — over-capitalization:** Both productivity measures are falling steadily. Each dollar of PP&E now generates \$2.48 of sales versus \$3.63 two years ago. Declining fixed-asset turnover means the business is becoming more capital-intensive without proportionate revenue growth — fixed costs rise, **operating leverage** increases, and earnings become more sensitive to any downturn. This connects three threads into one story: PP&E share creep ([[M3-Obj-3-1]]) → falling asset productivity (here) → operating margin compression ([[M2-Obj-2-2]]).

---

### IV. Ratio Trend Analysis & Credit Risk

Beyond single ratios, credit analysts track ratio *patterns across business cycles*:

- **Cycle-to-cycle stability** — similar highs and lows across economic upturns and downturns — signals a stable risk profile (the classic "rating through the cycle" philosophy of agencies like S&P and Moody's)
- **Cycle-to-cycle deterioration** — successively lower highs and lower lows in margin, coverage, and debt-service ratios — flags permanent structural decay rather than a routine cyclical slump

Tesla's three-year window is too short for full cycle analysis, but the pattern question is live: are 2024–2025 margin declines cyclical softness, or the start of successively lower highs? Modern analysts treat persistent multi-period declines as structural until proven otherwise — the historical numbers alone cannot make that call.

---

### Key Terms

| Term | Definition |
|------|------------|
| **Horizontal analysis** | Comparing financial data across consecutive periods to establish direction, speed, and magnitude of change |
| **Trend analysis** | Synonym for horizontal analysis emphasizing multi-period patterns |
| **YoY change** | Dollar or percentage change versus the same period one year earlier |
| **Index-number trend** | Restating multi-year data relative to a base year set at 100 to expose diverging trajectories |
| **CAGR** | Compound Annual Growth Rate — the smoothed geometric annual rate linking beginning value to ending value over \(n\) years |
| **Velocity ratios** | Turnover/timing metrics measuring how fast working capital cycles through operations |
| **DSO** | Days Sales Outstanding — average days to collect receivables |
| **DSI** | Days Inventory Held — average days inventory sits before sale |
| **DPO** | Days Payables Outstanding — average days taken to pay suppliers |
| **Cash Conversion Cycle (CCC)** | DSI + DSO − DPO; net days capital is tied up in the operating loop |
| **Fixed asset turnover** | Sales ÷ average net PP&E; productivity of the fixed asset base |
| **Total asset turnover** | Sales ÷ average total assets; overall capital productivity |
| **Over-capitalization** | Declining asset turnover indicating rising capital intensity without proportional sales growth |
| **Real growth** | Growth adjusted for inflation, separating volume from price effects |

---

> [!danger] Red Flags — What Trend Analysis Reveals (and Where It Misleads)
> **Reveals:**
> - **Channel loading / loose credit** — DSO climbing quarter after quarter while sales stagnate (the KnowledgeWare signature)
> - **Involuntary inventory buildup** — horizontally rising DSI pointing to slow-moving or obsolete stock heading for write-downs
> - **Payables stretching** — rising DPO inflating today's CFO at suppliers' expense (see [[M2-Obj-2-3]])
> - **Over-capitalization** — persistently declining fixed-asset turnover quietly loading the P&L with fixed costs
> - **Diverging indexes** — interrelated accounts (sales vs. AR, R&D vs. revenue, NI vs. CFO) pulling apart
>
> **Misleads when:**
> - **The base year is abnormal** — one-time items (Tesla's 2023 tax benefit) contaminate every index and CAGR built on them
> - **Percentages ignore materiality** — spectacular % changes in trivial accounts
> - **Seasonality is ignored** — comparing adjacent quarters without seasonal adjustment manufactures fake trends
> - **Nominal is read as real** — inflation flatters revenue growth
>
> Rule: verify the base, weight by dollars, then trust the trajectory.

---

### Review Questions

> [!question]- 1. What fundamental question does horizontal analysis answer that vertical analysis cannot?
> Vertical analysis shows internal *structure* at a point in time (the photo). Horizontal analysis shows *trajectory*: whether that structure is improving or deteriorating, at what speed, and with what magnitude — direction, velocity, and change over time (the video).

> [!question]- 2. Tesla's index numbers show R&D at 161.5 and revenue at 98.0 (2023 = 100). What does this divergence tell an analyst?
> Investment is compounding ~16× faster than sales. Combined with operating income at 49.0, it reveals a deliberate strategic bet (AI/robotics) financed by near-term profitability — and lets the analyst frame future results as evidence for or against that bet paying off.

> [!question]- 3. Why must Cost of Goods Sold — not Net Sales — be used in the inventory turnover numerator?
> Inventory is valued at historical cost. Using COGS matches cost against cost; using sales embeds unrealized margin in the numerator and distorts turnover whenever margins differ across products or periods.

> [!question]- 4. DSO rises from 12.2 to 17.3 days over two years. List the competing explanations and what additional evidence would discriminate between them.
> Explanations: (a) looser credit terms to sustain demand, (b) customers financially strained and paying slower, (c) mix shift toward longer-payment channels/fleet buyers. Discriminating evidence: stated credit terms vs. actual DSO, bad-debt provision trends, revenue growth by channel, aging schedule, and whether competitors' DSO moved similarly (industry-wide vs. company-specific).

> [!question]- 5. Tesla's CCC lengthened from 4.7 to 13.9 days yet remains exceptionally healthy. What drove the increase, and why is the *direction* still worth flagging?
> Drivers: DSO +5.1 days (slower collection), DPO −7.8 days (faster supplier payment), partially offset by DSI −3.7 days (leaner inventory). Direction matters because horizontal analysis exists to catch gradual drift early — a still-good number moving steadily worse is an early warning, not a crisis.

> [!question]- 6. Reported net income CAGR (−49.3%) vs. adjusted (−37.8%): what was adjusted, why, and what real-world case does this mirror?
> The 2023 base was reduced by the one-time tax benefit (\$5,001M, chiefly the \$6.5B valuation-allowance release), because CAGR built on an abnormal base manufactures a phantom trajectory. This mirrors IBM, whose reported 1999 operating income CAGR of 97% fell to 38% after stripping pension investment returns.

---

### Practice Activity

Using Tesla's 2024 data below, compute the velocity metrics:

| Input | Value |
|-------|------:|
| Average accounts receivable | \$3,963M |
| Average inventory | \$12,821.5M |
| Average accounts payable | \$13,452.5M |
| Net sales (2024) | \$97,690M |
| COGS (2024) | \$80,240M |

1. DSO
2. DSI
3. DPO
4. Cash Conversion Cycle

> [!success]- Check Your Answers
> Daily sales = 97,690 ÷ 365 = \$267.6M/day; daily COGS = 80,240 ÷ 365 = \$219.8M/day
>
> 1. DSO = 3,963 ÷ 267.6 = **14.8 days**
> 2. DSI = 12,821.5 ÷ 219.8 = **58.3 days**
> 3. DPO = 13,452.5 ÷ 219.8 = **61.2 days**
> 4. CCC = 58.3 + 14.8 − 61.2 = **11.9 days**
>
> Your figures should match the 2024 column in the velocity tables above. Master the mechanic, then practice the harder skill: writing the one-sentence *interpretation* for each number.

---

### Related Notes

- [[M3-Obj-3-1]] — Vertical analysis: the structural snapshot these trends move through
- [[M2-Obj-2-3]] — CFO source and the payables-stretch alert referenced above
- [[M2-Obj-2-2]] — Income statement behind the margin trajectories
- [[M3-Overview]] — Module roadmap
- [[M3-Obj-3-3]] — Next: Du Pont synthesis ties margins and turnover into ROE
