# NBFC Quant Toolbox - 1000+ Financial Tools

A comprehensive single-file HTML application containing 200+ mini-applications for Indian NBFC/Bank employees. All tools run 100% locally in the browser with no server uploads required.

## Features

- **Browser-Based Persistence**: IndexedDB for tool states and CSV datasets, LocalStorage for preferences
- **Multi-Tier Navigation**: Search (Ctrl+K), department tabs, favorites, and recent tools
- **Save/Load States**: Save tool inputs for later use with named slots
- **Export/Import**: Full backup and restore of all saved data

---

## Tools by Category

### Retail Lending

| Tool | One-Line Description |
|------|---------------------|
| **Retail Eligibility (FOIR)** | Max loan calculator based on Income & Obligations |
| **Loan Against Property (LAP)** | LTV vs FOIR eligibility check |
| **Education Loan Structurer** | Moratorium interest & capitalization for education loans |
| **Home Loan Eligibility** | FOIR + LTV with stamp duty and insurance adders |
| **Auto Loan On-Road Structurer** | On-road price breakup, margin, FOIR & tenure |
| **Gold Loan LTV Optimizer** | LTV vs per-gram price and auction buffer |
| **Personal Loan Top-Up Calculator** | Top-up eligibility net of foreclosure and charges |
| **Balance Transfer Savings Estimator** | EMI and interest savings after BT with fees |
| **FOIR Calculator** | Fixed Obligation to Income Ratio check |
| **EMI Calculator** | Standard EMI calculation with amortization schedule |
| **Prepayment Calculator** | Impact of part/full prepayment on loan |
| **Step-Up EMI Calculator** | Graduated EMI plan with annual increases |
| **Part-Payment Optimizer** | Reduce EMI vs reduce tenure analysis |
| **Rate Reset Calculator** | New EMI after MCLR/repo rate change |
| **Co-Borrower Income Split** | Combine incomes for eligibility check |
| **Debt Consolidation Analyzer** | Consolidate multiple loans into one |
| **Loan Comparison Tool** | Compare multiple loan offers side by side |
| **Effective Interest Rate (EIR)** | True cost of loan with fees and charges (Ind AS 109 compliant) |
| **Tenure Optimizer** | Optimal tenure for target EMI or total interest |
| **Moratorium Impact Calculator** | EMI change after moratorium period |
| **Floating Rate Risk Analyzer** | EMI sensitivity to rate changes |
| **LTV Calculator & Analyzer** | Loan-to-Value with multiple collaterals |
| **Margin Money Calculator** | Required margin for different products |
| **Amortization Schedule Analyzer** | Analyze EMI split over loan life with yearly summary |
| **Prepayment Impact Analyzer** | Compare reduce-EMI vs reduce-tenure options |

#### Detailed Descriptions

**Retail Eligibility (FOIR)**: Enter Net Income & EMIs to get Max Loan. Calculates maximum eligible loan amount based on Fixed Obligation to Income Ratio norms, considering existing EMIs and other fixed obligations.

**Loan Against Property (LAP)**: Compares Property-based vs Income-based limits. Determines the lower of LTV-based and FOIR-based eligibility for LAP applications.

**Education Loan Structurer**: Structures loan with study-period interest logic. Calculates interest accrual during moratorium/study period and capitalizes it into principal for EMI calculation.

**Home Loan Eligibility**: Input income, property value, duties, existing EMIs. Comprehensive eligibility calculator that factors in stamp duty, registration, insurance premiums, and existing obligations.

**Auto Loan On-Road Structurer**: Enter ex-showroom, taxes, accessories, and income. Breaks down on-road price into components and calculates maximum financing based on FOIR and margin requirements.

**Gold Loan LTV Optimizer**: Enter karat, grams, market price, and margin. Calculates loan eligibility based on gold purity, weight, and current market rates while maintaining auction buffers.

**Personal Loan Top-Up Calculator**: Enter OS balance, rate, remaining tenor, new rate. Determines additional loan amount available considering existing loan obligations and foreclosure charges.

**Balance Transfer Savings Estimator**: Compare current EMI vs proposed EMI and one-time fees. Quantifies total savings from balance transfer after accounting for processing fees and prepayment charges.

**FOIR Calculator**: Enter income, existing EMIs, proposed EMI, other obligations. Validates if proposed loan fits within FOIR limits (typically 40-60% based on income slab).

**EMI Calculator**: Enter principal, rate, tenure; get EMI and amortization. Standard reducing balance EMI calculation with full amortization schedule showing principal/interest split.

**Prepayment Calculator**: Enter outstanding, rate, remaining tenure, prepay amount. Shows impact on EMI or tenure after partial prepayment, with interest savings calculation.

**Step-Up EMI Calculator**: Enter loan, rate, tenure, step-up % per year. Creates graduated payment schedule where EMI increases annually, useful for borrowers expecting income growth.

**Part-Payment Optimizer**: Compare prepayment strategies for savings. Analyzes whether to reduce EMI (lower monthly outgo) or reduce tenure (higher interest savings).

**Rate Reset Calculator**: Enter current EMI, outstanding, remaining tenure, rate change. Calculates new EMI after floating rate reset due to repo/MCLR changes.

**Co-Borrower Income Split**: Enter primary and co-borrower incomes, obligations. Combines multiple income sources to determine total eligible loan amount with proper FOIR application.

**Debt Consolidation Analyzer**: Enter existing loans; see consolidated EMI savings. Compares total current EMI burden vs single consolidated loan EMI to show monthly savings.

**Loan Comparison Tool**: Enter up to 4 loan offers; compare EMI, total cost, effective rate. Side-by-side comparison highlighting best option based on total cost of borrowing.

**Effective Interest Rate (EIR)**: Enter principal, EMI, tenure, processing fee; get effective rate. Calculates true cost of loan including all upfront fees and charges as per Ind AS 109 requirements.

**Tenure Optimizer**: Enter loan amount, rate, and target; find optimal tenure. Shows tenure options with EMI affordability check against FOIR and total interest cost comparison.

**Moratorium Impact Calculator**: Enter loan details and moratorium months; see new EMI and total cost. Calculates interest capitalization during moratorium and resulting increase in EMI or tenure.

**Floating Rate Risk Analyzer**: Enter loan details; see EMI at different rate scenarios. Scenario analysis showing EMI and total interest impact for various rate change scenarios (+/-25, 50, 100 bps).

**LTV Calculator & Analyzer**: Enter property values and loan; compute LTV with haircuts. Checks LTV against product-specific norms (Home: 80%, LAP: 65%, Gold: 75%, Vehicle: 85%).

**Margin Money Calculator**: Enter loan amount and product; get margin requirement. Calculates required down payment/margin based on LTV norms for different loan products.

**Amortization Schedule Analyzer**: See principal/interest split, cumulative payments by period. Generates detailed month-wise and year-wise amortization with principal/interest breakup.

**Prepayment Impact Analyzer**: Enter prepayment amount; see savings in both scenarios. Compares reduce-EMI vs reduce-tenure options with total interest savings for each approach.

---

### MSME & Corporate

| Tool | One-Line Description |
|------|---------------------|
| **Supply Chain / Invoice Discounting** | Net disbursement & yield calculator |
| **Corporate Financial Analysis** | Financial statement spreading & ratio analysis |
| **Co-Lending Structurer** | Blended rate & spread calculator for 80:20 deals |
| **Working Capital Gap Analyzer** | Net working capital vs drawing power |
| **Cash-Credit DP Calculator** | Stock and book debts net of margins and ineligibles |
| **Bill Discounting Limit Setter** | Limit sizing from turnover, acceptances, and tenor |
| **Project Finance DSCR Builder** | DSCR timeline with moratorium and ballooning |
| **Consortium Share Allocator** | Bank-wise share, security, and rate splits |
| **DSCR Calculator** | Debt Service Coverage Ratio |
| **Financial Spreading Tool** | Analyze 3-year financials |
| **Cash Credit DP Calculator** | Drawing power calculation |
| **CGTMSE Calculator** | CGTMSE guarantee fee calculation |
| **Udyam Validator** | Validate Udyam registration |
| **Turnover Method Limit** | WC limit by turnover method |
| **Ratio Analysis Dashboard** | Key financial ratios analysis |
| **Bill Discounting Calculator** | Discount rate and proceeds |
| **MSME Classification Tool** | Classify as Micro/Small/Medium |
| **Quick Financial Ratios** | Instant ratio calculations with benchmarks |

#### Detailed Descriptions

**Supply Chain / Invoice Discounting**: Calculates upfront discount and effective yield. Determines net disbursement after discount deduction and computes annualized yield for the financier.

**Corporate Financial Analysis**: Enter financials to get DSCR, DE, Current Ratio. Comprehensive financial spreading with automatic ratio calculation from P&L and Balance Sheet inputs.

**Co-Lending Structurer**: Input Bank/NBFC share to get Blended Rate. Calculates weighted average lending rate for co-lending arrangements with proper spread allocation.

**Working Capital Gap Analyzer**: Enter inventory, receivables, payables, bank margins. Computes net working capital requirement using operating cycle method.

**Cash-Credit DP Calculator**: Upload stock & debtor aging; set margin %. Calculates drawing power after applying margins and excluding ineligible stocks/debtors.

**Bill Discounting Limit Setter**: Enter turnover, average acceptance days, dilution %. Sizes bill discounting limit based on turnover and typical outstanding period.

**Project Finance DSCR Builder**: Upload project cash flows; set debt profile. Creates year-by-year DSCR projection considering moratorium and balloon payments.

**Consortium Share Allocator**: Enter facility amount and bank participation %. Allocates security value, interest rate, and exposure across consortium members.

**DSCR Calculator**: Enter EBITDA, interest, principal; compute DSCR. Simple DSCR calculation with interpretation (>1.25 typically acceptable).

**Financial Spreading Tool**: Enter P&L and BS data; auto-compute ratios. Organizes 3-year financials with YoY growth and all key ratios calculated automatically.

**Cash Credit DP Calculator**: Enter debtors, stock, margins; compute DP. Standard drawing power calculation with aging-based debtor eligibility.

**CGTMSE Calculator**: Enter loan amount, tenure; compute guarantee fee. Calculates one-time and annual guarantee fees under CGTMSE scheme.

**Udyam Validator**: Enter Udyam number; validate format and lookup. Checks Udyam registration number format and classification.

**Turnover Method Limit**: Enter turnover, margin; compute permissible limit. Calculates WC limit as 20-25% of projected turnover (Nayak Committee method).

**Ratio Analysis Dashboard**: Enter financials; view profitability, liquidity ratios. Displays all key ratios with traffic-light indicators against industry benchmarks.

**Bill Discounting Calculator**: Enter bill amount, tenor, rate; compute proceeds. Calculates net proceeds after discount and effective yield.

**MSME Classification Tool**: Enter investment, turnover; classify per RBI norms. Classifies enterprise as Micro/Small/Medium based on current investment and turnover criteria.

**Quick Financial Ratios**: Enter basic financials; get all key ratios at once. Computes 10 key ratios (EBITDA margin, ROE, D/E, Interest Cover, etc.) with benchmark comparison.

---

### Collections & Recovery

| Tool | One-Line Description |
|------|---------------------|
| **Early Warning Scorecard** | DPD + bureau + bounce triggers for risk classification |
| **Promise-to-Pay Tracker** | PTP capture, hit-rate, and slippage monitor |
| **Settlement Offer Optimizer** | Optimal settlement curves by bucket |
| **Roll-Rate Cube Visualizer** | DPD migration matrix over time |
| **Cure Rate Forecast** | Forecast cures using logistic fit |
| **Field Ops Route Planner** | Route prioritisation by amount and proximity |
| **Legal Bucket ROI Calculator** | Compare legal costs vs expected recoveries |
| **Delinquency Ladder Converter** | Map PAR/DPD ladder to lifetime loss and spread |
| **Bounce Analysis** | NACH/ECS bounce rate by reason |
| **OTS Calculator** | One-time settlement computation |
| **DPD Bucket Report** | Delinquency bucket analysis |
| **Collection Agent Performance** | Agent-wise collection efficiency |
| **Payment Plan Builder** | Custom repayment plans for delinquents |
| **Agency Payout Calculator** | Collection agency commission calculation |
| **Recovery Forecast Model** | Project future recoveries from NPA pool |
| **Penal Interest Calculator** | Calculate penal charges on overdue EMIs |
| **Interest on Interest Calculator** | Compound interest on unpaid interest |
| **Collection Efficiency Calculator** | CE% with different methodologies |

#### Detailed Descriptions

**Early Warning Scorecard**: Upload loans with DPD; classify risk categories. Categorizes accounts into risk buckets based on DPD, bureau alerts, and bounce frequency.

**Promise-to-Pay Tracker**: Upload PTP log with dates, amounts, status. Tracks PTP success rate, broken promises, and collection efficiency by agent/bucket.

**Settlement Offer Optimizer**: Set bucket-wise min %, cost-to-collect, recoveries. Determines optimal settlement percentage by DPD bucket to maximize recovery NPV.

**Roll-Rate Cube Visualizer**: Upload DPD snapshots; see heatmap and stability. Visualizes flow rates between DPD buckets over multiple periods.

**Cure Rate Forecast**: Upload bucketed cures; tool fits curve for outlook. Uses logistic regression to project cure rates for delinquent accounts.

**Field Ops Route Planner**: Upload address+amount; set max visits/day. Optimizes field collection route to maximize amount covered per day.

**Legal Bucket ROI Calculator**: Enter claim amount, fees, win rate, timeline. Compares expected recovery vs legal costs to determine if legal action is worthwhile.

**Delinquency Ladder Converter**: Input PAR30/60/90, cure rates, LGD, WAL to get implied loss and bps. Converts PAR buckets to expected lifetime loss and required risk spread.

**Bounce Analysis**: Upload bounce file with reason codes; view patterns. Analyzes bounce patterns by bank, time of month, and reason codes.

**OTS Calculator**: Enter outstanding, provisions, recovery cost; get OTS range. Calculates acceptable settlement range based on expected recovery and costs.

**DPD Bucket Report**: Upload loan tape with DPD; view bucket distribution. Generates PAR report with bucket-wise outstanding and count.

**Collection Agent Performance**: Upload collection log; view agent metrics and ranking. Ranks agents by collection efficiency, resolution rate, and PTP conversion.

**Payment Plan Builder**: Enter overdues, capacity; generate flexible plan. Creates customized repayment schedule based on borrower's payment capacity.

**Agency Payout Calculator**: Enter collections, slab rates; calculate payout. Computes collection agency commission based on slab-wise rates and bucket-wise collections.

**Recovery Forecast Model**: Enter NPA pool, historical recovery curve; forecast. Projects future recoveries using historical recovery patterns.

**Penal Interest Calculator**: Enter overdue amount, DPD, penal rate; get charges. Calculates penal interest as per RBI guidelines (simple or compound).

**Interest on Interest Calculator**: For moratorium/default scenarios; compute IoI. Calculates compound interest on unpaid interest (relevant for SC moratorium order).

**Collection Efficiency Calculator**: Enter demand and collection; compute CE by bucket. Calculates collection efficiency ratio as per RBI methodology.

---

### Risk & Compliance

| Tool | One-Line Description |
|------|---------------------|
| **NPA & Provisioning (IRAC)** | Asset classification & provisioning per RBI norms |
| **Static Pool Analyzer** | Vintage analysis heatmap (Triangular View) |
| **Geo Performance Visualiser** | State/district AUM & PAR view |
| **Regulatory Return Validator** | CRILC / RBI schema QC |
| **Policy Matrix Validator** | Rules vs portfolio hit-rate |
| **Thin File Surrogate Score** | Alternate data weights for thin files |
| **Bureau Score Cutoff Optimizer** | Cutoff vs approval and loss trade-off |
| **Income Surrogate Uplift Analyzer** | Incremental approvals from surrogate income |
| **Fraud Rule Hit-Rate Tracker** | Rule-wise hit, precision, and recall |
| **PD/LGD/EAD Calibrator** | Binning + WoE and calibration |
| **Vintage CNL & NCL Tracker** | Cumulative loss tracking by vintage |
| **PAR/DPD Triangle Explorer** | PAR matrix across MOB and vintages |
| **CCF Calculator** | CCF by product, utilisation, and behavior |
| **Stress Loss Attribution** | Impact of PD/LGD shocks separately |
| **Gini/KS Model Validation** | Scorecard validation metrics |
| **Capital Adequacy Calculator** | RWA, CAR, Tier-1 buffers |
| **Leverage Ratio Monitor** | Tier-1 capital vs exposure measure |
| **ICAAP Scenario Worksheet** | Scenario-wise capital consumption |
| **IRAC Rule Engine** | Multi-product IRAC classification |
| **IND-AS ECL Calculator** | Stage migration and lifetime ECL |
| **ECL Calculator (Ind AS 109)** | Expected Credit Loss computation |
| **Gini/KS Score Tracker** | Model discrimination metrics |
| **Provision Coverage Ratio** | PCR calculation with stage breakdown |
| **SMA Classification Tool** | SMA-0/1/2 bucket classification |
| **Write-Off Eligibility Checker** | Check accounts eligible for write-off |
| **Concentration Risk Analyzer** | Sector/geography/borrower concentration |
| **GNPA/NNPA Calculator** | Gross and Net NPA ratios |
| **PAR Report Generator** | Portfolio at Risk by DPD bucket |

#### Detailed Descriptions

**NPA & Provisioning (IRAC)**: Upload account DPD; get IRAC class & provision. Classifies assets as Standard/SMA/Substandard/Doubtful/Loss and calculates provisions (0.4%, 15%, 25%, etc.).

**Static Pool Analyzer**: Upload vintage loss data; view cohort analysis table. Creates triangular view of cumulative losses by vintage and MOB for trend analysis.

**Geo Performance Visualiser**: Upload state/district metrics; visualize geographic risk. Maps AUM and PAR across geographies for concentration analysis.

**Regulatory Return Validator**: Upload CSV/XML; get missing/format errors. Validates CRILC, ALM, and other regulatory return formats for schema compliance.

**Policy Matrix Validator**: Upload rules and portfolio; see pass/fail % and overrides. Tests credit policy rules against portfolio to measure hit rates.

**ECL Calculator (Ind AS 109)**: Enter EAD, PD, LGD by stage; compute ECL. Calculates Expected Credit Loss as PD × LGD × EAD for each Ind AS 109 stage.

**Gini/KS Score Tracker**: Upload score, good/bad flag; compute Gini and KS. Validates scorecard discrimination with Gini, KS, and Lift charts.

**GNPA/NNPA Calculator**: Enter advances, gross NPA, provisions; compute ratios. Calculates Gross and Net NPA ratios as per RBI disclosure requirements.

---

### Treasury & ALM

| Tool | One-Line Description |
|------|---------------------|
| **XIRR & Cashflow Analyzer** | Account-wise and portfolio XIRR |
| **HPR & Annualised Return** | Holding period returns for securities |
| **ALM Stress & Duration Lab** | Parallel + twist scenarios |
| **Macro / CMIE Dashboard** | GDP & CPI quick view |
| **FX Forward Coverage Planner** | Coverage ladder vs payable schedule |
| **CP/CD Issuance Planner** | Optimal size/tenor vs ALM and investors |
| **Bond Yield-to-Worst Tool** | YTW across call/put schedules |
| **Duration Matching Optimizer** | Match asset/liability duration |
| **Liquidity Gap (Behavioral)** | ALM with decay and prepayment assumptions |
| **FX Swap vs Forward Arbitrage Checker** | Checks covered interest parity |
| **FTP Curve Builder** | Funds transfer pricing term structure |
| **Cost of Funds Tracker** | Weighted cost by source mix |
| **ECB vs NCD Funding Choice** | Compare all-in cost and covenants |
| **Callable vs Non-Callable Ladder** | Ladder planner for callable paper |
| **Bond YTM Calculator** | Yield to maturity for bonds |
| **Duration & Convexity** | Bond price sensitivity measures |
| **Cost of Funds Calculator** | Blended cost of all funding sources |
| **NIM Bridge Calculator** | Break down NIM movement drivers |
| **LCR/NSFR Calculator** | Liquidity coverage and stable funding ratios |
| **Interest Rate Scenario** | NII impact under rate shocks |
| **Portfolio Yield to Maturity** | YTM of loan portfolio considering prepay |

#### Detailed Descriptions

**XIRR & Cashflow Analyzer**: Upload raw cashflows. Negative=disbursal. Calculates account-wise and portfolio-level XIRR from irregular cash flow dates.

**HPR & Annualised Return**: Upload instrument ledger. Computes holding period return and annualized return for traded securities.

**ALM Stress & Duration Lab**: Duration/Convexity analysis. Runs parallel and twist scenarios on rate curve to measure NII and EVE impact.

**Cost of Funds Calculator**: Enter mix and rate per source; view WAC trend. Calculates weighted average cost of funds across all borrowing sources.

**NIM Bridge Calculator**: Enter yield, CoF changes; see NIM waterfall. Decomposes NIM movement into asset yield, cost of funds, and mix effects.

**LCR/NSFR Calculator**: Enter HQLA, outflows, stable funding; compute ratios. Calculates Basel III liquidity ratios with bucket-wise breakdown.

**Portfolio Yield to Maturity**: Enter portfolio with prepay assumptions; get YTM. Computes effective YTM considering prepayment rates and fee income.

---

### Securitisation

| Tool | One-Line Description |
|------|---------------------|
| **Indian Securitisation AI Suite** | End-to-end PTC modeling: Waterfall, Gaussian Copula LE, Pricing, Term Sheet |
| **DA Upfront Income Calculator** | Manual + pool CSV calculation for IO strip value |
| **CE Sufficiency Back-tester** | Back-test CE vs historical losses |
| **Trigger Breach Monitor** | Track OC/CC/DR triggers |
| **Replenishment Pool QC** | QC checklist for replenishment criteria |
| **Delinquency Diversion Scenario** | Simulate diversion of delinq collections |
| **Collateral Stratification Dashboard** | Strats by LTV, bureau, geography |
| **Waterfall Comparator** | Compare structure A vs B outputs |
| **Pool Yield Calculator** | Weighted average yield of loan pool |

#### Detailed Descriptions

**Indian Securitisation AI Suite**: Complete suite for PTC transactions. 1. Waterfall: Define structure & run flow. 2. LE: Run simulation for Credit Enhancement. 3. Docs: Generate Term Sheet.

**DA Upfront Income Calculator**: Upload pool with POS, Rate, Tenure; calculate IO strip value. Computes upfront income from Direct Assignment transactions.

**CE Sufficiency Back-tester**: Upload pool loss curves; test CE % sufficiency. Tests if credit enhancement would have been sufficient under historical stress.

**Trigger Breach Monitor**: Upload monthly pool metrics; flag breaches. Monitors OC ratio, collection ratio, and delinquency ratio triggers.

**Pool Yield Calculator**: Enter loans with amounts and rates; get pool WAY. Calculates weighted average yield of securitisation pool.

---

### Operations

| Tool | One-Line Description |
|------|---------------------|
| **TAT Monitor** | Turnaround time tracking |
| **E-NACH Success Forecaster** | Predicts success by bank and time |
| **Bounce Fee Engine** | Bounce fee rules and realized collections |
| **Escrow Reconciliation Tool** | Match escrow credits to loans |
| **PDC Inventory Tracker** | Track PDC status and expiries |
| **Service Request SLA Dashboard** | SLA adherence for service tickets |
| **KYC Completeness Checker** | KYC field gap analysis |
| **Udyam/GST Mismatch Detector** | Cross-check Udyam vs GST data |
| **Disbursement TAT Monitor** | Stage-wise TAT and bottleneck finder |
| **NACH Status Tracker** | NACH mandate status monitoring |
| **Document Checklist** | Loan document completeness check |
| **Disbursement Queue Manager** | Track pending disbursements |
| **EMI Schedule Generator** | Generate printable EMI schedule |
| **Balance Confirmation Letter** | Generate balance confirmation |
| **Foreclosure Statement** | Pre-closure amount calculation |
| **NOC Generator** | No Objection Certificate generator |
| **Stamp Duty & Registration Calculator** | State-wise stamp duty for loan documents |
| **PDC/RPDC Calculator** | Generate cheque series for EMI |
| **Grace Period Interest Calculator** | Interest accrued during grace period |
| **Disbursal Pacing Calculator** | Monthly disbursal to hit annual target |

#### Detailed Descriptions

**TAT Monitor**: Upload application timestamps; view SLA hits. Tracks turnaround time at each process stage and identifies bottlenecks.

**E-NACH Success Forecaster**: Upload NACH attempts with bank/time; get success lift. Predicts NACH success rate by bank and presentation time.

**Bounce Fee Engine**: Enter product-wise fee rules and bounce counts. Calculates bounce charges and tracks collection of the same.

**Document Checklist**: Select product; see required documents checklist. Product-specific document requirements with checklist for loan processing.

**Foreclosure Statement**: Enter loan; calculate foreclosure amount with charges. Computes total amount payable for loan closure including charges.

**Stamp Duty & Registration Calculator**: Select state, document type, loan amount; get duty payable. State-wise stamp duty and registration charge calculator.

**PDC/RPDC Calculator**: Enter EMI, start date, tenure; get cheque schedule. Generates post-dated cheque schedule with dates and amounts.

**Grace Period Interest Calculator**: Enter principal, rate, grace days; get accrued interest. Calculates pre-EMI interest during construction or grace period.

**Disbursal Pacing Calculator**: Enter YTD disbursal and target; get monthly run-rate needed. Calculates required monthly disbursement to achieve annual target.

---

### Pricing & Profitability

| Tool | One-Line Description |
|------|---------------------|
| **Risk-Based Pricing Grid Builder** | Price grid by risk bands and LTV/FOIR |
| **NIM Bridge Analyzer** | Drivers of NIM movement |
| **Net Yield after Costs** | Product net yield after all costs |
| **Upfront vs Amortized Fee Impact** | PV and accrual impact of fees |
| **Cross-Sell Take-Rate Forecaster** | Forecast take-rate and margin |
| **Prepayment Penalty Optimizer** | Optimal prepay charges vs attrition |
| **Loss-Leader Payback Calculator** | Payback period for promo offers |
| **Annualised Loss Rate (Risk Premium)** | Convert lifetime loss to annualised credit spread |
| **Vintage Loss Forecaster** | Extrapolate partial vintage losses to full lifetime |
| **Stress Uplift Recommender** | Scenario add-ons for GDP, inflation, rate shocks |
| **Co-Lending First-Loss Splitter** | Spread split given FLDG/first-loss share |
| **Bureau Score Cutoff Pricing** | Discount/premium by score band |
| **Product Mix Risk Uplift** | Weighted risk premium by product PD/LGD |
| **Severity vs Frequency Decomposer** | Split lifetime loss into PD and LGD levers |
| **Lifetime Loss to Annualized Spread** | Convert lifetime loss to annual risk spread for amortizing loans |
| **Interest Rate Converter** | Convert between flat, reducing, APR, EIR |
| **Break-Even Spread Calculator** | Min spread needed to cover costs and loss |
| **Penal Waiver Yield Impact** | Impact of penal interest waiver on total yield |
| **Subvention Calculator** | Dealer/manufacturer subvention computation |
| **Risk-Adjusted Return (RAROC)** | Return on capital adjusted for risk |

#### Detailed Descriptions

**Risk-Based Pricing Grid Builder**: Define bands; export pricing matrix. Creates rate grid by risk band (bureau score, LTV, FOIR) for automated pricing.

**NIM Bridge Analyzer**: Enter asset yield, CoF, OPEX, LLP changes. Decomposes NIM movement into component drivers with waterfall visualization.

**Net Yield after Costs**: Enter rates, fees, CoF, opex, credit cost. Calculates net yield after deducting all costs for product profitability.

**Lifetime Loss to Annualized Spread**: Enter principal, rate, tenure, prepay rate, lifetime loss; get annualized spread in bps. Converts lifetime loss percentage to annualized risk spread for loan pricing.

**Interest Rate Converter**: Enter rate in one format; see equivalent in all formats. Converts between flat rate, reducing rate, monthly rate, and APR.

**Break-Even Spread Calculator**: Enter CoF, opex, credit loss, capital cost; get break-even spread. Calculates minimum lending rate to break even after all costs.

**Penal Waiver Yield Impact**: Enter loan details and waiver amount; see yield and IRR impact. Quantifies impact of penal interest waiver on transaction yield in bps.

**Subvention Calculator**: Enter subvention scheme; compute payout and net rate. Calculates dealer/manufacturer subvention amount and effective customer rate.

**Risk-Adjusted Return (RAROC)**: Enter income, loss, capital; compute RAROC. Calculates risk-adjusted return on capital for profitability assessment against hurdle rate.

---

### Regulatory & Compliance

| Tool | One-Line Description |
|------|---------------------|
| **RLNG/ALM Form Pack Validator** | Schema QC for regulatory forms |
| **FATCA/CRS Flagger** | Flags reportable accounts |
| **CRILC Data Validator** | Validate CRILC submission format |
| **TDS Calculator** | TDS on interest/fees calculation |
| **Form 15G/15H Validator** | Validate 15G/H declarations |
| **KYC Completeness Checker** | Check KYC document completeness |
| **AML Risk Rating** | Customer AML risk classification |
| **Large Exposure Check** | RBI large exposure limit check |
| **CAR Calculator** | Capital Adequacy Ratio computation |
| **PSL Classification Tool** | Priority sector lending classification |
| **Regulatory Calendar** | RBI/SEBI submission deadlines |

#### Detailed Descriptions

**CRILC Data Validator**: Upload CRILC file; check for errors and warnings. Validates Central Repository of Information on Large Credits submission format.

**TDS Calculator**: Enter interest amount, PAN status; compute TDS. Calculates TDS on interest and fees with rate based on PAN availability.

**KYC Completeness Checker**: Enter customer type; check required KYC fields. Lists required KYC documents based on customer type and checks completeness.

**AML Risk Rating**: Enter customer profile; compute AML risk score. Scores customers on AML risk based on occupation, geography, transaction patterns.

**CAR Calculator**: Enter capital, RWA; compute CRAR. Calculates Capital to Risk-weighted Assets Ratio for regulatory compliance.

**PSL Classification Tool**: Enter loan purpose, amount; classify under PSL norms. Classifies loans under Priority Sector Lending categories.

**Regulatory Calendar**: View upcoming regulatory filing dates. Calendar of RBI, SEBI, and other regulatory submission deadlines.

---

### Microfinance

| Tool | One-Line Description |
|------|---------------------|
| **Microfinance Group Loan Splitter** | Group-level and member-level ticket sizing |

#### Detailed Descriptions

**Microfinance Group Loan Splitter**: Enter group income, member list, and repeat vs new. Sizes individual loans within a JLG/SHG based on member income and track record.

---

### Cards & Digital

| Tool | One-Line Description |
|------|---------------------|
| **Credit Card Limit Engine** | Limit setting using income, bureau, and utilization |
| **Revolver vs Transactor Profitability** | Profit bridge by revolve share and costs |
| **BNPL Tenor Pricing Tool** | Tenor-wise MDR, subvention, and NPV |
| **MDR & Interchange Simulator** | Take rate decomposition and net yield |
| **EMI Conversion Offer Picker** | Best plan given fee, tenure, and uptake |
| **Rewards Liability Forecaster** | Accrual vs redemption and breakage |

#### Detailed Descriptions

**Credit Card Limit Engine**: Enter income, bureau score, utilization bands. Sets credit limit based on income multiples and bureau score bands.

**Revolver vs Transactor Profitability**: Input revolve rate, MDR, funding cost, rewards %. Compares profitability of revolving vs transacting customers.

**BNPL Tenor Pricing Tool**: Enter ticket size, MDR/subvention %, loss %, CoF. Prices BNPL products by tenor considering all cost components.

---

### MIS & Reporting

| Tool | One-Line Description |
|------|---------------------|
| **AUM/OS Rollforward Builder** | Open, disb, collection, prepay, close |
| **Cohort Retention Dashboard** | Retention curves by cohort |
| **Geo Heatmap (RBI Districts)** | District-level AUM and PAR |
| **Segment Profitability Tree** | Waterfall of revenue to PAT by segment |
| **Early Delinquency Pulse (0-30)** | Early bucket monitoring |
| **New-to-Credit Performance Tracker** | NTC vs existing borrower performance |

#### Detailed Descriptions

**AUM/OS Rollforward Builder**: Upload monthly flows; tool builds rollforward. Creates opening balance → disbursements → collections → prepayments → closing balance reconciliation.

**Cohort Retention Dashboard**: Upload cohort-months; view survival curves. Tracks customer retention by origination cohort over time.

**Geo Heatmap (RBI Districts)**: Upload district codes and metrics; see map/heat. Visualizes portfolio metrics on India district map.

**Segment Profitability Tree**: Upload segment P&L; view waterfall. Shows revenue to PAT waterfall by business segment.

---

### Data Quality & Utilities

| Tool | One-Line Description |
|------|---------------------|
| **Excel Daily Toolkit** | Quick CAGR, % change, EMI utilities |
| **Schema Profiler** | Missingness, type, and format scan |
| **Duplicate Entity Resolver** | Fuzzy matching for duplicates |
| **Outlier Detector** | Z-score and IQR outlier flags |
| **Date/Amount Sanitizer** | Fix date formats and sign flips |
| **Currency/Unit Normalizer** | Normalize units and FX rates |
| **Master Data Diff Tool** | Diff two masters and highlight changes |
| **CAGR Calculator** | Compound annual growth rate |
| **IRR Calculator** | Internal rate of return |
| **NPV Calculator** | Net present value of cash flows |
| **Date Calculator** | Date difference and add/subtract |
| **Percentage Change Calculator** | % change between two values |
| **Weighted Average Calculator** | Compute weighted average |
| **CSV Schema Validator** | Validate CSV against schema |
| **Amount Normalizer** | Convert lakhs/crores to numbers |
| **Date Standardizer** | Standardize date formats |
| **Unit Converter** | Convert units (lakhs, crores, etc) |
| **XIRR Calculator** | IRR for irregular cash flows with dates |

#### Detailed Descriptions

**CAGR Calculator**: Enter start value, end value, years; compute CAGR. Calculates compound annual growth rate between two values.

**IRR Calculator**: Enter cash flows; compute IRR. Calculates internal rate of return for a series of regular cash flows.

**NPV Calculator**: Enter discount rate, cash flows; compute NPV. Calculates net present value at given discount rate.

**Date Calculator**: Compute days between dates or add days to date. Calculates date differences and adds/subtracts days from dates.

**XIRR Calculator**: Enter dates and cash flows; compute XIRR. Calculates IRR for irregular cash flows with specific dates using Newton-Raphson method.

**Outlier Detector**: Upload numeric columns; pick method and threshold. Identifies outliers using Z-score or IQR method with configurable thresholds.

**Amount Normalizer**: Enter amounts in various formats; normalize. Converts lakhs, crores, millions to numeric values.

**Unit Converter**: Enter value, from unit, to unit; convert. Converts between lakhs, crores, millions, billions, etc.

---

### Underwriting & Policy

| Tool | One-Line Description |
|------|---------------------|
| **Policy Matrix Validator** | Rules vs portfolio hit-rate |
| **Thin File Surrogate Score** | Alternate data weights for thin files |
| **Bureau Score Cutoff Optimizer** | Cutoff vs approval and loss trade-off |
| **Income Surrogate Uplift Analyzer** | Incremental approvals from surrogate income |

#### Detailed Descriptions

**Policy Matrix Validator**: Upload rules and portfolio; see pass/fail % and overrides. Tests credit policy rules against actual portfolio to measure effectiveness.

**Thin File Surrogate Score**: Enter bureau flags, bank statements, device signals. Creates surrogate score for thin-file customers using alternate data.

**Bureau Score Cutoff Optimizer**: Upload score vs loss; get KS/Gini and max profit. Determines optimal bureau score cutoff balancing approval rate and loss.

**Income Surrogate Uplift Analyzer**: Upload declared vs surrogate income; see lift. Quantifies incremental approvals from using surrogate income estimation.

---

## Installation

No installation required. Simply open `thousandapps.html` in any modern web browser (Chrome, Firefox, Edge, Safari).

## Data Storage

- **IndexedDB**: Tool states and CSV datasets (persistent across sessions)
- **LocalStorage**: User preferences, favorites, recent tools
- All data stored locally in your browser - nothing is sent to any server.

## Export/Backup

Use the backup feature to export all saved data as JSON. Import backups to restore your saved tool states.

---

*Generated for NBFC Quant Toolbox v1.0*
