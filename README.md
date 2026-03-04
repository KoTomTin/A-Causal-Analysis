Here is the README:

---

# NHANES Cadmium & Mortality — Causal Inference Analysis
Pooled NHANES 2007–2012 | Kaung Khant Tin

---

## What This Is

A fully reproducible causal analysis examining whether blood cadmium — a biomarker of cumulative environmental toxic burden — mediates the relationship between socioeconomic deprivation and all-cause mortality. Built as part of a PhD application to the Division of Cancer Sciences, University of Manchester.

## Methods

Three-level causal inference framework following Pearl's ladder of causation — association (Kaplan-Meier), intervention (sequential Cox regression), and counterfactual (g-computation with bootstrap CIs).

## Data

Four data streams linked at individual level via SEQN, downloaded automatically within the Rmd on first run: NHANES Demographics, Blood Cadmium, Serum Cotinine (via `nhanesA`), and CDC Linked Mortality Files via National Death Index through December 2019. Three cycles pooled (2007-08, 2009-10, 2011-12): N = 10,410 White and Black Americans, 1,780 all-cause deaths.

## How to Run

Open `nhanes_cadmium_report.Rmd` in RStudio and click Knit. Everything — data download, preparation, and analysis — runs in a single file. Requires R 4.2+ and an internet connection on first run. Packages install automatically.

---
