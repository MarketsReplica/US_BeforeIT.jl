# US BeforeIT.jl Data Sources: Comprehensive Cost & Integration Analysis

## **Core Economic Structure Data**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Input-Output Tables** | 71×71 industry make/use matrices | [BEA I-O Accounts](https://www.bea.gov/industry/input-output-accounts-data) | IMPLAN ($2K), Moody's ($$$$) | Free | Medium | Excel/CSV download | Annual updates, 5-year benchmarks |
| **Sectoral Employment** | Workers by 71 industries | [BLS QCEW](https://www.bls.gov/cew/) | Haver ($$), Nasdaq Data Link ($) | Free | Easy | CSV/API | Quarterly, 6-month lag |
| **Sectoral Output** | Value added by industry | [BEA GDP-by-Industry](https://www.bea.gov/data/gdp/gdp-industry) | [BEA Economy at a Glance](https://www.bea.gov/news/glance) | Free | Easy | Excel/API | Quarterly updates |

## **National Accounts & GDP Components**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Real GDP Components** | C, I, G, X, M quarterly | [BEA NIPA Tables](https://www.bea.gov/data/gdp/gross-domestic-product) | [Atlanta Fed GDPNow](https://www.atlantafed.org/cqer/research/gdpnow) (nowcast), Nasdaq Data Link | Free | Easy | Excel/API | BEA official, GDPNow for real-time |
| **Personal Consumption** | Household spending by category | [BEA Personal Income/Outlays](https://www.bea.gov/news/glance) | Moody's ($$$$), Haver ($$) | Free | Easy | Excel/API | Monthly updates |
| **Fixed Investment** | Business investment by type | BEA NIPA Table 1.1.5 | Commercial providers | Free | Easy | Excel/API | Quarterly, 2-month lag |
| **Government Consumption** | Federal + State/Local spending | BEA NIPA Tables | [USAFacts](https://usafacts.org/economy/) (simplified) | Free | Easy | Excel/API | Quarterly updates |

## **Financial Flow Accounts**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Household Balance Sheets** | Assets, liabilities, net worth | [Fed Z.1 Tables](https://www.federalreserve.gov/releases/z1/) | Moody's ($$$$), Haver ($$) | Free | Medium | CSV/HTML via DDP | Quarterly, comprehensive |
| **Corporate Finance** | Business debt, equity, cash | Fed Z.1 F.103, L.103 | S&P Global ($$), Bloomberg ($$$$) | Free | Medium | CSV download | Quarterly, 10-week lag |
| **Banking Sector** | Bank assets, loans, deposits | Fed Z.1 + H.8 Bank Assets | Haver ($$), FDIC data | Free | Medium | CSV/API | Weekly H.8, Quarterly Z.1 |
| **Government Debt** | Federal + S&L debt positions | Fed Z.1 F.106, F.107 | Treasury Direct, USAFacts | Free | Easy | CSV download | Quarterly comprehensive |

## **Labor Market Data**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Employment by Sector** | Payroll employment 71 industries | [BLS CES](https://www.bls.gov/ces/) | Nasdaq Data Link, [Macrotrends](https://www.macrotrends.net/charts/economy) | Free | Easy | Excel/API | Monthly, 1-week lag |
| **Unemployment Rates** | National + demographic breakdown | [BLS LFS](https://www.bls.gov/cps/) | FRED, Macrotrends | Free | Easy | Excel/API | Monthly releases |
| **Wages by Industry** | Average hourly earnings by sector | BLS Average Hourly Earnings | Haver ($$), BLS API | Free | Easy | API/Excel | Monthly updates |
| **Labor Force Participation** | Working age population dynamics | BLS Labor Force Statistics | FRED aggregation | Free | Easy | Excel/API | Monthly, seasonally adjusted |

## **Government Finance & Fiscal Data**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Federal Tax Revenue** | Income, corporate, payroll taxes | [Treasury Monthly Statement](https://fiscal.treasury.gov/reports-statements/) | IRS Statistics of Income (annual) | Free | Medium | PDF/Excel | Monthly Treasury data |
| **Federal Spending** | By function and agency | USASpending.gov | [USAFacts Government Spending](https://usafacts.org/economy/) | Free | Medium | CSV download | USAFacts provides cleaner interface |
| **State/Local Finance** | Revenue and expenditure by state | [Census Annual Survey](https://www.census.gov/programs-surveys/state/) | Lincoln Institute, Urban Institute | Free | Hard | Excel/PDF | 2-year lag, complex |
| **Social Benefits** | SS, Medicare, unemployment, etc. | SSA, DOL, CMS separately | Census consolidated data | Free | Hard | Multiple formats | Fragmented across agencies |
| **Tax Rates (Effective)** | Calculated effective rates | CBO reports, NBER TAXSIM | Tax Foundation, Moody's ($$$$) | Free* | Hard | Research papers | Need to calculate from microdata |

## **Interest Rates & Monetary Data**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Policy Rates** | Fed Funds, discount window | [Fed H.15 Interest Rates](https://www.federalreserve.gov/releases/h15/) | FRED, Nasdaq Data Link | Free | Easy | Excel/API | Daily updates |
| **Term Structure** | Treasury yield curve | Fed H.15, Treasury Direct | Bloomberg ($$$$), Refinitiv ($$$$) | Free | Easy | Excel/API | Daily government data |
| **Corporate Rates** | Commercial lending rates | Fed H.15 Commercial Paper | Moody's ($$$$), S&P ($$$) | Free* | Medium | Excel download | Limited granularity for free |
| **Money Supply** | M1, M2, monetary aggregates | [Fed H.6 Money Stock](https://www.federalreserve.gov/releases/h6/) | FRED aggregation | Free | Easy | Excel/API | Weekly releases |

## **External Sector & Trade Data**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Trade Flows** | Exports/imports goods & services | [BEA International Trade](https://www.bea.gov/news/glance) | Census Bureau trade data | Free | Easy | Excel/API | Monthly, 6-week lag |
| **Current Account** | Balance of payments | BEA International Transactions | IMF Balance of Payments | Free | Easy | Excel download | Quarterly, comprehensive |
| **Exchange Rates** | Trade-weighted dollar index | [Fed H.10 Exchange Rates](https://www.federalreserve.gov/releases/h10/) | FRED, commercial providers | Free | Easy | Excel/API | Daily updates |
| **Foreign Investment** | FDI flows and stocks | BEA International Investment Position | OECD FDI database | Free | Medium | Excel download | Annual, detailed |

## **Initial Conditions & Calibration Data**

| Data Category | Specific Requirements | Primary Source | Alternative Sources | Cost | Integration Ease | Format/Access | Notes |
|---------------|----------------------|----------------|-------------------|------|------------------|---------------|-------|
| **Baseline Period Data** | All variables for 2010Q1 (Austria reference) | Multiple sources above | Integrated commercial platform | Free* | Hard | Multiple downloads | Requires harmonization |
| **Forecast Parameters** | Taylor rule, autoregressive coefficients | Atlanta Fed research, Fed models | Moody's Global Model ($$$$) | Free* | Hard | Academic papers | Need econometric estimation |
| **Behavioral Parameters** | Consumption, investment elasticities | BEA research, academic papers | Commercial macro models | Free* | Hard | Research literature | Calibration-intensive |

## **Cost & Integration Summary**

### **Cost Legend:**

- **Free**: Government sources, no cost
- **$**: Under $5K annually  
- **$$**: $5K-15K annually
- **$$$**: $15K-50K annually
- **$$$$**: $50K+ annually

### **Integration Ease:**

- **Easy**: Direct download/API, ready-to-use format
- **Medium**: Some processing required, good documentation  
- **Hard**: Complex integration, manual processing needed

### **Recommended Strategy by Budget:**

| Budget Level | Recommended Approach | Coverage | Total Cost |
|--------------|---------------------|----------|------------|
| **Research/Academic** | Free government sources + academic discounts | 90% | $0-2K |
| **Small Commercial** | Free sources + targeted commercial (IMPLAN, basic Haver) | 95% | $5K-15K |
| **Full Commercial** | Comprehensive platform (Moody's/Haver) + government supplements | 99% | $30K-60K |

The **sweet spot** for most projects appears to be the "Small Commercial" approach, combining free government data with targeted commercial sources for the most challenging integration points.
