# Robo-Advisor Market Entry Model

An Excel model of the 2023-2033 U.S. robo-advisor retirement market and the economics of a firm's hypothetical entry: IRA contributions, assets under management (AUM), management fees, and the firm's payback period, NPV and IRR.

I built it in December 2024 for a firm's Corporate Strategy & Development interview case study, and updated it in October 2026 (see [2026 updates](#2026-updates)).

> Independent work sample. Not affiliated with or endorsed by the firm. Outputs reflect the case prompt's assumptions and my own, not the firm's data or a forecast.

## The question

Should the firm expand its individual retail retirement investor platform by launching a robo-advisory account product?

## Workbook tabs

| Tab | What it does |
|---|---|
| Overview | Case brief, tab guide, and the 2026 change log with before/after outputs |
| Case Study Answers | Written answers to the case prompt (December 2024 submission) |
| Module 1 | IRA contributions by age group, withdrawals, robo-advisor market size, AUM and fee revenue |
| Module 2 | firm revenue, costs, net income, payback, NPV and IRR |
| Assumptions | Case prompt background and key assumptions |
| Chart | Robo-advisor AUM and market by year |

## Results

| | Original (Dec 2024) | Corrections only | Updated (2026) |
|---|---|---|---|
| 2033 robo-advisor AUM | $1.59T | $1.59T | $2.25T |
| Fee market, 2023-2033 | $33.3B | $33.4B | $42.3B |
| Firm payback year | 2032 | 2032 | 2031 |
| Firm NPV (3% discount rate) | $136.6M | $140.6M | $491.1M |
| Firm IRR | not calculated | 6.7% | 13.6% |

"Corrections only" applies the 2026 fixes with the two new inputs set to 0%.

### Sensitivity to the new inputs

| Contribution growth | Market appreciation | 2033 AUM | NPV | IRR |
|---|---|---|---|---|
| 0% | 0% | $1.59T | $140.6M | 6.7% |
| 1% | 0% | $1.68T | $178.5M | 7.5% |
| 0% | 5% | $2.15T | $449.1M | 12.9% |
| 1% | 3% | $2.00T | $354.8M | 11.2% |
| 1% | 5% (default) | $2.25T | $491.1M | 13.6% |

The case prompt asks for market appreciation but gives no rate, so both defaults are my assumptions. Appreciation drives most of the change.

## How to use

1. Download the .xlsx. GitHub can't preview or recalculate Excel files.
2. Open it in Excel and enable editing.
3. Change inputs with the dropdowns: Module 1 C27 (contribution growth), C28 (market appreciation) and C26 (16-25 bracket share), and Module 2 R5 (initial investment), R9 (inflation) and R10 (discount rate).
4. Set C27 and C28 to 0% to see the corrections-only case.

The Assumptions tab holds the case prompt's inputs.

## 2026 updates

Made with Claude (an AI assistant by Anthropic) and logged in full on the Overview tab.

- **Added:** contribution growth and market appreciation inputs (Module 1 C27 and C28).
- **Corrected:** Module 2 net income included the market-share % row.
- **Corrected:** labor force growth wasn't applied to contribution dollars.
- **Corrected:** labor force growth for 2030-2033 used the 2026-2028 rate (+1.0%) instead of -0.5%.
- **Corrected:** the Chart tab's fee row was pasted values and is now linked to Module 1.
- **Added:** IRR and an NPV with the investment at the start (Module 2 C19:C20).

## Limitations

- The 4% rule (Module 1 row 45) is applied to annual IRA contributions, not accumulated balances.
- Fees are charged on ending AUM rather than average AUM.
- Operating costs are fixed plus inflation, with no taxes or terminal value.
- Some inputs have no source (listed on the Overview tab).
- The written answers on the Case Study Answers tab quote the original model's numbers.

## Repository layout

- `Robo_Advisor_Case_Study.xlsx`
- `README.md`

## About

Uyi Uwadiae · [Portfolio](https://uyiuwadiae.wordpress.com) · [LinkedIn](https://www.linkedin.com/in/uyiuwadiae/) · [Substack](https://uyiuwadiae.substack.com) · [Medium](https://uyi-uwadiae.medium.com)
