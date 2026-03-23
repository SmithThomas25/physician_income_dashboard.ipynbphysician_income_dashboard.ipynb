
# Physician Income Model – Québec GMF

## Overview
This project builds a quantitative model to analyze how different funding structures impact physician income in Quebec’s GMF system.

It combines economic theory, optimization, and Monte Carlo simulation to model physician behavior under different incentives.

## Key Features

- Monte Carlo simulation of physician income
- Multiple funding structures:
  - Fee-for-Service (FFS)
  - Capitation
  - Mixed model
- Patient heterogeneity:
  - Young, adult, chronic patients
- Bonus system based on continuity of care
- Nurse delegation modeling in capitation-heavy scenarios
- Interactive dashboard (ipywidgets + matplotlib)

## Model Structure

The physician income is modeled as:

Income = FFS + Capitation + Bonus

Subject to:
- Time constraints
- Patient complexity
- Demand uncertainty

## Technologies Used

- Python
- NumPy
- Matplotlib
- ipywidgets (interactive dashboard)

## How to Run

1. Open the notebook:
   physician_income_dashboard.ipynb

2. Run all cells

3. Use sliders to explore:
   - Capitation rate
   - Fee-for-service rate
   - Bonus levels
   - Patient mix

## Insights

- FFS-dominant models increase income volatility but allow higher upside  
- Capitation stabilizes income but introduces capacity constraints  
- Patient complexity significantly impacts time allocation and revenue  
- Bonus structures create nonlinear incentives  

## Author

[Your Name]
