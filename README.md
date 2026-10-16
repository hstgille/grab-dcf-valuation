# Grab Holdings (GRAB) – DCF Valuation

A discounted cash flow model of Grab Holdings built in Excel as a personal financial project. Base case value: **$2.38 per share vs $3.07 market price (about 22% below)**.

> Educational project, not investment advice.

## Result
| | |
|---|---|
| Enterprise value | $7.5bn |
| Equity value | $9.9bn |
| Value per share | $2.38 |
| Share price (6 Oct 2026) | $3.07 |
| WACC / terminal growth | 11.6% / 2.5% |
| Terminal value as % of EV | 63% |

Across a WACC range of 10.5–12.5% and terminal growth of 1.5–3.5%, value per share ranges from $2.06 to $2.93. No combination of WACC and terminal growth reaches the current price, so the market is pricing in faster margin improvement than my base case.

## Approach
- 10-year forecast (FY26E–FY35E) of revenue by segment (Deliveries, Mobility, Financial Services), with growth fading to 5% and operating margin (after share-based compensation) rising from 4% to 15%.
- Free cash flow = operating profit – tax + D&A – capex – working capital.
- WACC via CAPM: bottom-up beta (Damodaran), plus a revenue-weighted country risk premium for Southeast Asia.
- Terminal value by Gordon growth. Equity bridge deducts customer deposits, debt (incl. convertible notes) and non-controlling interests.

## Workbook structure
Summary → Historicals → Forecast → WACC → DCF → Sensitivity

(colour code: blue = typed input, black = formula, green = link to another tab)

## Key judgement calls
- Share-based compensation is treated as a real cost, so my figures sit below Grab's adjusted EBITDA guidance.
- Forecast is deliberately cautious: FY26E revenue $4.11bn vs guidance of $4.10–4.15bn, but margins reach 15% only by FY35E.

## Limitations
-  FY26 cash flows are discounted as if they were a full year ahead despite it being October. Using the Jun-26 balance sheet against an October share price adds a small timing mismatch.
- The banking loan book isn't forecast or valued, although customer deposits are deducted making the result slightly conservative.
- Diluted shares are approximated by the Q2 2026 diluted weighted average (4,168m). Options, RSUs and July buybacks aren’t separately modelled.
- Tax is a flat 22% blended rate. Tax-loss carry-forwards are ignored.
- Superbank was consolidated from June 2026, so the recent history isn’t like-for-like.
- The beta is a bottom-up industry figure, not Grab’s own regression beta.
- Cost of debt uses a risk-free-plus-2% credit spread. Grab’s credit rating wasn’t checked.



## Sources
- Grab Holdings Form 20-F for FY2024 and FY2025 (historical financials, segment revenue, share counts, debt note).
- Grab quarterly earnings press releases: Q3 2025, Q4 2025, Q1 2026, Q2 2026 (LTM figures, Jun-26 balance sheet, guidance).
- Damodaran (NYU Stern), January 2026 data: equity risk premium, country risk premiums, industry betas.
- US Treasury 10-year yield, 5 Oct 2026 (FRED / Federal Reserve H.15).
- Grab share price (GRAB), closing price on 6 Oct 2026.
