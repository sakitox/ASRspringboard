# Analysis of house prices in London 1995-2019

We explored residential transactions across UK and London specifically and managed to achieve an optimized RMSE. Unfortunately, the features were not rich enough to have a more accurate prediction with a 98% confidence on +-65,000 compared to the actual prices in 2020. Nonetheless our result allows us to have a clear comparison between the expected properties prices and the ones offered in the corona-market economy. 

The model can be run to predict a new observation dated to the current month (June 2020) and any postcode in London. For example, entry for postcode ‘W4 1PE’ reflects the expected price of the property in 06-2020. The model does not discriminate between number of beds or baths as there is no data to link transactions to flat descriptors. However, our study is accurate enough to help any individual inform themselves better about real estate price projections to a very high level of detail. The XGB model was run to estimate a comparison on the price for a typical property at ‘W3 7QN’ in 06-2000, the predicted price for the property in 06-2012, and the predicted price for the property and 06-2020. The predicted prices are £242k in 2000, £484k in 2012 (actual value £568k), and £616k in 06-2020. Interesting, huh?

## Introduction

The housing market was in a fairly good position before Covid-19. The head of research at estate agent Knight Frank stated that the housing market was in a “strong position” for the first months of 2020, noticing a general trend of price increases and sales across the UK. For properties in central London, the market was beginning to experience a reversal of the decline caused by Brexit uncertainty. More houses were being built and around 70,000 mortgage approvals were made in February alone, which was the highest monthly figure in six years.

## Data Sources

The data set was acquired from various open sources. The first set was retrieved from the UK government HM Land Registry. The dataset dubbed ‘Price Paid Data’ or PPD includes information on all property sales in England and Wales that are sold for value and are lodged with HRMC for registration; the data contains HM Land Registry data ©Crown copyright and database right 2020. This data is licensed under the Open Government License v3.0.
The second and third datasets were retrieved from the Office for National Statistics, also a part of the UK government. The second file contains the National Statistics Postcode Lookup (NSPL) for the United Kingdom as of February 2019 in Comma Separated Variable (CSV). The third and final file contains the digital vector boundaries for Local Authority Districts in the United Kingdom as of 1 April 2019.

## Model

Comparison of XGBoost and Random Forest Regressor both in normal quantities and log transforms. We initially tried a few more algorithms that have been omitted due to poor performance

