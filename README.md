# Modeling-Asymmetric-Tail-Risk-in-Equity-Markets-with-a-Copula-GARCH-Framework

## Overview

This repository contains the implementation and results of the project **“Modeling-Asymmetric-Tail-Risk-in-Equity-Markets-with-a-Copula-GARCH-Framework”** The study develops a two-stage framework to model marginal volatility via GARCH(1,1) and joint dependence via copulas, focusing on asymmetric tail risk and its applications to relative-value trading signals and dynamic hedging.

## Summary of Contents

* **Introduction**: Outlines the motivation for modeling joint tail risk and describes the Copula–GARCH framework.
* **Data Preparation**: Details the data sources and preprocessing steps for S\&P 500 and STOXX Europe 600 price series.
* **Marginal Modeling**: Implements GARCH(1,1) filters to capture individual asset volatility dynamics.
* **Tail Dependence Analysis**: Defines and interprets lower and upper tail dependence coefficients for extreme co-movements.
* **PIT & Copula Estimation**: Applies the Probability Integral Transform to residuals and fits multiple copula families; selects the best model based on AIC and tail-fit diagnostics.
* **Visualization**: Compares empirical joint density plots with theoretical copula contours to assess fit.
* **Pseudo–Maximum Likelihood Fitting**: Performs semiparametric estimation using rank-based uniforms for robust parameter inference.
* **Monte Carlo Simulation**: Simulates joint return scenarios under the fitted Copula–GARCH model to estimate empirical joint tail probabilities versus the independence benchmark.
* **Signal Generation**: Extracts conditional tail probabilities as triggers for relative-value trading signals and dynamic hedging overlays.
* **Backtesting & Performance**: Summarizes strategy outcomes on S\&P 500 and STOXX Europe 600, including Sharpe ratio, drawdown, and profit factor metrics.
* **Alternative Implementation Perspective**: Discusses protective overlays and gradual de-risking based on tail asymmetry insights.

## Repository Structure

```
├── scripts/                # R scripts with reusable functions for modeling and analysis
├── copula_project.Rmd      # Main R Markdown file for the full analysis and report
├── copula_project.html     # Rendered HTML report (output of R Markdown)
└── README.md               # This file
```


## Key Outputs

* **Marginal GARCH filters**: Estimated volatility processes for each index
* **Copula selection**: Comparison of Gaussian, Student‑t, and Archimedean copulas based on AIC and tail diagnostics
* **Tail dependence**: Analytical and empirical estimates of lower/upper tail coefficients
* **Conditional probability signals**: Time series of tail‐asymmetry metrics used for trading and hedging
* **Backtest results**: Performance summary of a market‑neutral strategy on S\&P 500 & STOXX Europe 600

## Contributing

Contributions are welcome. Please fork the repository, create a feature branch, and submit a pull request. Before submitting, ensure all code passes linting and the report renders without errors.


## Contact

**Laura Anedda**
MSc Financial Risk & Data Analysis
E: [laura.anedda01@gmail.com](mailto:laura.anedda01@gmail.com) 
LinkedIn: linkedin.com/in/laura-anedda
