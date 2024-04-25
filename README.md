 ## Data for the paper 
 
 This repository contains all data used to produce the results in the following paper:

<b><i>Subset SSD for enhanced indexation with sector constraints</i></b>

The following files are available:
 
 -  `marketData.csv`: A csv file containing prices for every asset in the S&P500 index, from end of 2018 to end of 2023. Each row represents a date and each columns an asset; assets are identifier by their ticker. A missing price means that either the price did not exist at the time or was not found. A negative price means that the asset was not part of the S&P500 at the time.
 -  `marketData_benchmarks.csv`: A csv file containing prices for the S&P500 index and all 11 sector subindices.
 -  `marketData_tags.csv`: A csv file containing the sector to which each asset belongs.

In the paper, the experiments were run from 2018-12-31 until 2023-12-31. Every rebalance uses 84-days of historical returns ending at the day of the rebalance, hence the data also includes 84 prices prior to 2018-12-31.
