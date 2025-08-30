# Real Estate Rental Profitability Data Analysis: Technical Report  

## Objective and Scope  

This project analyzes **70,000 real estate listings** to uncover the property characteristics that maximize rental profitability. Profitability here is defined as:  

- **Higher annual net rent** relative to purchase price.  
- **Shorter payback period** (years to profit).  

## Data Preparation and Feature Engineering  

To better evaluate profitability, three key features were created:  

- **`annual_expenses`** – sum of property tax, insurance, and maintenance costs.  
- **`annual_net_rent`** – annual rent minus expenses, reflecting true rental income.  
- **`years_to_profit`** – payback period, calculated as purchase price ÷ annual net rent.  

These engineered variables provide a reliable foundation for comparing investment opportunities.  

## Exploratory Data Analysis (EDA)  

The dataset was explored across both categorical and numerical dimensions:  

- **Distributions**: Analyzed property price, net rent, and years to profit.  
- **Categorical comparisons**: Compared averages across location, region type, property type, condition, and furnishing.  
- **Correlations**: Used heatmaps and scatterplots to explore how size, economic indicators, and neighborhood factors impact profitability.  

## Analytical Methods  

- **Barplots with means**: Highlighted group differences with annotated averages.  
- **mean payback years**: Summarized profitability timelines.  
- **Correlation coefficients**: Identified the strongest numeric drivers of rental returns.  

## Key Findings  

- **Location matters**: *San Diego, San Jose, and Los Angeles* deliver **20–35% higher net rents** and recover investments **15–20% faster**.  
- **Property type**: *Houses and Apartments* earn **25–30% more rental income** compared to other types.  
- **Urban premium**: Urban properties outperform suburban with **18–22% higher yields**.  
- **Condition & furnishing**: *New or excellent* condition and *fully furnished* homes achieve **15–30% higher rents**.  
- **Size effect**: Larger properties (≥1500 sqft, 3+ bedrooms, multi-story, parking) strongly correlate with higher income and faster payback.  
- **Neighborhood economy**: Areas with *median income > $50,000* and *employment > 90%* consistently outperform in rental returns.  

## Conclusion  

The analysis confirms that profitability is driven by a combination of **location, property design, condition, and local economic health**.  
The engineered features (`annual_expenses`, `annual_net_rent`, `years_to_profit`) and the structured EDA process provide a **replicable framework** for evaluating real estate investment opportunities with data-driven precision.  
