# Factor Models and Technology Stocks During the AI Boom

## Overview
This project analyzes how the explanatory power of the **Fama–French Five-Factor Model** changed for major U.S. technology stocks during the speculative AI boom. Focusing on two distinct periods—**pre-AI boom (2021–2022)** and **AI boom (2023–2024)**—the analysis evaluates whether traditional risk factors, particularly the market excess return (**Mkt–Rf**), became more or less influential as AI-driven optimism reshaped investor behavior.

Rather than testing asset-pricing theory in the abstract, the project examines **how technological speculation alters established risk–return relationships** in practice.

---

## Research Questions
1. **Which Fama–French factors significantly explain daily returns of leading technology companies over the full sample period (2021–2024)?**
2. **Did technology stocks become more or less sensitive to market-wide movements (Mkt–Rf) during the AI boom compared to the pre-AI period?**
3. **Were AI-focused firms affected differently from general technology companies?**

---

## Data
- **Stock Returns:** Daily returns for seven large-cap U.S. technology companies, including both AI-focused and general tech firms (e.g., Microsoft, IBM)
- **Risk Factors:** Fama–French Five Factors (Mkt–Rf, SMB, HML, RMW, CMA)
- **Time Periods:**
  - Pre-AI boom: 2021–2022  
  - AI boom: 2023–2024  

All datasets were merged and aligned at the daily frequency.

---

## Methodology

### Statement 1: Factor Significance Over the Full Period
To identify which Fama–French factors significantly explain technology stock returns over the full sample, we estimated a multivariate OLS regression:

- Dependent variable: Daily stock returns  
- Independent variables: Mkt–Rf, SMB, HML, RMW, CMA  

Hypotheses were tested using standard coefficient significance tests (p < 0.05). This step establishes a baseline understanding of which risk factors are most relevant for technology stocks across the entire period.

---

### Statement 2: Market Sensitivity Before vs. During the AI Boom
Given that Mkt–Rf exhibited the strongest explanatory power, we then examined whether technology stocks’ sensitivity to market-wide risk changed across regimes.

- Compared two one-year windows (2021–22 vs. 2023–24)
- Estimated changes in responsiveness to Mkt–Rf
- Used hypothesis testing (Z-tests and p-values) to assess whether differences were statistically significant
- Visualized changes in sensitivity over time to isolate regime effects

This approach allows changes in factor influence to be attributed to market conditions rather than seasonal variation.

---

## Key Findings
- Market excess return (Mkt–Rf) is the dominant factor explaining daily returns for large-cap technology stocks
- During the AI boom, the correlation between Mkt–Rf and stock returns declines significantly**
- Hypothesis testing confirms that technology stocks’ sensitivity to market-wide movements changed materially between periods
- Results suggest partial decoupling from traditional market risk pricing during periods of intense technological speculation

---

## Interpretation
The decline in market sensitivity during the AI boom is consistent with a shift toward company-specific narratives, innovation expectations, and speculative sentiment, which temporarily reduce reliance on broad market movements.

These findings illustrate how transformative technologies can disrupt established asset-pricing relationships, particularly in innovation-driven sectors.

---

## Limitations
- The analysis does not explicitly control for macroeconomic variables such as inflation, monetary policy, or geopolitical shocks
- The sample is limited to seven large-cap technology firms, which restricts generalizability
- The SMB and RMW factors are difficult to interpret meaningfully due to limited size and profitability variation within the sample
- COVID-19 recovery dynamics overlap with the pre-AI period, complicating causal attribution between pandemic effects and AI-driven market shifts

---

## Conclusion
This project demonstrates that speculative technological booms can materially alter the behavior of traditional financial risk factors. While Mkt–Rf remains central to explaining technology stock returns, its influence weakens during periods of intense innovation-driven optimism.

The results highlight the importance of adapting classical financial models to account for regime shifts, especially in rapidly evolving sectors. Understanding when and why traditional relationships break down is critical for investors, analysts, and policymakers navigating modern financial markets.

---

## Tools
Python · pandas · statsmodels · matplotlib · Fama–French data
