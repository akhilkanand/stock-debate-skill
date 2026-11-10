# Sample output: Tata Motors (TMPV + TMCV)

> **Excerpt from a `/stock-debate Tata Motors` run on 10 Nov 2026.** Trimmed to show how the skill works. Each role's buy/sell stance, the price targets and the Judge's conviction scores have been removed. Numbers were gathered by AI agents from public web sources and have not been independently verified. They will be out of date by the time you read this. **Educational illustration only, not investment advice.**

This run shows the skill handling a **demerger**. Tata Motors split in Oct 2025 into two listed companies, so the Researcher first works out the corporate structure and then tags every number with its entity. The debate then argues about each business separately.

A full run has seven turns (Researcher, Bull, Bear, two rebuttal rounds each, Judge) and comes to about 70 KB of markdown. Below are selected parts.

---

## RESEARCHER (excerpt)

Each figure is tagged with its entity:
- **TMPV**: Tata Motors Passenger Vehicles Ltd, covering India PV, EV and JLR. This is the old listed Tata Motors entity, renamed.
- **TMCV**: Tata Motors Ltd, formerly TML Commercial Vehicles Ltd. This is the commercial-vehicle business.

### Corporate structure (checked)

| Item | Fact | Source |
|---|---|---|
| Demerger effective date | 1 Oct 2025. The CV business moved into TML Commercial Vehicles Ltd. | screener.in TMCV note |
| Rename of CV company | Renamed Tata Motors Ltd on 29 Oct 2025. NSE symbol TMCV. Listed Nov 2025. | screener.in TMCV note |
| Old listed entity | Renamed Tata Motors Passenger Vehicles Ltd (NSE: TMPV). Keeps PV, EV and JLR. | screener.in TMPV |
| Iveco (TMCV) | Initial settlement of the tender offer completed 30 Oct 2026. TML CV Holdings B.V. holds about 89.42% of Iveco. | InvestyWise, citing a BSE filing, 30 Oct 2026 |

### Five-year financials: TMPV consolidated (continuing listed entity)

**Series break:** FY22–FY24 are the pre-demerger consolidated figures, including CV. FY25 and FY26 appear restated to exclude CV: FY25 revenue is ₹3,66,094 cr, below the reported pre-demerger figure of about ₹4.4 lakh cr. FY26 PAT includes a non-cash demerger gain of about ₹82,000 cr booked in Q2 FY26.

| Item (₹ cr) | FY22 | FY23 | FY24 | FY25 | FY26 |
|---|---|---|---|---|---|
| Revenue | 2,78,454 | 3,45,967 | 4,34,016 | 3,66,094 | 3,35,582 |
| EBITDA margin (OPM) | 9% | 9% | 13% | 13% | 6% |
| PAT | -11,309 | 2,690 | 31,807 | 28,149 | 82,645* |
| Operating cash flow | 14,283 | 35,388 | 67,915 | 63,102 | 13,041 |
| Free cash flow | -655 | 16,443 | 36,732 | 26,034 | -23,195 |
| Debt/Equity | 3.29 | 2.96 | 1.26 | 0.62 | 0.71 |
| ROCE | 1% | 6% | 19% | 16% | 3% |

\*Inflated by the demerger gain.

### TMCV financials (short history)

TMCV has only about a year of separate history, so the sheet shows what exists and says what doesn't:

| Item (₹ cr) | FY25 | FY26 | TTM |
|---|---|---|---|
| Revenue | 58,217 | 83,855 | 93,950 |
| EBITDA margin | 11% | 9% | 11% |
| PAT | 3,195 | 3,030 | 6,308 |
| Free cash flow | 7,005 | 12,878 | – |
| ROE / ROCE (TTM) | – | – | 34.0% / 35.9% |

- Sources disagree on FY26 revenue: ₹83,855 cr vs ₹77,400 cr. Screener labels the year "10m".
- Pre-demerger CV segment history for FY22–FY24: **not found** from verified sources.

### Valuation (9 Nov 2026 close, screener.in)

| Company | P/E (TTM) | P/B | ROE | ROCE |
|---|---|---|---|---|
| TMPV | 109 | 0.97 | 75.7%* | 2.7% |
| TMCV | 22.5 | 10.5 | 34.0% | 35.9% |
| Maruti Suzuki | 30.2 | ~3.7 | 14.3% | 18.9% |
| M&M | 20.4 | 4.18 | 20.3% | 15.1% |
| Ashok Leyland | 27.6 | 7.21 | 27.4% | 13.6% |
| Eicher Motors | 36.0 | 8.34 | 24.0% | 30.5% |

\*Distorted by the demerger gain. 5-year multiple history: **not found** as clean series. TMCV has about 12 months of listed history, and pre-demerger multiples are not comparable.

---

## How an argument develops: JLR's "recovery"

One thread, followed across four turns.

**BULL (opening):** JLR Q2 FY27 wholesale was **82.4k, up 24.5% YoY** (JLR, 3 Oct 2026). Range Rover, Range Rover Sport and Defender made up 77.6% of the mix. These are the highest-margin models.

**BEAR (opening):** That is a wholesale-versus-retail gap. **Wholesale rose 24.5% while retail fell 7% to 79.0k.** Shipments to dealers grew while sales to end customers shrank. Retail incentives (VME) jumped to 7.1% from 4.1% in Q1 FY27.

**BULL (rebuttal 1):** The retail fall is mostly a China-JV accounting gap:

| Q2 FY27 | Wholesale | Retail | Retail YoY |
|---|---|---|---|
| UK | 21.0k | 18.5k | +31% |
| North America | 27.1k | 24.8k | +8% |
| Europe | 13.2k | 12.7k | -9% |
| China | 6.1k | 6.3k | -41% |
| CJLR (China JV, in retail only) | – | 0.9k (prior year 7.4k) | -88% |

CJLR volumes never appear in wholesale. Excluding China, retail was about **72.7k vs 74.8k, roughly -3%**, not -7%.

**BEAR (rebuttal 1):** *"The Bull's ex-China retail arithmetic is correct."* But the two-year view is worse: Q2 FY25, before the cyber-attack, had **103,108 retail**. Q2 FY27 retail is **23% lower**.

**BULL (rebuttal 2):** *"My 'it's China' defence covers the one-year comparison only. It does not explain the two-year decline."* Instead: the three core models' wholesale is about **9% above the pre-cyber quarter** (63.9k vs 58.5k units).

**BEAR (rebuttal 2):** *"The two mix figures are measured the same way."* But that base quarter was itself disrupted by the Novelis aluminium force majeure. JLR's CEO cited about 30k Range Rover / Range Rover Sport units that quarter against a normal run-rate of 40k or more. Against a normal base, Q2 FY27 is still lower.

---

## JUDGE (CIO) (excerpt)

### Checking the disputed number first

**The Iveco stake is 96.29%, not 89.42%.** Autocar Pro confirms the 7 Nov 2026 filing. The fact sheet's 89.42% was the initial-period figure.

That decides the leverage dispute. At 96.29%, the cost is about ₹33,600 cr. Less ₹15,900 cr of net cash, net debt comes to about ₹17,700 cr, or about 1.65x TMCV's pre-Iveco TTM EBITDA. The Bull's 1.46x no longer holds. The Bear's 1.8x is also not the right test, because "combined EBITDA" includes Iveco, whose EBITDA is not reported. What survives is moderate leverage that is not yet measurable, not a balance-sheet threat.

### Points won

| Issue | Winner | Why |
|---|---|---|
| JLR one-year retail decline is mostly CJLR | Bull | Bear conceded: ex-China retail -2.8%, not -7% |
| JLR two-year retail erosion (ex-China about -19% vs Q2 FY25) | Bear | Bull conceded |
| Core-model "+9% vs pre-cyber" | Bear | The base quarter was Novelis-disrupted |
| Defender tariff (EU 15%, not 27.5%) | Bull | Factual correction; Bear conceded |
| TMPV valuation (0.97x P/B vs 2.7% ROCE, about -₹35,000 cr FCF over five quarters) | Bear | The Bull did not rebut the returns or the cash burn |
| India PV/EV deserves a premium multiple | Bear | Bull withdrew it after the -0.5% Q1 FY27 EBIT margin |
| India CV quality (65% auto ROCE, net cash, -89 WC days) | Bull | Bear conceded |
| TMCV "cheap vs peers" | Draw | Core P/E about 23x vs Ashok Leyland 27.6x, but Iveco consolidation and bridge interest are not in it |
| Iveco Defence perimeter / industrial net debt of €34m | Bull | Bear conceded |
| Iveco earnings trough vs structural weakness | Bear, provisional | 9M industrial EBIT €14m and FCF €(1.38)bn; Q4 decides |
| Post-deal leverage | Draw, leaning Bear | About 1.65–1.8x on TMCV EBITDA alone; combined figure not computable |
| Dilution risk | Bull | Funding reported as debt plus internal accruals, no equity (5 Nov 2026) |

### Unresolved questions

1. TMCV consolidated net debt after Iveco, and the refinancing of the 12-month bridge. Not found.
2. Iveco EBITDA and ex-Defence normalised EBIT. Not reported, so "combined EBITDA" cannot be calculated.
3. JLR Q2 FY27 VME and dealer inventory. Not found. They determine whether +24.5% wholesale against -7% retail is restocking or channel push.
4. Whether the 4% JLR FY27 EBIT guidance survives. With H1 near 3%, it needs H2 above 5%.
5. TMCV standalone other income. Not disclosed separately.

### What to watch

| Date | Event | What it tests |
|---|---|---|
| 13 Nov 2026 | TMPV Q2 FY27 results | JLR EBIT margin vs 4% guidance, VME, H2 bridge, FCF |
| Early Jan 2027 | JLR Q3 FY27 retail volumes | Whether UK and North America retail keep growing |
| Late Jan / Feb 2027 | TMCV Q3 FY27, first quarter with Iveco consolidated | Disclosed net debt vs combined EBITDA; India CV margin |
| Feb 2027 | Iveco Q4 / FY2026 results | Whether Iveco's industrial EBIT and FCF recover |
| By Oct–Nov 2027 | Bridge refinancing (12-month tenor) | Long-term debt terms vs an equity raise |

*Educational discussion, not investment advice.*
