# IFRS 9 Credit Risk Modelling - Week 6
## Macroeconomic Variables and Economic Framework

![Badge](https://img.shields.io/badge/Course-IFRS9%20Credit%20Risk-blue)
![Badge](https://img.shields.io/badge/Week-6-orange)
![Badge](https://img.shields.io/badge/Level-Intermediate-green)
![Badge](https://img.shields.io/badge/Focus-Macro%20Economics-success)

---

## 📚 Week 6 Overview

This week bridges the gap between **macroeconomic theory** and **credit risk modeling**. Understanding how GDP, interest rates, inflation, and employment affect borrower behavior is essential for building forward-looking Probability of Default (PD) models compliant with IFRS 9.

### Core Learning Theme
**"From Central Bank Decisions to Default Behavior"** - How do macro policies eventually cause defaults?

---

## 🎯 Learning Objectives

After completing Week 6, you will:

✅ Understand the **differences between GDP, GNP, and NNP**
✅ Recognize why **real values matter more than nominal** in credit modeling
✅ Explain the **product markets framework** and aggregate demand components
✅ Trace the **causal chain** from interest rates to default rates
✅ Understand **savings-investment equilibrium** and interest rate determination
✅ Apply the **inflation-unemployment tradeoff** to credit risk decisions
✅ Recognize the **paradox of thrift** and its impact on defaults
✅ Identify and mitigate **adverse selection** through risk-based pricing
✅ Build **forward-looking PD scenarios** incorporating macroeconomic variables

---

## 📁 Materials Included

### 1. **IFRS9_Week6_Macroeconomic_Variables_and_Framework.docx**
**40+ pages of detailed learning notes covering:**

| Section | Content |
|---------|---------|
| 1 | From Historical to Forward-Looking PD |
| 2 | Core Macroeconomic Measures (GDP, GNP, NNP) |
| 3 | Real vs. Nominal Values & Price Adjustments |
| 4 | Product Markets Framework |
| 5 | Interest Rate Mechanism |
| 6 | Savings & Investment Equilibrium |
| 7 | Inflation-Unemployment Tradeoff (Phillips Curve) |
| 8 | The Paradox of Thrift |
| 9 | Adverse Selection & Risk-Based Pricing |
| 10 | Linking Macro Variables to PD Models |
| + | Glossary & Appendix |

**Format:** Professional, beginner-friendly, heavy use of analogies
**Tone:** Conversational but technical
**Length:** ~25,000 words

---

### 2. **IFRS9_Week6_Excel_Workbook.xlsx**
**10 interactive worksheets with practical examples:**

| Sheet | Purpose |
|-------|---------|
| **Macro Measures** | Compare GDP vs GNP vs NNP with real examples |
| **Product Markets** | Understand aggregate demand calculation |
| **Interest Rate Impact** | See how RBI repo rate changes cascade through economy |
| **Savings-Investment** | Visualize equilibrium interest rate determination |
| **Phillips Curve** | Explore inflation-unemployment tradeoff |
| **Paradox of Thrift** | Numerical example of savings paradox effect |
| **Adverse Selection** | Compare pricing strategies and portfolio quality |
| **Real vs Nominal** | Calculate real NNP adjustments for inflation |
| **Forward-Looking PD** | Build scenario-weighted PD model |
| **Segment Analysis** | See macro sensitivity differences across borrower types |

**Features:**
- Real banking calculations and scenarios
- Ready-to-use formulas
- Can be customized for your portfolio
- Color-coded for easy reading

---

## 💡 Key Concepts Summary

### GDP vs GNP vs NNP
```
GDP = Economic output within geographic boundaries
GNP = GDP + Net Income from Abroad (includes remittances)
NNP = GNP - Depreciation (sustainable income)

For credit risk modeling: Use Real NNP growth
```

### The Interest Rate Chain
```
RBI raises Repo Rate
         ↓
Banks raise Lending Rates
         ↓
Businesses reduce Investment
         ↓
Employment declines
         ↓
Default Rates increase (lagged 2-3 quarters)
```

### Aggregate Demand Components
```
AD = C + I + G

Where:
- C (Consumption) = Function of income
- I (Investment) = Function of interest rates (negative correlation)
- G (Government) = Policy variable (fixed in models)
```

### Real vs. Nominal (Critical!)
```
TRAP: 10% nominal NNP growth + 10% inflation = 0% REAL growth
      But if modeler uses nominal, they overestimate repayment capacity!

CORRECT: Always deflate by CPI to get real growth
         Real NNP = Nominal NNP ÷ (CPI/100)
```

### The Paradox of Thrift
```
Individual behavior (save more) = Rational
Aggregate behavior (all save more) = Irrational
         ↓
Less spending → Less sales → Less investment
         ↓
Recession despite abundant savings in banks!
```

---

## 📊 What You'll Learn: Real Examples

### Example 1: How Interest Rates Affect Defaults
**Scenario:** RBI raises repo rate from 4% to 8%

**Timeline:**
- **Q1:** Banks raise lending rates; corporates still invest; no change
- **Q2-Q3:** Investment declines 20%; fewer jobs created
- **Q4:** Unemployment begins to rise
- **Q1 (next year):** Retail defaults spike; corporate stress increases
- **Q2 (next year):** SME defaults surge (hardest hit)

**Learning:** Monetary policy effects are lagged and amplified

---

### Example 2: Real vs. Nominal Trap
**Company reports:**
- Nominal revenue growth: +12%
- Inflation (CPI): +12%
- **Real revenue growth: 0%**

**What this means:**
- Looks good nominally but company isn't actually growing
- Profit margins haven't improved
- Repayment capacity hasn't improved
- Default risk hasn't changed despite positive-looking numbers

**Modeler's mistake:** Using nominal growth overestimates borrower health

---

### Example 3: Risk-Based Pricing
**Bank lending at single rate (18%):**
- Only desperate/risky borrowers apply
- Default rate: 10%+
- Bank loses money

**Bank lending with risk-based pricing:**
- Safe companies borrow at 8% (abundant); Default 0.5%
- SMEs borrow at 12% (good volume); Default 2.5%
- Risky borrow at 16% (some); Default 5%
- Weighted portfolio Default: 2-3%
- Bank makes profit!

**Learning:** Pricing impacts borrower selection which impacts defaults

---

## 🔄 How Week 6 Connects to Other Weeks

### Prerequisite Knowledge (Weeks 1-5)
- IFRS 9 ECL framework ✓
- PD, LGD, EAD concepts ✓
- Point-in-time vs. through-the-cycle ✓
- Basic macro variables ✓

### This Week (Week 6)
- **Deep dive into macro mechanisms**
- **How macro variables quantitatively affect PD**
- **Building forward-looking PD models**

### Next Week (Week 7)
- Unemployment rate modeling
- Sector-specific sensitivities
- Econometric implementation

---

## 📈 Practical Application: Building Your Own Model

### Step 1: Gather Macro Forecasts
```
Source: RBI forecasts, economist consensus
Variables: Real NNP growth, interest rates, unemployment, CPI
Frequency: Update quarterly
```

### Step 2: Determine Sensitivities
```
For your portfolio: How sensitive is PD to each variable?
Regression analysis on historical data
Example: 1% GDP growth decrease → 0.3% PD increase
```

### Step 3: Create Scenarios
```
Pessimistic: Real growth -2%, Rates 8%, Unemployment 7%
Base Case:   Real growth 5%, Rates 6.5%, Unemployment 5%
Optimistic:  Real growth 8%, Rates 5%, Unemployment 3.5%
```

### Step 4: Calculate Scenario PDs
```
Adjusted PD = TTC PD × Macro adjustment factor
Macro adjustment = f(Real NNP growth, Interest rates, etc.)
```

### Step 5: Weight by Probability
```
Forward-looking PD = 20% × Pessimistic PD 
                   + 60% × Base PD 
                   + 20% × Optimistic PD
```

---

## 🚨 Common Mistakes to Avoid

| Mistake | Why It's Wrong | Impact |
|---------|---------------|---------
| Using nominal values | Inflation masks real economic conditions | Overestimate repayment capacity |
| Ignoring interest rate lags | Effects take 2-3 quarters to show | Miss early warning signals |
| One PD for all segments | Retail, SME, corporate react differently | Mismeasure risk by segment |
| Forgetting paradox of thrift | High savings can trigger recession | Underestimate downside PD |
| Charging uniform high rates | Only bad borrowers apply | Portfolio quality deteriorates |
| Using GDP not NNP | Doesn't account for depreciation | Overstates sustainable income |

---

## 💼 CIB Banking Application

### For Corporate Banking
- Monitor GDP growth and industrial output
- Track interest rate trajectory (affects pricing negotiations)
- Assess leverage risk during high-rate environments
- Diversify across sectors (differential macro sensitivities)

### For SME Banking
- Most vulnerable to rate hikes (less borrowing capacity)
- Watch unemployment carefully (drives defaults)
- Consider government support programs (RBI priority sectors)
- Tighter risk-based pricing controls essential


---

## ✨ Key Formulas

### Real Value Calculation
```
Real Value = Nominal Value ÷ (CPI Index / 100)
```

### Investment Function
```
I = Ī - c×R

Where:
I = Investment
Ī = Autonomous investment
c = Sensitivity coefficient
R = Interest rate
```

### Consumption Function
```
C = a + b×Y

Where:
C = Consumption
a = Autonomous consumption
b = Marginal propensity to consume
Y = Income
```

### Savings Function
```
S = -a + (1-b)×Y

Where:
S = Savings
(1-b) = Marginal propensity to save
```

---

## 🎓 Discussion Questions

1. **Why is Real NNP more important than GDP for credit modeling?**
   
2. **Trace the full chain from "RBI raises repo rate" to "retail defaults increase."**
   
3. **In the paradox of thrift, why do banks have deposits but can't lend?**
   
4. **Why does risk-based pricing solve the adverse selection problem?**
   
5. **How would you adjust PD differently for corporates vs. SMEs during a rate hike?**

---

## 📚 External Resources

### RBI Documents
- [RBI Monetary Policy Framework](https://www.rbi.org.in)
- [RBI Financial Stability Reports](https://www.rbi.org.in)
- [Credit Risk Management Guidelines](https://www.rbi.org.in)

### Economic Data
- [Ministry of Statistics GDP data](https://mospi.gov.in)
- [CEIC India Economic Database](https://www.ceicdata.com)
- [IMF World Economic Database](https://www.imf.org)

### Academic References
- Keynes, J. M. (1936) - "The General Theory" (original macro framework)
- Mishkin, F. S. - "Economics of Money, Banking, and Financial Markets"
- Saunders & Allen - "Credit Risk Measurement"
