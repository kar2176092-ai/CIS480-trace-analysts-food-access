# CIS480-trace-analysts-food-access
## Food Access Prioritization Pipeline | USDA 2019 (LRAM) | Cook County, Illinois
### Team Trace Analysts

This project is a reproducible Python pipeline designed to identify census tracts that are most in need by assessing barriers regarding food accessibility. Using the USDA 2019 Large Retailer Access Map (LRAM), we analyze socioeconomic and geographic indicators across Cook County, Illinois.

### Key Features
* **Design Architecture:** Built with a modular design, allowing the analysis to be re-run for any state or county by simply changing configurations.
* **Data Cleaning & Imputation:** Handles USDA's specific null values, imputes missing median incomes, and preserves census tract IDs as 11-digit strings.
* **Prioritization Scoring:** Calculates a weighted `PriorityScore` based on six key indicators: Poverty Rate, distance to supermarkets (>1 mile), low-income & low-access populations, housing units without vehicles, SNAP household rates, and median family income.
* **Exportable Outputs:** Generates clean, analysis-ready CSVs (`cook_county_scored.csv` and `cook_county_top20.csv`) for mapping and visualization.

### Data Disclaimer
LRAM data is historical, limited to 2010 census-tract boundaries & population, 2014–18 ACS
socioeconomics, and 2019 retailer locations. It is not a 2026 measure of food access.
