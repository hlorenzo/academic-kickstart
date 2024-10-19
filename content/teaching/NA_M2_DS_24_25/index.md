+++
title = "How to deal with missing values, 2022"

date = 2024-10-18T00:00:00

summary = "AMU"

tags = ["French","Formation continue","Visualization","Missing values"]

# Optional external URL for project (replaces project detail page).
# external_link = "/uploads/M2_DS/M2_stats_de_la_SD_2024.html"
+++

[Course]("./uploads/M2_DS/M2_stats_de_la_SD_2024.html")

1. **Definition of Missing Data**:
   - Data is considered missing when a variable's observation is unavailable. 
   - Complete case analysis (removing observations/variables with missing values) is generally discouraged due to the risk of introducing bias and reducing statistical power.

2. **Examples and Scenarios**:
   - Practical examples illustrate missing data consequences, such as weight saturation values or subpopulations not responding.

3. **Mechanisms of Missing Data**:
   - Based on Little and Rubin's framework:
     - **MCAR (Missing Completely At Random)**: The probability of missingness is independent of any variable.
     - **MAR (Missing At Random)**: Probability depends on observed data but not the missing value itself.
     - **MNAR (Missing Not At Random)**: Probability depends on the missing value, even considering observed data.

4. **Imputation Methods**:
   - **Simple Imputation**: Techniques like the mean/median, k-Nearest Neighbors (kNN), random forests (**missForest**), or PCA (**missMDA**) replace missing values.
   - **Multiple Imputation**: Tools like the **mice** package generate multiple imputed datasets to account for uncertainty.

5. **Advanced Methods**:
   - **EM Algorithm**: Iteratively estimates missing data and updates parameters for likelihood maximization, suitable for **MAR** scenarios with models like the multivariate normal distribution.
   - **MCEM (Monte Carlo EM)**: Uses Monte Carlo simulations when the E-step cannot be computed directly, effective for complex and high-dimensional data models.
   - **VBEM (Variational Bayes EM)**: Employs variational methods for Bayesian estimation, providing efficient approximations in **MNAR** contexts where traditional EM is computationally intensive.

6. **Practical Exercises**:
   - Simulations using INSEE data on French population age distributions demonstrate different missing data mechanisms (MCAR, MAR, MNAR).
