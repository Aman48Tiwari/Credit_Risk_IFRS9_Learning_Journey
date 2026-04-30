# IFRS 9 Credit Risk Modelling - Week 5
## PD Modelling Framework and Macroeconomic Variables

![Badge](https://img.shields.io/badge/Course-IFRS9%20Credit%20Risk-blue)
![Badge](https://img.shields.io/badge/Week-5-orange)
![Badge](https://img.shields.io/badge/Level-Beginner-green)
![Badge](https://img.shields.io/badge/Updated-2024-success)

---

## 📚 Course Overview

This repository contains comprehensive learning materials for **Week 5** of the IFRS 9 Credit Risk Modelling course. This week focuses on understanding **Probability of Default (PD) Modelling** and how **macroeconomic variables** drive credit risk in a Point-In-Time (PIT) framework.

### Course Structure
- **Week 1-4**: Foundation concepts (ECL, stages, provisioning)
- **Week 5** ← You are here: PD Modelling & Macroeconomic Variables
- **Week 6+**: LGD, EAD, and full implementation

---

## 🎯 Learning Objectives

By the end of Week 5, you will understand:

1. **TTC vs PIT PD** - Why IFRS 9 requires forward-looking probability estimates
2. **Macroeconomic Variables** - How GDP, unemployment, interest rates, and house prices drive defaults
3. **Variable Transformations** - Techniques to prepare macro data for statistical models
4. **PD Model Building** - Practical steps to develop segment-specific default models
5. **Scenario Analysis** - How to forecast PD under different economic conditions
6. **Real-World Implementation** - Case studies and backtesting examples

---

## 📁 Repository Contents

### Core Learning Materials
- **`IFRS9_Week5_PD_Modelling_and_Macroeconomic_Variables.docx`**
  - 40+ pages of detailed theoretical notes
  - Easy-to-understand explanations with examples and analogies
  - Covers all key concepts in logical progression
  - **Best for**: Reading and understanding core concepts

- **`IFRS9_Week5_PD_Modelling_Excel_Workbook.xlsx`**
  - 10 interactive worksheets with practical examples
  - Real banking scenario data and calculations
  - Macro variable analysis and model output
  - **Best for**: Hands-on learning and model building

### Navigation Guide

**For Conceptual Understanding:**
1. Start with Word document: Introduction → TTC vs PIT → Macroeconomic Variables
2. Review practical Excel examples alongside theory

**For Technical Implementation:**
1. Excel Sheet: "Macro Variables" - Understand what each variable means
2. Excel Sheet: "Transformations" - Learn how to prepare data
3. Excel Sheet: "Model Example" - See how logistic regression works
4. Excel Sheet: "Scenarios" - Forecast PD under different conditions

**For Quick Reference:**
- Excel Sheet: "Formulas" - All key equations
- Word Document: Section 9 (Glossary) - Important terms

---

## 🔑 Key Concepts Summary

### 1. Point-In-Time (PIT) vs Through-The-Cycle (TTC) PD

| Aspect | TTC | PIT |
|--------|-----|-----|
| **Timeframe** | 10+ years (historical) | Next 12 months (forward) |
| **Basis** | Historical average defaults | Current conditions + forecasts |
| **Changes Over Time** | Smooth, stable | Volatile with economy |
| **IFRS 9 Use** | ❌ Not compliant | ✅ Required |
| **Example** | 3% (fixed baseline) | 2.1% to 7.5% (scenario-dependent) |

### 2. Core Macroeconomic Variables

**GDP Growth** → Economic expansion → More income → Fewer defaults
- Negative correlation with PD: ↑Growth = ↓Defaults

**Unemployment Rate** → Job losses → Less repayment ability → More defaults
- Positive correlation with PD: ↑Unemployment = ↑Defaults

**Interest Rates** → Higher borrowing costs → Payment stress → More defaults
- Positive correlation with PD: ↑Rates = ↑Defaults (for floating-rate borrowers)

**House Prices** → Collateral value → LGD changes → Risk changes
- Negative correlation with PD: ↑Prices = ↓Risk

### 3. Model Formula

```
PIT PD = TTC PD × Macro Adjustment Factor

where:
TTC PD = Historical baseline (e.g., 3%)
Macro Adjustment Factor = e^(β₁×GDP + β₂×Unemployment + β₃×Rates + ...)
```

**Example Scenario:**
- TTC PD = 3%
- In Base Case: Adjustment = 1.00 → PIT = 3.0%
- In Recession: Adjustment = 1.80 → PIT = 5.4%
- In Boom: Adjustment = 0.70 → PIT = 2.1%

---

## 📊 What's Included in Excel Workbook

### Sheet 1: Macro Variables
Overview of 6 key macroeconomic variables, their definitions, and relationship with defaults.

### Sheet 2: TTC to PIT
Shows how base TTC PD converts to forward-looking PIT PD using adjustment factors.

### Sheet 3: Transformations
Explains how to transform raw macro data (growth rates, standardization, lagging).

### Sheet 4: Model Example
Real small business lending case study with actual correlation coefficients and model parameters.

### Sheet 5: Scenarios
Shows how PIT PD varies from 1.5% (boom) to 7.5% (severe recession).

### Sheet 6: Forward-Looking Indicators
Techniques for forecasting future macro values (surveys, leading indicators, expert opinions).

### Sheet 7: Formulas
Quick reference for all mathematical formulas used in PD modelling.

### Sheet 8: Backtesting
Historical validation showing model predictions vs actual defaults (8 quarters).

### Sheet 9: Segments
Comparison of macro sensitivities across loan types (retail, SME, corporate).

### Sheet 10: Implementation Checklist
15-step checklist for rolling out PD models in your organization.

---

## 💡 Learning Tips

### For Beginners
1. **Don't memorize formulas** - Focus on understanding *why* each variable matters
2. **Use analogies** - Think of PD as "weather forecast" (TTC = historical average, PIT = tomorrow's weather)
3. **Start with scenarios** - See PD change from 2% to 7% helps intuition
4. **Practice with Excel** - Plug in different numbers to see effects

### For Advanced Users
1. **Study model coefficients** - Interpret β values (elasticity of default to macro changes)
2. **Examine lagging effects** - Understand timing: GDP in Q1 affects defaults in Q2-Q3
3. **Validate assumptions** - Check: Are historical correlations stable? Do they break in crises?
4. **Consider non-linearity** - In severe stress, might GDP-PD relationship change?

### For Practitioners
1. **Segment your portfolio** - One-size-fits-all models don't work
2. **Combine expert judgment** - Don't rely only on models; include economist forecasts
3. **Scenario test regularly** - Update quarterly as conditions change
4. **Document everything** - Regulators need transparent, auditable models

---

## 🎓 Key Takeaways

✅ **IFRS 9 requires forward-looking (PIT) PD**, not historical (TTC) PD

✅ **Macroeconomic variables** are the primary drivers of PD variation

✅ **GDP and unemployment** are the strongest predictors for most segments

✅ **Different segments** have different macro sensitivities (customize your models)

✅ **PD can range 2-5x** depending on economic scenario (not just +/-10%)

✅ **Scenario analysis** is essential for understanding portfolio risk

✅ **Regular recalibration** needed as economy evolves and new data arrives

---

## 📈 Real-World Context

### India-Specific Insights
- **RBI Policy Rate**: Currently 6.5% (used in rate sensitivity models)
- **GDP Growth**: 6-8% expected in 2024-25 (improving from 2023)
- **Unemployment**: 4-5% (moderate but rising)
- **Industrial Production**: Growing ~4-5% YoY (weak manufacturing)

**Impact**: In current environment, PD should be near baseline or slightly elevated. Monitor if GDP growth slows below 5%.

---

## 🔗 External Resources

### Official Guidance
- [IFRS 9 Full Text](https://www.ifrs.org) - Official standard
- [RBI Circular on Expected Credit Loss](https://www.rbi.org.in) - Indian implementation
- [Basel III Credit Risk Framework](https://www.bis.org) - Regulatory capital requirements

### Further Reading
- Vasicek, O. (1987) "Probability of Loss on Loan Portfolio"
- Lando, D. (2004) "Credit Risk Modeling: Theory and Applications"
- Gordy, M. (2000) "A Comparative Anatomy of Credit Risk Models"

### Data Sources
- RBI: [RBI Statistical Release](https://www.rbi.org.in)
- Ministry of Statistics: [Official data portal](https://mospi.gov.in)
- World Bank: [World Development Indicators](https://data.worldbank.org)

---

## ❓ Frequently Asked Questions

**Q: Why use PIT instead of TTC?**
A: PIT reflects current conditions so provisions increase when defaults actually rise (during recessions). TTC stays flat, providing no early warning.

**Q: How often should we update PD models?**
A: Quarterly for most segments. More frequently (monthly) for volatile portfolios during stress.

**Q: Can we use just one macro variable?**
A: Not recommended. Use multiple variables to capture different drivers. But avoid multicollinearity.

**Q: What if our historical data is incomplete?**
A: Supplement with industry data, peer benchmarks, or expert judgment. But document and stress-test assumptions.

**Q: How do we forecast macro variables for next 12 months?**
A: Use: (1) Central bank forecasts, (2) Consensus economist surveys, (3) Market-implied forecasts, (4) Your own economic team.

---

## 📝 Glossary (Quick Reference)

- **PD**: Probability of Default - chance borrower won't repay
- **TTC**: Through-The-Cycle - long-term average default rate
- **PIT**: Point-In-Time - forward-looking default rate based on current conditions
- **N12M PD**: Next 12-Month PD - IFRS 9 Stage 1 estimate
- **ECL**: Expected Credit Loss - PD × LGD × EAD
- **LGD**: Loss Given Default - percentage lost if default occurs
- **EAD**: Exposure at Default - amount owed at time of default
- **Macro Adjustment Factor**: Multiplier to convert TTC to PIT
- **Backtesting**: Comparing predicted defaults to actual outcomes
- **Scenario Analysis**: Forecasting PD under different economic conditions

---

## 💬 Discussion & Feedback

**Have questions?** Create an issue in this repository.

**Want to contribute?** Pull requests welcome for:
- Additional case studies
- Alternative modelling approaches
- Updated macro data
- Regional adaptations

---

## 📄 License

These learning materials are provided for educational purposes. For use in commercial implementations, ensure compliance with your organization's policies and regulatory requirements.

---

## 🙏 Acknowledgments

Created for banking professionals learning IFRS 9 credit risk modelling from first principles. All examples use realistic banking scenarios but are illustrative in nature.

---

**Last Updated**: June 2024  
**Course Level**: Beginner to Intermediate  
**Estimated Learning Time**: 6-8 hours  

---

### Quick Start Guide

1. **First time?** Read: Word document → Introduction (Section 1-2)
2. **Want examples?** Open: Excel workbook → Scenarios sheet
3. **Ready to build?** Study: Excel workbook → Model Example sheet
4. **Need formulas?** Check: Excel workbook → Formulas sheet

**🚀 Ready to learn? Start with Section 1 of the Word document!**
