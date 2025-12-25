# Workers' Compensation Loss Reserving Analysis

## Project Overview
Predictive modeling project for **TOU Insurance Company** to assess unpaid claim reserves for Workers' Compensation. Developed two independent actuarial models to estimate **$2.1M ultimate losses** with **less than 2% variance** between methods.

*Completed for UT Dallas Actuarial Case Competition (Oct–Nov 2025)*

---

## Objective
Estimate unpaid claim liabilities using industry-standard actuarial techniques, providing reliable reserve estimates for financial planning and regulatory compliance.

---
<img width="1244" height="452" alt="image" src="https://github.com/user-attachments/assets/a12bb8ca-64bb-4aea-a7bb-0dc61462253e" />

## Methods

### Method 1: Chain-Ladder Loss Development
- Constructed **paid** and **reported** loss triangles from 10+ years of claims data
- Calculated age-to-age development factors using **volume-weighted averages**
- Applied **exponential decay curve fitting** (1 + Ae^(-λt)) for tail factor estimation
- Adjusted for catastrophe outliers and inflation impacts

### Method 2: Frequency-Severity Approach
- Decomposed losses using: **E[S] = E[N] × E[X]**
  - E[N]: Ultimate claim count
  - E[X]: Ultimate average claim cost
- Developed separate triangles for claim counts and severity
- Applied trend factors to project ultimate values

---

## 🔍 Key Findings

| Metric | Result |
|--------|--------|
| Ultimate Loss Estimate | ~$2.1M |
| Model Variance | <2% between methods |
| Medical Loss Share | 53% of total reserves |
| Medical Growth Rate | Faster than indemnity losses |

### Data Challenges Addressed
- Missing data for years preceding 2010
- Catastrophic event outlier (3 years prior)
- Decreasing reported loss amounts (settlement adjustments)
- Inflation adjustments for indemnity payments

---

## 🛠️ Tools & Technologies
- **Python**: Pandas, NumPy, Matplotlib
- **Excel**: Data processing, triangle construction
- **Statistical Methods**: Curve fitting, weighted averages, trend analysis

---

## Repository Structure
```
├── README.md
├── ACT_competition.ipynb    # Main analysis code
└── data/                    # Loss triangles (if applicable)
```
<img width="2274" height="810" alt="image" src="https://github.com/user-attachments/assets/90c16f43-95ee-4f4c-9557-8595cef0227d" />


---

## Business Impact
- Provides actuarially sound reserve estimates for financial reporting
- Supports regulatory compliance (NAIC requirements)
- Identifies medical cost trends for strategic planning
- Enables sensitivity analysis for risk management decisions

---

## 👤 Author
**Crystal W Li, Melody Tsai, Howard Zhang, Yaohan**  
B.Sc. Statistics & Actuarial Science, University of Toronto  
[LinkedIn](http://linkedin.com/in/crystal-li-baa648351) | [Email](mailto:crystalw.li@mail.utoronto.ca)
