# Hyundai_Stock_Price Simulator

## Main Goal/Aim ##
Underwent DCF Analysis through WACC-based discount rate to analyse and forecast the expected growth of Hyundai within the next 5 years. In addition, simulated share price analysis using Monte Carlo simulations, modelling both uncertainty and risk. This DCF Model has been built with the assumption that Hyundai is going to launch its IPO just like top-tier Korean Semi-Conductor Company, SK Hynix where they have underwent IPO in 2026. As such, I hope that this model for future investors give deeper insights into the valuation of business.




## Summary of Files and Pages

- Python File:

  Holds the Monte Carlo Simulations of Share prices, using normally distribued probability distributions to analyse and simulate potential prices of Hyundai shares for 10 years.

  Here, I have used the WACC I have obtained from Alphaspread as a discounting factor for Hyundai for transparency and higher accuracy.

  

- Excel File:

  Holds the DCF Model that includes the expected EBIT growth and revenue growth alongside discounting factors of WACC. Revenue growth have been forecasted using historical mean and stadard deviations, where I have generated a normally generated random figure. Excel file also contains financial records and calculations that I have reconciled and approximated from available sources online.

## Key Findings:

* True variance: 11827.8870
* Monte Carlo-Generated variance: 1307.9007
* Percentage error: 88.94%

There lies significance variances in the true history of stock prices for Hyundai compared to the Monte-Carlo Generated Stock price. Major cause of this could be due to simulations that may not reflect upon the data of the true data. As data itself has been generated through a normally distributed random sampling, data may have some outliers but most will be centered around the Mean and Variance.


* WACC from Alphaspread: 7.38%
* WACC estimated: 1.80%

WACC has been generated from the DCF modelling of share prices, using historical growth patterns to generate reasonable data. After some testing, Share price tends to differ in prices of roughly 0% to 309%. We take 0%, only if the given Firm Value comes out as a negative value from the simulations, which is a reasonable assumption to make.


## Limitations:

- Calculation of WACC using my approach to generate and forecast projected revenue using historical mean and standard deviation ultimately led to significant variance in the outcome of the FCF Calculation, which consequently impact the firm value and share price calculation

- Time periods for both dataset obtained for the Excel File and the Python Jupyter Notebook may differ, which could impact calculation of firm value

- Used the CAPM approach to calculate cost of equity that impacts the overall WACC. However, limitations of this exist such as Beta being a measure of systematic risk faced by holding Hyundai shares and thus cannot be accurately measured, the Market Rate also needs to be approximated and cannot be pinpointed and a higher beta does not necessarily yield greater returns and thus shows very little correlation between High Beta (High systematic risk) vs Shareholder Returns


## Potential Improvements:

- When calculating the cost of equity, can also utilise the Dividend Growth Model to historically track change in cost of equity throughout time

- Double confirmation of dataset and calculation of key components like Capital Expenditures captured within the file. So far, I have realistically assumed off of the financial statements to estimate the capital expenditures and other components that were not directly listed

## References:
- https://www.hyundai.com/worldwide/en/company/ir/financial-information/quarterly-earnings
- https://www.alphaspread.com/security/krx/005380/discount-rate
- https://www.investopedia.com/
- https://valueinvesting.io/005380.KS/valuation/wacc
