# A Causal Analysis (NHANES Cadmium & Mortality)

This repository contains a causal analysis written as an R Markdown report, 
built as a methodological proof of concept for the proposed PhD research at 
the University of Manchester's Division of Cancer Sciences.

## The main deliverables are:

- `CausalInference.Rmd` — the full analysis and code
- `CausalInference.html` — the knitted report output (HTML)

## What this analysis does

Using pooled NHANES 2007–2012 data (N = 10,410; 1,780 deaths), this analysis 
investigates whether blood cadmium — a biomarker of cumulative environmental 
toxic burden — partially explains the link between socioeconomic deprivation 
and premature mortality. The analysis is structured around Judea Pearl's three 
levels of causal inference:

- **Level 1 — Association:** Kaplan-Meier curves and descriptive analysis
- **Level 2 — Intervention:** Sequential Cox proportional hazards models 
  (M1–M5) with confounding decomposition, multiplicative interaction test, 
  additive interaction analysis (RERI; VanderWeele & Knol 2014), Schoenfeld 
  diagnostics, and cotinine sensitivity analysis
- **Level 3 — Counterfactual:** G-computation with Weibull AFT model and 
  bootstrap confidence intervals (n = 500)

## Viewing the report (HTML)

GitHub sometimes cannot display large HTML files directly in the browser.
To view the report:

1. Open `CausalInference.html` in this repo
2. Click **Download** (or **View raw**) to save it to your computer
3. Open the downloaded file in a web browser (Chrome/Safari)

## How to run / re-knit the report

1. Open `CausalInference.Rmd` in RStudio
2. Install any missing packages when prompted
3. Click **Knit**
