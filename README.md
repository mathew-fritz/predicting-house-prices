# Predicting House Prices
This project uses the following data which was imported, cleaned, merged, and explored before making the model: 

## Federal Reserve Data
- [Consumer Price Index](https://fred.stlouisfed.org/series/CPIAUCSL)
- [Rental Vacancy Rate](https://fred.stlouisfed.org/series/RRVRUSQ156N)
- [30 Year Fixed Mortgage Rate](https://fred.stlouisfed.org/series/MORTGAGE30US)

## [Zillow Data](https://www.zillow.com/research/data/)
- Zillow Home Value Index (ZHVI, raw, weekly)
- Median sale price (raw, all homes, weekly)

# Model Creation
A random forest machine learning model was then made to help predict future house prices. Included in this model is backtesting to ensure past data is used as the basis for future predictions. Five years of past data is used initially (2008-2013) to predict 2014, then 2008-2014 is used to predict 2015 and so on. Yearly ratios were added as predictors to the model to help better identify trends for variables such as interest rate. The most important variables (predictors) were determined as well.

# Results
- The initial accuracy of the model was approximately 57%. 
- Once additional variables (yearly ratios) were added, the accuracy of the model improved to 66%, a 9% increase.
- The most important variables to the model were adjusted price and value (ZHVI).

# Ways to improve the model
- Try different algorithm types (such as support vector machine or decision tree).
- Find extra data to use as additional variables (news articles for example).
