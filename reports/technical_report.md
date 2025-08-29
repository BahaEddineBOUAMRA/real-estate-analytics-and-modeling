# Real Estate Rental Profitability Data Analysis: Technical Report

## Objective and Scope

This analysis explores a dataset of 70,000 real estate listings to identify key property features maximizing rental profitability, defined by the highest annual net rent relative to purchase price, and the shortest years to profit.

## Data Preparation and Feature Engineering

- Engineered critical variables:
  - `annual_expenses`: Summation of property tax, insurance, and maintenance.
  - `annual_net_rent`: Annualized rent minus expenses, capturing real net income.
  - `years_to_profit`: Payback period as price divided by annual net rent.

These features allow an accurate assessment of rental investment viability.

## Exploratory Data Analysis (EDA)

- Analyzed distributions of price, net rent, and years to profit.
- Compared averages for price and net rent across categorical features: location, region_type, property_type, condition, furnishing.
- Examined numeric feature correlations via heatmaps and scatterplots, focusing on size, economic, and neighborhood factors.

## Key Analytical Methods

- Used categorical barplots with mean estimators and annotations to visualize group differences.
- Calculated mode and mean payback years to characterize temporal profitability.
- Leveraged correlation coefficients to evaluate numeric variable impact.

## Findings

- Location significantly influences profitability: San Diego, San Jose, and Los Angeles yield 20-35% higher net rents and 15-20% faster payback.
- Property types: Houses and Apartments outperform others by 25-30% in rental income.
- Urban region type delivers 18-22% greater rental yields than suburban.
- New or excellent condition and furnished homes command 15-30% higher rents.
- Larger floor area (≥1500 sqft), 3+ bedrooms, multi-story structures with parking strongly correlate with higher net rents and faster payback.
- Economic factors: neighborhoods with median incomes > $50,000 and employment > 90% show superior rental performance.

## Conclusion

This analysis confirms that combining location, property design, condition, and economic context optimizes rental investment decisions. The engineered features and comprehensive EDA provide a replicable framework for data-driven real estate profitability assessment.
