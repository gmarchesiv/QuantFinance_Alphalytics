# Alphalytics
This repository contains the data and analysis for portfolio optimization using dynamic asset allocation through the business cycle. 

The goal of this project is to maximize the historic return of an investment portfolio by optimizing the asset allocation during the four stages of an economic cycle: 
1. Recovery: period immediately after a slowdon or recession  
2. Expansion: stable growth period after a recovery period 
3. Slowdown: period of stagnant or decreasing growth that may precede a recessions or might happen in the middle of a cycle
4. Contraction: period of decreasing growth, following a slowdown

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

When using this metric against equities there is a certain degree of endogeneity, although the weight of the S&P is only 3.81%. I constrast the findings of this methodology with the Coincident Economic Index, also from the Conference Board composed of the following 4 variables:

- Employees on nonagricultural payrolls	
- Personal income less transfer payments	
- Industrial production
- Manufacturing and trade sales

and the NBER classification of the business cycle (month of expansion or contraction).

The chosen assets for this analysis are the following ETFs: 
## Equities: 
1. SPY: SPDR Standard and Poors 500 Trust
2. DIA: SPDR Dow Jones Industrial Trust 
3. IWM: iShares Russell 2000 Trust
4. QQQ: Invesco QQQ NASDAQ Trust
## Treasuries: 
5. IEF: iShares 7-10 Year Treasury Bond ETF
6. SHY: iShares 1-3 Year Treasury Bond ETF
7. TLT: iShares 20+ Year Treasury Bond ETF
## Corporates: 
8. IGLB: iShares 10+ Year Investment Grade Corporate Bond ETF
## Commodities: 
9. GLD: SPDR Goldshares Trust
10. DBC: Invesco DB Commodity Index Tracking Fund
## Cryptocurrencies: 
11. BTC: Bitcoin
12. ETH: Ethereum 

The algorithn optimizes by risk adjusted weight at the asset allocation. At the asset level, a second type of algorithm, a trading algorithm seeks to maximize the return of the asset by trading on the signals of price change for different hourly/daily periods and market volatility as represented by VIX. 
This repository is divided in three sections: 

1. Data: the compiled csv data to run the notebooks
2. Analysis: the python notebooks
3. Results: the writeup reports 

Trading algorithms are the authors IP and will not be shared, though results will be presented section 3. 

