# 📊 Credit Risk & IFRS 9 Learning Journey

This repository documents my structured learning journey in Credit Risk Modeling, IFRS9, and Financial Risk Analytics.

---
## Week 1: IFRS9 Foundations
- Understanding Banking P&L & Balance Sheet
- Role of Provisioning in Banking
- Expected vs Unexpected Loss
- IFRS9 vs Basel (Core Differences)

## Objective
To build deep expertise in Credit Risk, Financial Engineering, and Risk Modeling.

# 📘 Week 2 — IFRS 9 Credit Risk Modelling

This week focuses on understanding how banking portfolios are structured and how IFRS 9 approaches credit risk differently from capital frameworks like Basel.

---

## 🔍 Key Topics Covered

### 1. Banking Portfolio Structure
- Lending book divided into:
  - **Retail Portfolio**
    - Large number of borrowers
    - Small individual exposure
  - **Commercial Portfolio**
    - Fewer borrowers
    - High exposure per borrower

---

### 2. Risk-Based Classification (Basel Perspective)
- Assets classified based on **riskiness**
  - Credit Cards → High Risk (Revolving, Unsecured)
  - Personal Loans → Medium Risk
  - Auto Loans → Lower Risk (Secured)
  - Mortgages → Lowest Risk (Collateralized)

---

### 3. IFRS 9 Perspective (Cash Flow Based)
- Focus is NOT on risk category  
- Focus is on:
  - **Contractual Cash Flows**
  - **SPPI Test (Solely Payments of Principal & Interest)**

---

### 4. Personal Loan Mechanics

#### Characteristics:
- Fixed tenure (e.g., 36–60 months)
- Unsecured loan
- Fixed EMI payments

#### Key Concept:
- Loan = **Intangible Asset** for bank  
- Generates income via **interest cash flows**

---

### 5. Amortization Concept

Loan repayment happens through **EMIs**, consisting of:
- Interest component
- Principal component

#### Key Behavior:
- Initial EMIs → Mostly Interest  
- Later EMIs → Mostly Principal  

---

### 📊 Amortization Formula

\[
EMI = P \times \frac{r(1+r)^n}{(1+r)^n - 1}
\]

Where:
- **P** = Principal  
- **r** = Rate of interest per period  
- **n** = Number of periods  

---

### 6. IFRS 9 Classification Outcome

Personal Loans:
- Pass **SPPI Test**
- Classified under **Amortised Cost**
- Eligible for **ECL (Expected Credit Loss) modelling**

---

## 📉 Expected Credit Loss (ECL)

Two types:

### 1. 12-Month ECL
- For **Stage 1 accounts**
- Low credit risk

### 2. Lifetime ECL
- For **Stage 2 & Stage 3 accounts**
- Higher credit risk or default

---

## 🧭 Staging Concept (Core IFRS 9 Concept)

| Stage | Description | Provision Type |
|------|------------|---------------|
| Stage 1 | Performing (No issues) | 12-month ECL |
| Stage 2 | Credit risk increased (SICR) | Lifetime ECL |
| Stage 3 | Default / Impaired | Lifetime ECL |

---

## ⚠️ Key Trigger

### SICR — Significant Increase in Credit Risk

- Driven by **borrower behavior**
- NOT driven by collateral value changes

Example:
- Missed EMIs → Moves to Stage 2  
- Default → Moves to Stage 3  

---

## 📊 Excel Template Included

The repository includes a working Excel model to simulate:

- Loan inputs (Principal, Rate, Tenure)
- EMI calculation
- Full amortization schedule
- Interest vs Principal breakdown
- Outstanding balance tracking

---

