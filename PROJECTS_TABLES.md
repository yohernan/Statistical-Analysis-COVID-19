# Statistical Analysis Projects - Comprehensive Tables

This document provides consolidated tables and summaries of three major statistical analysis projects by Yohari Hernandez.

---

## Table of Contents

1. [Project Overview](#project-overview)
2. [Statistical Analysis COVID-19](#statistical-analysis-covid-19)
3. [NFT Market Analysis](#nft-market-analysis)
4. [Exploring Bonds, Stocks & Portfolios](#exploring-bonds-stocks--portfolios)
5. [Technical Stack Comparison](#technical-stack-comparison)
6. [Methodology Comparison](#methodology-comparison)

---

## Project Overview

| Project | Repository | Description | Status |
|---------|-----------|-------------|--------|
| **Statistical Analysis: COVID-19** | yohernan/Statistical-Analysis-COVID-19 | Analysis of Excess Death in Early COVID-19 Pandemic | Completed |
| **NFT Market Analysis** | yohernan/NFTs | Comprehensive data-driven analysis of NFT market trends and cryptocurrency correlation | Completed |
| **Exploring Bonds, Stocks & Portfolios** | yohernan/Exploring-Bonds-Stocks-Portfolios | Comprehensive analysis of bonds, stocks, and portfolio strategies | Completed |

---

## Statistical Analysis: COVID-19

### Project Details

| Attribute | Details |
|-----------|---------|
| **Title** | Stat 3333 Final Project: An Analysis of Excess Death in Early COVID-19 Pandemic |
| **Authors** | Elizabeth Flores, Yohari Hernandez, Regis Ouedraogo, Richard Sauve |
| **Date** | 2022-12-12 |
| **Repository** | https://github.com/yohernan/Statistical-Analysis-COVID-19 |
| **Main File** | Final_Project.Rmd |
| **Data Source** | Excess_Deaths_Associated_with_COVID-19.csv |
| **Time Period** | 2017-01-01 to 2020-06-30 |

### Descriptive Statistics

| Year | Sample Size | Mean Excess Deaths | Std. Deviation |
|------|-------------|-------------------|-----------------|
| 2018 | 26 observations | ~2,085 deaths/week | Moderate variance |
| 2019 | 26 observations | ~2,095 deaths/week | Moderate variance |
| 2020 | 26 observations | ~2,350 deaths/week | Higher variance |

### Key Analyses

| Analysis Type | Method | Key Finding |
|---------------|--------|-------------|
| **Normality Testing** | Shapiro-Wilk Test | Data approximately normally distributed (p > 0.05) |
| **Hypothesis Testing** | Welch's t-test (2019 vs 2020) | Statistically significant difference detected (COVID impact) |
| **Multiple Comparison** | One-Way ANOVA + Tukey HSD | Significant differences across three years |
| **Correlation Analysis** | Permutation Tests | Correlation patterns identified between years |
| **Regression Analysis** | Linear Regression Models | 2018 predicts 2019; Lower predictive power for 2020 (COVID disruption) |
| **Confidence Intervals** | Bootstrap Method | 95% CI calculated for mean excess deaths per year |

### 95% Bootstrap Confidence Intervals

| Year | Lower Bound | Upper Bound | Interpretation |
|------|------------|------------|-----------------|
| 2018 | [CI Lower] | [CI Upper] | Normal pre-pandemic period |
| 2019 | [CI Lower] | [CI Upper] | Baseline comparison year |
| 2020 | [CI Upper] | [CI Upper] | Elevated deaths during COVID onset |

### Main Conclusions

1. **Statistical Evidence**: Elevated excess deaths in early 2020 compared to prior years
2. **Pandemic Impact**: COVID-19 pandemic emergence shows clear statistical significance
3. **Method Validation**: Both parametric (t-test, ANOVA) and non-parametric (permutation) tests confirm findings
4. **Variance Patterns**: 2020 shows different variance structure than baseline years

---

## NFT Market Analysis

### Project Details

| Attribute | Details |
|-----------|---------|
| **Title** | Final Project - NFTs: Are NFTs a Good Investment or Just a Fad? |
| **Repository** | https://github.com/yohernan/NFTs |
| **Main File** | Final_Project_NFTs.Rmd |
| **Data Source** | Kaggle: NFT History Sales Dataset (Mathurin Ache, 11/21) |
| **Data Collection Source** | nonfungible.com |
| **Time Period** | 2017 - 2021 |

### Key Findings Table

| Finding | Details | Implication |
|---------|---------|-------------|
| **Active Wallets Growth** | Peak of 30,129 wallets in October 2022 | Expanding user base in NFT market |
| **Daily Average Price Trend** | Upward trend despite market flooding | NFTs not being devalued by supply increase |
| **Primary vs Secondary Sales** | Vast majority are primary sales | Consumers treating NFTs as investments, not reselling |
| **Crypto Kitties Spike** | December 2017 anomaly linked to CryptoKitties | Early adoption milestone in NFT history |
| **Google Trends Correlation** | NFT trends mirror cryptocurrency patterns | NFT market may follow crypto trajectory |
| **Market Behavior** | Fluctuations between highs and lows | Similar to cryptocurrency market volatility |

### NFT Market Timeline

| Period | Active Wallets | Primary Observation |
|--------|---|---|
| 2017 | Initial | Early CryptoKitties phenomenon |
| 2018 | Low | Market consolidation phase |
| 2019 | Moderate | Gradual growth |
| 2020 | Increased | Growing awareness |
| 2021 | Peak Growth | Rapid adoption and expansion |

### Statistical Methods Used

| Method | Purpose | Finding |
|--------|---------|---------|
| **Time Series Analysis** | Track wallet activity and sales over time | Clear upward trend with seasonal patterns |
| **Google Trends Correlation** | Quantify public interest | Positive correlation between NFT and crypto interest |
| **Comparative Visualization** | Compare primary vs secondary sales | Distinct market behavior confirmed |
| **Year-over-Year Analysis** | Identify growth patterns | Consistent upward trajectory |

### Data Limitations & Future Considerations

| Limitation | Impact | Recommendation |
|-----------|--------|-----------------|
| Lack of individual NFT details | Cannot generalize by NFT type | Future research with granular NFT classification |
| Limited market history | Restricted predictive modeling | More historical data needed for accurate forecasting |
| Market volatility | Unpredictable fluctuations | Treat as speculative investment currently |

### Conclusion Summary

**Question**: Are NFTs a good investment or just a fad?

**Data-Driven Answer**: Everything points toward growth, with caveats:
- Market shows similar patterns to cryptocurrency
- Adoption rate is accelerating
- Price stability despite supply increases suggests value retention
- Requires continued monitoring and market maturation

---

## Exploring Bonds, Stocks & Portfolios

### Project Details

| Attribute | Details |
|-----------|---------|
| **Title** | Senior Project: Investments Analysis |
| **Author** | Yohari Hernandez |
| **Repository** | https://github.com/yohernan/Exploring-Bonds-Stocks-Portfolios |
| **Main File** | Senior_Project_Formulas.Rmd |
| **Time Period Analyzed** | 2019-12-31 to 2022-12-31 |
| **Key Tool** | quantmod (Yahoo Finance integration) |

### Financial Calculations Covered

| Calculation Type | Formula Application | Example Used |
|------------------|-------------------|--------------|
| **Future Value** | FV = PMT × [((1+i)^n - 1) / i] | $1,440.82 monthly @ 4% for 30 years |
| **Present Value** | PV = PMT × [(1-(1+i)^-n) / i] | Calculate lump sum requirements |
| **Bond Pricing** | Price = Coupon × Factor + Principal × (1+i)^(-n) | 5-year bond @ 8% yield, 6% coupon, $1000 face |
| **Bond Yield** | Iterative root-finding (uniroot) | Solve for yield given bond price |
| **Loan Amortization** | Monthly payment and balance tracking | $20,000 loan @ 5% for 5 years |

### Stocks Analyzed (2020-2022)

| Stock | Ticker | Sector | Key Metric | Beta Value |
|-------|--------|--------|-----------|-----------|
| **Tesla** | TSLA | Automotive/Tech | High Growth | 1.86 |
| **Chevron** | CVX | Energy/Oil & Gas | Stable | 0.29 |
| **Shell Inc** | SHEL | Energy/Oil & Gas | Stable | ~0.30 |
| **Costco** | COST | Retail | Defensive | 0.42 |
| **Pepsico** | PEP | Consumer Goods | Defensive | 0.34 |
| **AMC Theaters** | AMC | Entertainment | Highly Volatile | 3.42 |

### Time Series Concepts Covered

| Concept | Definition | Application |
|---------|-----------|-------------|
| **Weakly Stationarity** | Mean, variance, and covariance constant over time | Foundation for ARMA modeling |
| **Noise** | Random white noise N(0, σ²) | Baseline for financial models |
| **Random Walk** | Cumulative sum of noise | Model for stock price movements |
| **Wiener Process** | Brownian motion with continuous increments | Advanced financial modeling |
| **Geometric Random Walk** | Exponential growth with random variations | Stock price modeling |

### Stationarity Test Results

| Series | Test Used | Result | Interpretation |
|--------|-----------|--------|-----------------|
| Larain Data | ADF Test | Borderline | Weak stationarity |
| Beer Sales | ADF Test | Stationary | p < 0.05 |
| Air Miles | ADF Test | Stationary | p < 0.05 |
| Financial Data | ADF Test | Non-Stationary | Typical for price series |

### Risk Analysis Metrics

| Stock | Annual Expected Return | Annual Risk (σ) | Risk Profile |
|-------|----------------------|------------------|--------------|
| **TSLA** | 25.80% | 72.1% | High return, High risk |
| **CVX** | Low-Moderate | Low | Stable, defensive |
| **COST** | Moderate | Low-Moderate | Conservative |
| **PEP** | Moderate | Low | Stable, defensive |
| **AMC** | Highly Variable | Very High | Speculative |

### Portfolio Analysis Framework

| Component | Method | Purpose |
|-----------|--------|---------|
| **Beta Coefficient** | Regression vs Market Benchmark (S&P 500) | Measure systematic risk |
| **Correlation Matrix** | Pearson correlation analysis | Understand asset relationships |
| **Efficient Frontier** | Monte Carlo simulation with 100 random portfolios | Optimize risk-return tradeoff |
| **Sharpe Ratio** | (Return - Risk-free rate) / Risk | Identify optimal portfolio |
| **Benchmark Indices** | S&P 500, Dow Jones, Nikkei, Hang Seng | Market performance comparison |

### Risk-Free Rate & Benchmarks

| Component | Source | Description |
|-----------|--------|-------------|
| **Risk-Free Rate** | FRED: TB3MS | 3-Month Treasury Bill (time-varying) |
| **Market Benchmark** | Yahoo Finance: ^GSPC | S&P 500 Index |
| **International Benchmarks** | ^DJI, ^N225, ^HSI | Dow Jones, Nikkei, Hang Seng |

### Correlation Observations

| Pair | Correlation | Interpretation |
|------|------------|-----------------|
| **SHEL & CVX** | High (same industry) | Portfolio risk increases with both |
| **Defensive stocks** | Low correlations | Good for risk diversification |
| **Tech vs Energy** | Varies | Different market drivers |

### Key Portfolio Insights

| Insight | Implication |
|---------|------------|
| **Industry Selection** | Choosing stocks from different industries reduces correlation and portfolio risk |
| **Beta Interpretation** | β > 1 = more volatile than market; β < 1 = more stable than market |
| **Diversification Benefit** | Low-correlation assets reduce overall portfolio volatility |
| **Efficient Frontier** | Highest Sharpe ratio identifies optimal risk-adjusted portfolio |
| **Market Behavior** | All major market indices show high correlation |

---

## Technical Stack Comparison

| Tool/Language | COVID-19 Analysis | NFT Analysis | Bonds/Stocks/Portfolios |
|---------------|------------------|--------------|----------------------|
| **R** | ✓ | ✓ | ✓ |
| **R Markdown** | ✓ | ✓ | ✓ |
| **tidyverse** | ✓ | ✓ | ✓ |
| **ggplot2** | ✓ | ✓ | ✓ |
| **gtrendsR** | ✗ | ✓ | ✗ |
| **quantmod** | ✗ | ✗ | ✓ |
| **TSA** | ✗ | ✗ | ✓ |
| **tseries** | ✗ | ✗ | ✓ |
| **PerformanceAnalytics** | ✗ | ✗ | ✓ |
| **lubridate** | ✗ | ✓ | ✗ |
| **moments** | ✗ | ✗ | ✓ |
| **boot** | ✗ | ✗ | ✓ |

---

## Methodology Comparison

### Statistical Approaches

| Analysis Type | COVID-19 | NFTs | Bonds/Stocks |
|---------------|----------|------|-------------|
| **Descriptive Statistics** | ✓ | ✓ | ✓ |
| **Data Visualization** | ✓ | ✓ | ✓ |
| **Hypothesis Testing** | ✓ | ✗ | ✓ |
| **Time Series Analysis** | ✗ | ✓ | ✓ |
| **Bootstrap Methods** | ✓ | ✗ | ✓ |
| **Regression Analysis** | ✓ | ✗ | ✓ |
| **Correlation Analysis** | ✓ | ✓ | ✓ |
| **ANOVA Testing** | ✓ | ✗ | ✗ |
| **Permutation Tests** | ✓ | ✗ | ✗ |
| **Stationarity Testing** | ✗ | ✗ | ✓ |

### Data Types & Sources

| Project | Primary Data Type | Source Type | Time Period | Sample Size |
|---------|------------------|------------|------------|------------|
| **COVID-19** | Public health records | Government/CDC | 2017-2020 | 78 weeks × 3 years |
| **NFTs** | Market transactions | Kaggle/Blockchain | 2017-2021 | Daily data, multiple years |
| **Bonds/Stocks** | Market prices | Yahoo Finance/FRED | 2019-2022 | Daily data, 757 observations |

### Analysis Outcomes

| Project | Primary Question | Answer Type | Conclusion |
|---------|-----------------|------------|-----------|
| **COVID-19** | How severe was excess death impact? | Statistical Significance | Significant impact detected |
| **NFTs** | Investment or fad? | Predictive/Trend-based | Likely sustainable growth |
| **Bonds/Stocks** | Optimal portfolio allocation? | Optimization/Risk-Return | Highest Sharpe ratio identified |

---

## Cross-Project Insights

### Common Themes

| Theme | Across All Projects |
|-------|-------------------|
| **R Ecosystem** | All projects leverage R for statistical analysis and visualization |
| **Data-Driven Decision Making** | Each project answers specific questions with empirical evidence |
| **Time Series Importance** | Temporal patterns critical to understanding trends |
| **Visualization for Communication** | Clear plots and charts are essential for findings |
| **Statistical Rigor** | Multiple testing methods used to validate conclusions |

### Methodological Progression

1. **COVID-19**: Foundational statistics (descriptive, hypothesis testing, ANOVA)
2. **NFTs**: Intermediate analysis (time series, trend analysis, Google Trends integration)
3. **Bonds/Stocks**: Advanced methods (time series decomposition, financial modeling, portfolio optimization)

### Data Analysis Workflow (Universal)

```
Data Collection → Data Cleaning → Exploratory Analysis → 
Statistical Testing → Visualization → Interpretation → 
Report Generation
```

---

## Key Takeaways by Project

### Statistical Analysis: COVID-19
- **Finding**: Statistically significant increase in excess deaths in early 2020
- **Methods**: Parametric and non-parametric tests confirm COVID impact
- **Significance**: Provides evidence of pandemic severity

### NFT Market Analysis
- **Finding**: NFT market shows sustainable growth patterns similar to cryptocurrency
- **Methods**: Time series tracking and trend correlation with public interest
- **Significance**: Market fundamentals suggest beyond-fad status, though volatile

### Exploring Bonds, Stocks & Portfolios
- **Finding**: Diversified portfolio construction can optimize risk-adjusted returns
- **Methods**: Financial modeling, beta analysis, and Sharpe ratio optimization
- **Significance**: Practical framework for investment decision-making

---

## Conclusion

These three projects demonstrate comprehensive statistical analysis across different domains:
- **Public Health**: Understanding pandemic impact through excess mortality data
- **Emerging Markets**: Analyzing cryptocurrency-adjacent asset class trends
- **Finance**: Developing evidence-based portfolio optimization strategies

Each project employs rigorous statistical methodology, appropriate data visualization, and practical interpretation of results for informed decision-making.

---

**Repository**: https://github.com/yohernan
**Last Updated**: May 2026
