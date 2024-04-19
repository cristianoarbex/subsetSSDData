 ## Data for the paper 
 
 This repository contains all data used to produce the results in the following paper:

<b><i>A SSD approach to enhanced indexation with sector constraints</i></b>

The following files are available:
 
 -  `marketData.csv`: A csv file containing prices for every asset in the S&P500 index, from end of 2018 to end of 2023. Each row represents a date and each columns an asset; assets are identifier by their ticker. A missing price means that either the price did not exist at the time or was not found. A negative price means that the asset was not part of the S&P500 at the time.
 -  `marketData_benchmarks.csv`: A csv file containing prices for the S&P500 index and all 11 sector subindices.
 -  `marketData_tags.csv`: A csv file containing the sector to which each asset belongs.
