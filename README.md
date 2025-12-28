# Indian-Banking-Sector-Market-Risk-Analysis-Monte-Carlo-VaR-
A quantitative risk assessment of India’s "Big Five" banks (HDFC, SBI, ICICI, Kotak, Axis) using Value at Risk (VaR) and Expected Shortfall (ES). This project explores the systemic stability of the banking sector in 2025 and validates a Monte Carlo model through historical backtesting.

Key Features
-Monte Carlo Simulation: Generated 10,000 potential future paths using Cholesky Decomposition to preserve historical correlations between banks.
-Risk Metrics: Calculated 95% VaR and Conditional VaR (Expected Shortfall) to understand both the boundary of loss and the severity of tail events.
-Backtesting: Validated the model against 246 trading days of 2025 data, achieving a 3.25% exception rate (within the Basel "Green Zone").
-Automation: Integrated yfinance for automated data pulls of NSE-listed banking tickers.

Methodology
-Log Returns: Utilized logarithmic returns for time-additivity and statistical stability.
-Covariance Matrix: Modeled the interdependence of private and public sector banks.
-Monte Carlo Engine: Simulated portfolio returns to capture "Fat Tail" risks that simple parametric models often miss.

Results & Interpretation
-Daily VaR (95%): -1.61% (Max likely loss of ₹16,100 on ₹10L investment).
-Expected Shortfall: -2.04% (Average loss during extreme market shocks).

Model Performance: The model recorded only 8 breaches in 2025, proving it to be a reliable and conservative risk estimator for the sector.

Libraries Used
-Pandas
-numpy
-Matplotlib/Seaborn 
-yfinance 
