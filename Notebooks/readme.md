# Analysis

This folder contains the necessary pyhton notebooks to conduct the macroeconomic analysis. These were written for Google Colaboratory and might need certain adjustments when loading the data locally using Jupyter Notebook like eliminating the file.upload() method and pointing directly to the local directory in the read_csv() function.  

## Methodology
Using the Leading Economic Index produced by the Conference Board, I identify patterns in monthly, quarterly and semi-annual changes in the index, as well as in the magnitude of the semi-annual changes, to classify each month into one of the four stages of the economic cycle. I contrast this classification with NBER's determination of contraction and expansion periods. I use this backdrop to estimate the average returns of each asset during each stage and estimate the correlations among assets to choose a shifting optimized portafolio across stages.   

## List of notebooks
1. Generating_Economic_Dataset: calculates 1m, 3m and 6m changes in the LEI and the signs of those changes to create a new dataset. 
2. LEI_deltas_vs_NBER_data: contrasts magnitude in LEI changes to NBER classification of "expansion" or "contraction" 
3. Four_stages_cycle: identifies the four stages of the cycle according to the patterns emerging from 1m, 3m and 6m changes in LEI
4. Cycle_vs_SP500: behavior of S&P 500 against the backdrop of the four stages of the economic cycle
5. Cycle_vs_CEI: behavior of CEI against the backdrop of the four stages of the economic cycle
6. Assets_correlation_all_stages: calculates correlations among all assets and betas against S&P 500
