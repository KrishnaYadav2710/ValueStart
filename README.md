ValueStart

ValueStart is a web-based business valuation platform designed to
convert historical financial data and user-defined assumptions into an
indicative business valuation.

The application combines a three-year financial forecast, Discounted
Cash Flow (DCF) analysis, market multiples, sensitivity analysis, trend
visualization, and data-driven financial diagnostics.

Features

• Professional animated landing page
• Company and valuation information input
• CSV financial data upload
• Manual financial data entry
• Three-year financial forecasting
• Discounted Cash Flow (DCF) valuation
• EV/Revenue valuation
• EV/EBITDA valuation
• Historical and forecast trend chart
• DCF sensitivity heatmap
• Low / Base / High valuation analysis
• Data-driven financial observations
• Professional valuation report
• Print / Save as PDF functionality
• Responsive interface
• Reserved payment section for future payment-gateway integration

Valuation Workflow

Company Information -> Historical Financials -> CSV Upload / Manual
Entry -> Forecast Assumptions -> Comparable Multiples -> Valuation
Analysis -> Trend Chart & DCF Heatmap -> Data-Driven Diagnostics ->
Professional Report

CSV Upload Format

The CSV must contain these columns:

period,revenue,ebitda,depreciation_amortization,capex,working_capital,cash,debt
previous_year_2,120,13.2,3.0,5.5,18.0,9.0,12.0
previous_year_1,138,16.6,3.4,6.2,20.0,11.0,10.0
current_year,160,21.6,4.0,7.0,23.0,14.0,8.0

Period Definitions

CSV Value           Meaning                         Chart Label

────────

previous_year_2     Two years before Current Year   PY2
previous_year_1     One year before Current Year    PY1
current_year        Current financial year          CY
Forecast Year 1     First projected year            FY1
Forecast Year 2     Second projected year           FY2
Forecast Year 3     Third projected year            FY3

Do not change the CSV column names or period identifiers because
ValueStart uses them to identify and import financial data.

Financial Fields

Historical data includes Revenue, EBITDA, Depreciation & Amortization,
Capital Expenditure, Working Capital, Cash, and Debt.

Financial values are interpreted according to the currency and reporting
unit selected by the user.

Forecast Model

ValueStart creates a three-year forecast using Revenue Growth, EBITDA
Margin, Tax Rate, D&A / Revenue, CapEx / Revenue, and Working Capital /
Incremental Revenue.

Forecast periods are displayed as FY1, FY2, and FY3.

DCF Methodology

ValueStart estimates Free Cash Flow to Firm (FCFF) broadly as:

FCFF = NOPAT + D&A - CapEx - Change in Working Capital

Forecast FCFF is discounted using the user-defined WACC.

The perpetual-growth terminal value is:

Terminal Value = FCFF(FY3) x (1 + g) / (WACC - g)

The model requires WACC to be greater than the terminal growth rate.

Cash and debt are then used to bridge from enterprise value to
indicative equity value.

Market Multiples

ValueStart supports EV / Revenue and EV / EBITDA. Users can enter Low,
Base, and High comparable multiples. An optional comparable source and
source date can be entered.

Trend Analysis

The trend chart displays Revenue and EBITDA across:

PY2 -> PY1 -> CY -> FY1 -> FY2 -> FY3

A divider separates historical periods from forecast periods.

DCF Sensitivity Heatmap

The heatmap shows how DCF equity value changes under different
combinations of WACC and terminal growth rate. The base case is
highlighted.

Data-Driven Diagnostics

ValueStart generates observations from the actual financial data and
valuation assumptions, including historical revenue growth, forecast
growth trajectory, EBITDA margin movement, DCF assumptions, and
valuation-method dispersion.

These observations are analytical diagnostics and are not investment
recommendations.

Professional Report

The report includes an executive summary, company profile, historical
financials, three-year forecast, DCF valuation, market-multiple
valuation, valuation-method comparison, data-driven observations,
methodology, and limitations.

The report is currently available free through the browser’s Print /
Save as PDF functionality.

Payment Integration

The current version provides report access for free. A payment section
is reserved for future payment-gateway integration.

For production use, report access should only be unlocked after
successful server-side payment verification.

Running ValueStart

Open index.html in a modern web browser.

The project can be deployed using GitHub Pages, Netlify, Vercel, or
another static hosting provider.

Disclaimer

ValueStart produces indicative analytical valuations based on
user-supplied financial information and assumptions.

The results are not a certified valuation, fairness opinion, investment
recommendation, tax opinion, or financial advice.

Valuation results can change materially depending on forecast
assumptions, discount rates, terminal-growth assumptions,
comparable-company selection, and the quality of the underlying
financial information.

Independent professional review may be appropriate before using the
output for transactions, fundraising, statutory filings, taxation,
investment decisions, or other regulated purposes.

Project

ValueStart - Professional Valuation Studio
