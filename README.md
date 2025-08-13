# CO₂ Emission Dataset – EDA Insights

## 1. Data Overview

Countries: 267

Years Covered: 1990–2019 (2020 & 2021 missing for all countries).

Metric: CO₂ emissions in metric tons per capita.

Regions: 8 distinct (largest: Europe & Central Asia – 58 countries).

Income Groups: 5 categories (largest: High income – 80 countries).

## 2. Data Quality & Pre-processing
~9–12% missing values for most years before 2020.

Region missing for 18% of countries; IncomeGroup missing for 18.5% — filled as "Unknown".

Missing numeric values filled with 0 for continuity.

Removed duplicate country codes.

Dropped irrelevant columns: 1996.1, 2020, 2021.

## 3. Univariate Findings
Distribution: All yearly emissions are right-skewed — most countries emit little, a few emit very high amounts.

Outliers: Before treatment, ~3–7% of countries per year had extreme high values (e.g., Qatar, Kuwait).

**Central Tendency Example (2019):**

Mean: 3.69 t/capita

Median: 2.34 t/capita

Max: 32.76 t/capita

Mode: 0.0 t/capita

**Regions with the most countries:**

Europe & Central Asia (58)

Sub-Saharan Africa (48)

Unknown (48)

Most frequent income group: High income (80 countries).

## 4. Bivariate Insights
Region vs Income Group: Strong association (Chi-square p < 0.0001).

High income concentrated in Europe, North America.

Low income concentrated in Sub-Saharan Africa & South Asia.

Average Emissions by Region:

Highest: North America & Middle East

Lowest: Sub-Saharan Africa & South Asia

Average Emissions by Income Group:

High income countries consistently highest in all years.

Low income countries have negligible per capita emissions.

## 5. Temporal Correlation
Year-to-Year correlation is very high (> 0.9), showing emissions patterns are persistent over decades.

Countries with high emissions remain high; low remain low.

## 6. Outlier Treatment
Replaced extreme values (IQR method) with yearly medians for cleaner analysis.

## 7. Key Takeaways
Inequality in emissions — a small group of nations dominate per capita output.

Economic link — higher income levels strongly correlate with higher emissions.

Regional divide — Developed regions emit more per capita than developing ones.

Stable rankings — Country emission levels change little over time.

Data gaps — 2020–2021 entirely missing, likely due to reporting delays.


# Simple, Impactful Insights

1. Most of the world pollutes very little — but a few countries pollute a lot

- The majority of countries emit less than 2 tons of CO₂ per person per year.

- A handful of countries emit more than 30 tons per person — that’s over 15× the global median.

- This shows global emissions are not evenly distributed.

2. Wealth and emissions go hand-in-hand

- Richer countries almost always have higher per-person emissions.

- Poorer countries contribute far less, even though they may have large populations.

3. Your region matters

- People in North America and the Middle East emit far more CO₂ than those in Africa or South Asia.

- This reflects differences in lifestyle, industry, and energy use.

4. Countries rarely change their pollution ranking

- If a country was a high emitter in 1990, it’s probably still high today.

- This means emissions are tied to long-term economic and infrastructure patterns, not short-term changes.

5. 2020 and 2021 data is missing

- Likely due to delays in international reporting (and possibly COVID-19 disruptions).

- This gap itself is important — it means we can’t yet see the pandemic’s effect on emissions.

6. Some extreme values may be misleading

- For very small countries with tiny populations, even modest industrial activity can push their per-person emissions off the charts.

- Example: A small island with a big oil refinery can appear “dirtier” than big economies.
