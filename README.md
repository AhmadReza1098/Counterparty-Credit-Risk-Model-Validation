# 🧮 credit-risk-capital-ifrs9-stress-testing

Simulating wholesale credit risk capital and expected credit loss using **Python**, with Basel III Pillar‑I, CCAR‑style stress testing, IFRS‑9 ECL, and internal severe stress on a synthetic 1,000‑obligor portfolio. [file:2]

---

## 📌 Table of Contents

- [Overview](#overview)  
- [Problem Statement](#problem-statement)  
- [Dataset](#dataset)  
- [Tools & Technologies](#tools--technologies)  
- [Project Structure](#project-structure)  
- [Modeling & Calculations](#modeling--calculations)  
- [Exploratory Analysis & Visuals](#exploratory-analysis--visuals)  
- [How to Run This Project](#how-to-run-this-project)  
- [Future Enhancements](#future-enhancements)  
- [Author & Contact](#author--contact)  

---

## Overview

This project builds a **synthetic wholesale credit portfolio** of 1,000 counterparties and applies multiple risk frameworks to each exposure: Basel III Pillar‑I capital, CCAR‑style regulatory stress, IFRS‑9 expected credit loss, and an internal severe stress scenario. The aim is to demonstrate how capital and expected losses change under different stress assumptions and which segments (industry, country, rating) are most sensitive. [file:2]

---

## Problem Statement

Banks and lending institutions need to understand how their wholesale credit portfolios behave under both regulatory and internal stress scenarios, and how this translates into capital requirements and expected credit losses. This project aims to design a synthetic 1,000‑obligor portfolio and build an end‑to‑end framework that: 
- (1) calculates Basel III Pillar‑I regulatory capital, 
- (2) quantifies capital impact under CCAR‑style and severe internal stress tests, and 
- (3) estimates IFRS‑9 lifetime expected credit losses at counterparty and segment level, in order to compare baseline vs stressed risk measures and identify segments that drive the largest capital and loss sensitivity. [file:2]

---

## Dataset

- Source: Fully synthetic, generated in Python (no real customer data). [file:2]  
- Portfolio size: 1,000 counterparties (`CounterpartyID` 1–1000). [file:2]

Key columns:

- `CounterpartyID` – Unique ID per obligor. [file:2]  
- `EAD` – Exposure at Default (continuous, 1e6–1e9). [file:2]  
- `PD` – Probability of Default (1%–20%). [file:2]  
- `LGD` – Loss Given Default (20%–80%). [file:2]  
- `Industry` – Banking & Financial Services, Manufacturing, Services, Retail, Technology, Energy & Utilities, Real Estate & Construction. [file:2]  
- `Country` – US, UK, Germany, France, Switzerland, China, South Korea. [file:2]  
- `Rating` – AAA, AA, A, BBB, BB, B, CCC, CC, C, D. [file:2]

Derived risk measures:

- `Pillar_I_Capital_Requirement` – Basel III Pillar‑I capital. [file:2]  
- `Stressed_PD`, `Stressed_LGD`, `Capital_Requirement_CCAR` – CCAR stress capital. [file:2]  
- `Expected_Credit_Loss_IFRS9` – IFRS‑9 ECL. [file:2]  
- `Stressed_PD_Internal`, `Stressed_LGD_Internal`, `Capital_Requirement_Internal_Stress_Test` – internal severe stress capital. [file:2]  
- `Perc_Increase_Baseline_to_Severe` – % increase from Pillar‑I to internal severe stress. [file:2]

---

## Tools & Technologies

- **Python (pandas, numpy)** – Data simulation and risk calculations. [file:2]  
- **Jupyter Notebook** – Interactive analysis and visualization. [file:2]  
- **Matplotlib / Seaborn** – Charts for portfolio and risk metrics. [file:2]  
- **GitHub** – Version control and project documentation. [file:1]

---

## Project Structure

# 🧮 credit-risk-capital-ifrs9-stress-testing

Simulating wholesale credit risk capital and expected credit loss using **Python**, with Basel III Pillar‑I, CCAR‑style stress testing, IFRS‑9 ECL, and internal severe stress on a synthetic 1,000‑obligor portfolio. [file:2]

---

## 📌 Table of Contents

- [Overview](#overview)  
- [Problem Statement](#problem-statement)  
- [Dataset](#dataset)  
- [Tools & Technologies](#tools--technologies)  
- [Project Structure](#project-structure)  
- [Modeling & Calculations](#modeling--calculations)  
- [Exploratory Analysis & Visuals](#exploratory-analysis--visuals)  
- [How to Run This Project](#how-to-run-this-project)  
- [Future Enhancements](#future-enhancements)  
- [Author & Contact](#author--contact)  

---

## Overview

This project builds a **synthetic wholesale credit portfolio** of 1,000 counterparties and applies multiple risk frameworks to each exposure: Basel III Pillar‑I capital, CCAR‑style regulatory stress, IFRS‑9 expected credit loss, and an internal severe stress scenario. The aim is to demonstrate how capital and expected losses change under different stress assumptions and which segments (industry, country, rating) are most sensitive. [file:2]

---

## Problem Statement

Banks and lending institutions need to understand how their wholesale credit portfolios behave under both regulatory and internal stress scenarios, and how this translates into capital requirements and expected credit losses. This project aims to design a synthetic 1,000‑obligor portfolio and build an end‑to‑end framework that: (1) calculates Basel III Pillar‑I regulatory capital, (2) quantifies capital impact under CCAR‑style and severe internal stress tests, and (3) estimates IFRS‑9 lifetime expected credit losses at counterparty and segment level, in order to compare baseline vs stressed risk measures and identify segments that drive the largest capital and loss sensitivity. [file:2]

---

## Dataset

- Source: Fully synthetic, generated in Python (no real customer data). [file:2]  
- Portfolio size: 1,000 counterparties (`CounterpartyID` 1–1000). [file:2]

Key columns:

- `CounterpartyID` – Unique ID per obligor. [file:2]  
- `EAD` – Exposure at Default (continuous, 1e6–1e9). [file:2]  
- `PD` – Probability of Default (1%–20%). [file:2]  
- `LGD` – Loss Given Default (20%–80%). [file:2]  
- `Industry` – Banking & Financial Services, Manufacturing, Services, Retail, Technology, Energy & Utilities, Real Estate & Construction. [file:2]  
- `Country` – US, UK, Germany, France, Switzerland, China, South Korea. [file:2]  
- `Rating` – AAA, AA, A, BBB, BB, B, CCC, CC, C, D. [file:2]

Derived risk measures:

- `Pillar_I_Capital_Requirement` – Basel III Pillar‑I capital. [file:2]  
- `Stressed_PD`, `Stressed_LGD`, `Capital_Requirement_CCAR` – CCAR stress capital. [file:2]  
- `Expected_Credit_Loss_IFRS9` – IFRS‑9 ECL. [file:2]  
- `Stressed_PD_Internal`, `Stressed_LGD_Internal`, `Capital_Requirement_Internal_Stress_Test` – internal severe stress capital. [file:2]  
- `Perc_Increase_Baseline_to_Severe` – % increase from Pillar‑I to internal severe stress. [file:2]

---

## Tools & Technologies

- **Python (pandas, numpy)** – Data simulation and risk calculations. [file:2]  
- **Jupyter Notebook** – Interactive analysis and visualization. [file:2]  
- **Matplotlib / Seaborn** – Charts for portfolio and risk metrics. [file:2]  
- **GitHub** – Version control and project documentation. [file:1]

---

## Project Structure

# 🧮 credit-risk-capital-ifrs9-stress-testing

Simulating wholesale credit risk capital and expected credit loss using **Python**, with Basel III Pillar‑I, CCAR‑style stress testing, IFRS‑9 ECL, and internal severe stress on a synthetic 1,000‑obligor portfolio. [file:2]

---

## 📌 Table of Contents

- [Overview](#overview)  
- [Problem Statement](#problem-statement)  
- [Dataset](#dataset)  
- [Tools & Technologies](#tools--technologies)  
- [Project Structure](#project-structure)  
- [Modeling & Calculations](#modeling--calculations)  
- [Exploratory Analysis & Visuals](#exploratory-analysis--visuals)  
- [How to Run This Project](#how-to-run-this-project)  
- [Future Enhancements](#future-enhancements)  
- [Author & Contact](#author--contact)  

---

## Overview

This project builds a **synthetic wholesale credit portfolio** of 1,000 counterparties and applies multiple risk frameworks to each exposure: Basel III Pillar‑I capital, CCAR‑style regulatory stress, IFRS‑9 expected credit loss, and an internal severe stress scenario. The aim is to demonstrate how capital and expected losses change under different stress assumptions and which segments (industry, country, rating) are most sensitive. [file:2]

---

## Problem Statement

Banks and lending institutions need to understand how their wholesale credit portfolios behave under both regulatory and internal stress scenarios, and how this translates into capital requirements and expected credit losses. This project aims to design a synthetic 1,000‑obligor portfolio and build an end‑to‑end framework that: (1) calculates Basel III Pillar‑I regulatory capital, (2) quantifies capital impact under CCAR‑style and severe internal stress tests, and (3) estimates IFRS‑9 lifetime expected credit losses at counterparty and segment level, in order to compare baseline vs stressed risk measures and identify segments that drive the largest capital and loss sensitivity. [file:2]

---

## Dataset

- Source: Fully synthetic, generated in Python (no real customer data). [file:2]  
- Portfolio size: 1,000 counterparties (`CounterpartyID` 1–1000). [file:2]

Key columns:

- `CounterpartyID` – Unique ID per obligor. [file:2]  
- `EAD` – Exposure at Default (continuous, 1e6–1e9). [file:2]  
- `PD` – Probability of Default (1%–20%). [file:2]  
- `LGD` – Loss Given Default (20%–80%). [file:2]  
- `Industry` – Banking & Financial Services, Manufacturing, Services, Retail, Technology, Energy & Utilities, Real Estate & Construction. [file:2]  
- `Country` – US, UK, Germany, France, Switzerland, China, South Korea. [file:2]  
- `Rating` – AAA, AA, A, BBB, BB, B, CCC, CC, C, D. [file:2]

Derived risk measures:

- `Pillar_I_Capital_Requirement` – Basel III Pillar‑I capital. [file:2]  
- `Stressed_PD`, `Stressed_LGD`, `Capital_Requirement_CCAR` – CCAR stress capital. [file:2]  
- `Expected_Credit_Loss_IFRS9` – IFRS‑9 ECL. [file:2]  
- `Stressed_PD_Internal`, `Stressed_LGD_Internal`, `Capital_Requirement_Internal_Stress_Test` – internal severe stress capital. [file:2]  
- `Perc_Increase_Baseline_to_Severe` – % increase from Pillar‑I to internal severe stress. [file:2]

---

## Tools & Technologies

- **Python (pandas, numpy)** – Data simulation and risk calculations. [file:2]  
- **Jupyter Notebook** – Interactive analysis and visualization. [file:2]  
- **Matplotlib / Seaborn** – Charts for portfolio and risk metrics. [file:2]  
- **GitHub** – Version control and project documentation. [file:1]

---

## Project Structure


credit-risk-capital-ifrs9-stress-testing/
│
├── README.md                        # Project documentation
│
├── notebook/                        # Jupyter notebook(s)
│   └── credit_risk_capital_ifrs9.ipynb
│
├── scripts/                         # Reusable Python scripts
│   ├── generate_portfolio.py        # creates synthetic EAD/PD/LGD + categories
│   ├── calculate_capital_ifrs9.py   # Pillar I, CCAR, IFRS‑9 ECL, internal stress, severity
│   └── summarize_results.py         # segment-level summaries (industry, rating, country)
│
├── images/                          # Plots and charts
│   ├── avg_ead_by_industry.png
│   └── pd_distribution_by_rating.png
│
└── output/                          # Model outputs
    └── credit_risk_model_data.csv   # final enriched dataset


This structure mirrors common patterns used in risk modeling and analytics portfolio projects: clean separation of notebooks, scripts, outputs, and visuals. [file:2]

---

## Modeling & Calculations

Main modeling steps performed in Python: [file:2]

- **Portfolio generation**  
  - Simulate EAD, PD, LGD with `numpy`.  
  - Randomly assign `Industry`, `Country`, and `Rating` from predefined lists.  
  - Implemented in `scripts/generate_portfolio.py`.  

- **Basel III Pillar‑I capital**  
  - Formula per counterparty:  
    \[
    \text{Capital}_\text{Pillar I}
    =
    \text{EAD} \times \text{PD} \times \text{LGD} \times 12.5
    \]
  - Implemented in `add_pillar1_capital(df)` inside `calculate_capital_ifrs9.py`.  

- **CCAR stress scenario**  
  - `Stressed_PD = PD × 1.5` (50% increase).  
  - `Stressed_LGD = LGD × 1.2` (20% increase).  
  - \[
    \text{Capital}_\text{CCAR}
    =
    \text{EAD} \times \text{Stressed_PD} \times \text{Stressed_LGD} \times 12.5
    \]
  - Implemented in `add_ccar_stress(df)`.  

- **IFRS‑9 Expected Credit Loss**  
  - \[
    \text{ECL}_\text{IFRS9} = \text{EAD} \times \text{PD} \times \text{LGD}
    \]
  - Implemented in `add_ifrs9_ecl(df)`.  

- **Internal severe stress**  
  - `Stressed_PD_Internal = PD × 2.0` (100% increase).  
  - `Stressed_LGD_Internal = LGD × 1.5` (50% increase).  
  - \[
    \text{Capital}_\text{Internal}
    =
    \text{EAD} \times \text{Stressed_PD_Internal} \times \text{Stressed_LGD_Internal} \times 12.5
    \]
  - Severity metric:  
    \[
    \text{Perc\_Increase\_Baseline\_to\_Severe}
    =
    \frac{\text{Capital}_\text{Internal} - \text{Capital}_\text{Pillar I}}
    {\text{Capital}_\text{Pillar I}} \times 100
    \]
  - Implemented in `add_internal_stress(df)` and `add_severity_metrics(df)`.  

- **Segment summaries**  
  - Group by `Industry`, `Rating`, and `Country` to aggregate EAD, capital, and ECL.  
  - Implemented in `summarize_results.py`.  

[file:2]

---

## Exploratory Analysis & Visuals

Using the enriched dataset (`output/credit_risk_model_data.csv`), the notebook explores: [file:2]

- Distribution of **EAD** by industry and rating.  
- Basel, CCAR, internal capital, and IFRS‑9 ECL by segment.  
- Percentage increase in capital from baseline to internal severe stress.

Key plots (saved in `images/`):

- `avg_ead_by_industry.png` – Average EAD by industry, highlighting sectors that dominate exposure and capital.  
- `pd_distribution_by_rating.png` – PD distribution across ratings, showing higher default risk for lower ratings (BB, B, CCC, etc.).  

[file:2]

---

## How to Run This Project

1. **Open the project folder**
2. **Install dependencies**

3. **Run the notebook**

- Open: `notebook/credit_risk_capital_ifrs9.ipynb`.  
- Run all cells to:  
  - Generate the synthetic portfolio.  
  - Add Pillar‑I, CCAR, IFRS‑9, and internal stress metrics.  
  - Export `output/credit_risk_model_data.csv`.  
  - Save charts into `images/`.  

[file:2]

---

## Future Enhancements

- Add rating‑based PD/LGD curves calibrated to external benchmarks.  
- Implement multi‑period IFRS‑9 staging (Stage 1 vs Stage 2/3).  
- Introduce macroeconomic scenario‑driven PD/LGD instead of fixed multipliers.  
- Build a dashboard (Power BI / Streamlit) for interactive exploration of capital and ECL by segment.  

[file:2]

---

## Author & Contact

**Ahmad Reza**  
Economics Postgraduate · Data Analysis & Credit Risk Modeling Enthusiast  

- 📧 Email: [ahmadreza6122@gmail.com](mailto:ahmadreza6122@gmail.com)  
- 🔗 LinkedIn: [www.linkedin.com/in/ahmad-reza-econ](https://www.linkedin.com/in/ahmad-reza-econ)  
- 🔗 GitHub: [https://github.com/AhmadReza1098](https://github.com/AhmadReza1098)  

[file:1]



