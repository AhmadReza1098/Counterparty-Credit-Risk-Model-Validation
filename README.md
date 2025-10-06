This repository contains code and data related to the development and validation of credit risk models for counterparty credit ratings. The project simulates key credit risk variables such as Exposure at Default (EAD), Probability of Default (PD), and Loss Given Default (LGD) for 1000 synthetic counterparties.
Generation of synthetic counterparts data including industry, country, and credit ratings.
Calculation of regulatory capital requirements under multiple frameworks:
- Basel III Pillar-I
- CCAR stress testing
- IFRS-9 Expected Credit Loss (ECL)
- Internal stress testing scenarios
- Scenario-based stress testing demonstrating capital sensitivity to increases in PD and LGD.
- Analysis of percentage increases in capital needs under moderate and severe economic stress.
- Use of Python, pandas, and numpy for data processing and risk modeling.
- Visualization templates for capital sensitivity and portfolio risk concentration dashboards.

# Regulatory Frameworks

This project follows key regulatory frameworks relevant to credit risk management:

- **Basel I-IV:** International banking regulations focusing on capital adequacy, risk management, and supervisory review.
- **CCAR:** The US Federal Reserve's stress testing framework to evaluate bank capital resilience under adverse economic scenarios.
- **IFRS-9:** International accounting standards requiring banks to measure and recognize expected credit losses.
  
These frameworks guide the capital requirement calculations, stress testing, and loss modeling implemented in this project.
