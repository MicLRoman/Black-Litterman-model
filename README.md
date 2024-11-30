# Black-Litterman Portfolio Optimization

This project demonstrates the implementation of the Black-Litterman model for portfolio optimization. It leverages market data, risk models, and user-defined confidence in sector-specific views to construct a portfolio with optimal weights for target returns.

## Features

1. **Market Data Loading**:  
   Retrieves historical price data and market capitalization for selected stocks and ETFs using Yahoo Finance.

2. **Risk Modeling**:  
   Utilizes covariance shrinkage (Ledoit-Wolf estimator) for precise risk estimation.

3. **Black-Litterman Model**:  
   - Generates market-implied prior returns.  
   - Incorporates user-defined views with variable confidence levels.  
   - Produces posterior estimates of returns and covariances.

4. **Sector Constraints**:  
   Ensures portfolio allocations respect sector-specific upper and lower bounds.

5. **Optimization**:  
   Employs the Efficient Frontier approach to achieve optimal portfolio weights based on posterior returns and covariances.

6. **Visualizations**:  
   - Bar charts comparing prior, posterior, and view-based returns.  
   - Covariance matrix heatmaps.  
   - Pie chart illustrating portfolio allocation across sectors and ETFs.

## Key Steps

1. **Data Preparation**:  
   - Weekly price data and adjusted close prices are loaded for a 10-year period.  
   - Average annual returns and volatilities are calculated.

2. **Confidence Intervals**:  
   - Customized intervals for each sector and stock are created based on volatilities
