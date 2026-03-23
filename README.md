# Physician Income Model – Québec GMF

## Overview

This project develops a quantitative framework to analyze how different funding structures influence physician income within Quebec’s Groupe de médecine de famille (GMF) system. It is grounded in economic theory and formalizes physician behavior as an optimization problem under multiple incentive mechanisms.

The model integrates fee-for-service compensation, capitation payments, and performance-based bonuses into a unified structure. It further incorporates uncertainty through a Monte Carlo simulation approach, allowing for the estimation of income distributions rather than deterministic outcomes.

## Model Description

Physician income is modeled as the aggregation of three primary components: fee-for-service revenues, capitation payments linked to enrolled patients, and performance-based bonuses. This structure is evaluated under binding constraints, notably limited physician time, heterogeneous patient complexity, and stochastic demand for medical services.

Patient heterogeneity is explicitly modeled by assigning different complexity weights to distinct patient profiles, including younger individuals, standard adult patients, and those with chronic conditions. These differences affect both revenue generation and time allocation, creating a trade-off between patient volume and care intensity.

The model also incorporates organizational dynamics observed in GMFs, particularly the delegation of certain tasks to nursing staff in capitation-heavy environments. This mechanism effectively relaxes time constraints and alters the physician’s optimal strategy.

## Methodology

The analytical framework relies on Monte Carlo simulation to capture the inherent uncertainty in patient demand, attendance rates, and panel composition. Each simulation represents a potential realization of the physician’s practice environment, generating a distribution of income outcomes across different funding structures.

This approach allows for a rigorous comparison of scenarios dominated by fee-for-service incentives, capitation-based models, and hybrid structures. The results are evaluated in terms of expected income as well as variability, providing insight into both performance and risk.

## Implementation

The model is implemented in Python using numerical and visualization libraries. An interactive dashboard is developed to enable real-time exploration of key parameters, including capitation rates, fee-for-service levels, bonus structures, and patient composition. This interface allows users to observe how changes in funding design translate into different income distributions and risk profiles.

## Results and Insights

The simulation highlights that funding structures fundamentally shape physician behavior. Fee-for-service dominant models tend to increase income variability while offering higher potential upside, reflecting strong incentives for volume maximization. In contrast, capitation-based systems provide more stable income streams but introduce binding capacity constraints, particularly in the presence of complex patient populations.

The inclusion of performance-based bonuses generates nonlinear effects, as income can shift significantly once specific thresholds are reached. Additionally, patient complexity emerges as a critical determinant of both revenue and time allocation, reinforcing the importance of accounting for heterogeneity in healthcare modeling.

## How to Run

To run the model, open the notebook file titled `physician_income_dashboard.ipynb` in a Jupyter environment or Google Colab, execute all cells, and interact with the dashboard using the provided sliders. This allows for dynamic exploration of the model’s parameters and their impact on income distributions.

## Author

Smith Thomas Dotonou
