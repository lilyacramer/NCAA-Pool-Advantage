# Pool Advantage: Facility Characteristics and Performance in NCAA Swimming

**Lily Cramer — Rice University, SMGT 490 | May 2026**

This project investigates whether pool characteristics systematically influence swimmer performance in NCAA Division I women's swimming. Using mixed-effects regression on five seasons of USA Swimming data (2021–2026), I estimate venue-level effects on standardized swim times after controlling for athlete and team quality.

## Live Application

🏊 https://wpc01l-lily-cramer.shinyapps.io/ncaa_pool_app/

## Repository Contents

**Paper** — paper/ folder
- Final report (PDF), LaTeX source, bibliography, and figures

**Code** — code/ folder
- 01_data_cleaning.R — Data wrangling, time conversion, and standardization
- 02_eda.R — Exploratory data analysis and visualization
- 03_modeling.R — Mixed-effects models, figures, and results

**App** — app/ folder
- app.R — Shiny application code
- pool_df.rds — Processed pool-level data for the app

## How to Reproduce

Run scripts in order: 01_data_cleaning.R → 02_eda.R → 03_modeling.R
Then launch the app with shiny::runApp("app/")

Note: Raw swimmer-level data is not included due to privacy considerations.

## Data Sources

Performance data: USA Swimming Top 500 Times, 2021–2026 women's NCAA seasons
Facility data: Collected from institutional aquatic center websites

## Key Findings

- Indoor environment and altitude are the strongest predictors of pool speed
- Pool depth and lane count are not statistically significant after controlling for athlete and team quality
- The pool fixed effects model outperforms the characteristics model (AIC: 10,538 vs. 10,563)
- Christiansburg Aquatic Center ranks as the fastest pool in the sample
