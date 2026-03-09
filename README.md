# Chicago Building Permits: Investment Opportunity Assessment
**BUSN 32120 Final Project — Group 50**
Audrey Zhang, Jeena Lee, Vincent Wang

---

## Project Overview
This project analyzes 2024+ Chicago building permit data combined with neighborhood socioeconomic indicators to identify real estate investment opportunities across Chicago's 77 community areas. The analysis is aimed at **real estate developers and investment firms** looking for data-driven insights on where and how to deploy capital in the Chicago construction market.

## Repository Contents

| File | Description |
|------|-------------|
| `Final_Project.ipynb` | Main Python analysis notebook — data collection, EDA, feature engineering, and predictive modeling |
| `SQL_Queries.ipynb` | Standalone SQL notebook with 12 annotated SQLite queries covering joins, window functions, rollups, and subqueries |
| `Chicago_Investment_Presentation.pdf` | Slide deck presented in class |

## Data Sources
- **Chicago Building Permits** — City of Chicago Open Data Portal (Socrata API)
- **Chicago Socioeconomic Indicators** — City of Chicago community area demographics (income, poverty, unemployment)

## Key Questions Answered
1. Which community areas are attracting the most construction investment?
2. How do neighborhood income levels correlate with development activity?
3. What is the cost structure across different project types?
4. Are there under-invested, high-upside neighborhoods (gentrification signals)?
5. What predicts whether a project will be a major investment (≥$100K)?

## Methods
- Data collection via paginated REST API calls
- Exploratory data analysis with seaborn and matplotlib
- Feature engineering: OHE, min-max normalization, IQR outlier detection, composite investment score
- Predictive modeling: Linear Regression (project cost) and Logistic Regression (high-value classifier)
- SQL analysis: SQLite with joins, window functions, GROUP BY/ROLLUP, and CTEs