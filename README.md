# Alphalytics
This repository contains the data and notebooks for the construction of a dynamic asset allocation model throughout the business cycle. 

The goal of this project is to maximize the historic return of an investment portfolio by optimizing the asset allocation during the four stages of an economic cycle: 
1. Recovery: period immediately after a slowdon or recession  
2. Expansion: stable growth period after a recovery period 
3. Slowdown: period of stagnant or decreasing growth that may precede a recessions or might happen in the middle of a cycle
4. Contraction: period of decreasing growth, following a slowdown

## Determining the stages of the cycle
To determine these stages, I use The Conference Board's Leading Economic Index, the longest running and most reputable leading indicator in the market. The index is composed of the following ten variables: 

- Average weekly hours in manufacturing 
- Average weekly initial claims for unemployment insurance
- Manufacturers’ new orders for consumer goods and materials
- ISM® Index of New Orders
- Manufacturers’ new orders for nondefense capital goods excluding aircraft orders
- Building permits for new private housing units
- S&P 500® Index of Stock Prices; Leading Credit Index™
- Interest rate spread (10-year Treasury bonds less federal funds rate) 
- Average consumer expectations for business conditions.

When using this metric against equities there is a certain degree of endogeneity, although the weight of the S&P is only 3.81%. 

I constrast the findings of this methodology with the Coincident Economic Index, also from the Conference Board composed of the following 4 variables:

- Employees on nonagricultural payrolls	
- Personal income less transfer payments	
- Industrial production
- Manufacturing and trade sales

and the NBER classification of the business cycle (month of expansion or contraction).

The first part of the analysis centers on determining these four stages. Further analysis evaluates the performance of asset classes during the stages. 



