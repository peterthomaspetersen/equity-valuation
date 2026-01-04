# Mercedes-Benz Equity Analysis: A Multi-Method Valuation Framework

## Overview

This repository contains my equity research project analyzing Mercedes-Benz Group AG (MBG), developed during my Investment Research Analyst internship at Strategic Global Advisors. The project combines traditional fundamental valuation techniques with a novel GenAI-enhanced approach to price target validation.

The analysis culminated in a stock pitch presentation that generated sufficient conviction among senior analysts to pursue deeper due diligence on the investment thesis.

---

## Project Objectives

1. Conduct comprehensive fundamental analysis of Mercedes-Benz using industry-standard valuation methodologies
2. Develop traditional DCF and DDM models to establish intrinsic value estimates
3. Build a novel risk-scoring mechanism for price target validation as an alternative to traditional model-dependent approaches
4. Leverage GenAI tools to enhance thesis development, challenge assumptions, and stress-test the investment narrative
5. Synthesize findings into a compelling, defensible stock pitch

---

## Valuation Methodologies

### Discounted Cash Flow (DCF) Model

The DCF model estimates intrinsic value by projecting future free cash flows and discounting them back to present value. This approach answers the question: "What is the company worth based on the cash it will generate?"

**Key components built:**
- Revenue projections based on segment analysis (Mercedes-Benz Cars, Mercedes-Benz Vans, Mercedes-Benz Mobility)
- Operating margin assumptions informed by historical performance and industry trends
- Capital expenditure and working capital forecasts
- Weighted Average Cost of Capital (WACC) calculation incorporating:
  - Cost of equity (via CAPM)
  - Cost of debt (based on current borrowing rates)
  - Target capital structure
- Terminal value estimation using perpetuity growth method
- Sensitivity analysis across discount rates and growth assumptions

### Dividend Discount Model (DDM)

The DDM values a stock based on the present value of expected future dividends. This approach is particularly relevant for Mercedes-Benz given its history of consistent dividend payments and commitment to shareholder returns.

**Key components built:**
- Historical dividend analysis and payout ratio trends
- Dividend growth rate projections (multi-stage model)
- Cost of equity calculation
- Gordon Growth Model implementation for terminal value
- Scenario analysis across dividend growth assumptions

### Price Target Risk-Scoring Mechanism (Novel Approach)

Traditional valuation models like DCF and DDM are highly sensitive to input assumptions — small changes in growth rates or discount rates can dramatically swing the output. This creates false precision and makes it difficult to assess confidence in price targets.

I developed an alternative framework that assigns probability-weighted risk scores to a vector of price targets, providing a more nuanced view of valuation uncertainty.

**How it works:**
- Generate a range of price targets based on varying input assumptions
- Assign probability weights to each scenario based on likelihood
- Calculate expected value and confidence intervals
- Score overall risk based on distribution characteristics (variance, skewness, tail risk)
- Compare risk-adjusted targets against current market price

**Why this matters:**
- Acknowledges uncertainty rather than hiding it in point estimates
- Provides a framework for comparing conviction levels across investment ideas
- Offers an independent validation layer that doesn't rely solely on model outputs

---

## GenAI-Enhanced Analysis

A key differentiator of this project was the systematic integration of GenAI tools throughout the research process. Rather than using AI as a shortcut, I developed a structured prompt library to enhance rigor and challenge my own thinking.

### Applications:

**Thesis Development & Ideation**
- Industry analysis and competitive positioning
- Identification of key value drivers and risk factors
- Generation of alternative investment narratives to stress-test assumptions

**Assumption Validation**
- Cross-referencing growth assumptions against industry benchmarks
- Identifying potential blind spots in the investment thesis
- Generating bear case scenarios and counterarguments

**Research Synthesis**
- Summarizing earnings calls and management commentary
- Extracting key metrics from financial filings
- Identifying sentiment shifts in analyst coverage

**Presentation Refinement**
- Structuring the narrative arc of the stock pitch
- Anticipating likely pushback questions from senior analysts
- Refining language for clarity and impact

### Prompt Library

The `/prompts` folder contains the GenAI prompts I developed and refined throughout this project, organized by use case. These represent a reusable framework for AI-enhanced equity research.

---

## Data Sources

- **FactSet** — Financial statements, estimates, market data, and comparable company metrics
- **Bloomberg Terminal** — Real-time pricing, news, and supplementary financial data
- **Company Filings** — Annual reports, investor presentations, and earnings call transcripts
- **Industry Research** — Automotive sector reports and macroeconomic analysis

---

## Repository Structure

```
├── README.md
├── /notebooks
│   ├── 01_data_collection.ipynb
│   ├── 02_dcf_model.ipynb
│   ├── 03_ddm_model.ipynb
│   ├── 04_risk_scoring_model.ipynb
│   └── 05_sensitivity_analysis.ipynb
├── /excel
│   ├── mercedes_dcf_model.xlsx
│   ├── mercedes_ddm_model.xlsx
│   └── price_target_risk_matrix.xlsx
├── /prompts
│   ├── thesis_development.md
│   ├── assumption_validation.md
│   ├── bear_case_generation.md
│   └── presentation_refinement.md
├── /data
│   └── (sample data files - proprietary data excluded)
└── /output
    └── (visualizations and summary tables)
```

---

## Key Findings

*Note: Specific price targets and recommendations are omitted to protect proprietary analysis.*

The analysis identified Mercedes-Benz as a compelling opportunity based on:

- Undervaluation relative to intrinsic value estimates across multiple methodologies
- Strong free cash flow generation supporting dividend sustainability
- Strategic positioning in luxury EV transition
- Margin resilience despite industry headwinds
- Attractive risk/reward profile based on probability-weighted scenario analysis

The investment thesis was presented to senior analysts and portfolio managers, resulting in further due diligence and deeper examination of the opportunity.

---

## Skills Demonstrated

- **Financial Modeling:** DCF, DDM, sensitivity analysis, scenario modeling
- **Quantitative Analysis:** Probability weighting, risk scoring, statistical distributions
- **Programming:** Python (pandas, numpy, matplotlib), Jupyter Notebooks
- **Data Platforms:** FactSet, Bloomberg Terminal
- **GenAI Application:** Structured prompt engineering for research workflows
- **Communication:** Synthesizing complex analysis into actionable investment recommendations

---

## About Me

I'm a recent graduate from the University of Oregon with a BS in Operations and Business Analytics. I'm passionate about combining quantitative methods with emerging AI tools to solve business problems.

This project represents my approach to analysis: rigorous fundamentals, intellectual honesty about uncertainty, and thoughtful integration of new technologies.

**Contact:**
- Email: peterthomaspetersen@gmail.com
- LinkedIn: [linkedin.com/in/peter-petersen-49a7182a5](https://linkedin.com/in/peter-petersen-49a7182a5)

---

## Disclaimer

This repository is for educational and portfolio demonstration purposes only. It does not constitute investment advice. Proprietary data and specific investment recommendations have been excluded. All opinions are my own and do not reflect the views of Strategic Global Advisors or any other organization.# equity-valuation
