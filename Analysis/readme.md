# Analysis

This folder contains the necessary pyhton notebooks to conduct the analysis. These were written for Google Colaboratory and might need certain adjustments when loading the data locally using Jupyter Notebook like eliminating the file.upload() method and pointing directly to the local directory in the read_csv() function.  

## Methodology
Using the Leading Economic Index produced by the Conference Board, I identify patterns in monthly, quarterly and semi-annual changes in the index, as well as in the magnitude of the semi-annual changes, to classify each month into one of the four stages of the economic cycle. I contrast this classification with NBER's determination of contraction and expansion periods. I use this backdrop to estimate the average returns of each asset during each stage and estimate the correlations among assets to choose a shifting optimized portafolio across stages.   

## List of notebooks
1. Generating_Economic_Dataset: calculates 1m, 3m and 6m changes in the LEI and the signs of those changes to create a new dataset. 
2. Determining_Cycle_Stage: 
3. Cycle_vs_SP500:
4. Cycle_vs_LEI:
