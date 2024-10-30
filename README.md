 ## Data for the paper 
 
 This repository contains all data used to produce the results in the following paper:

<b><i>Subset SSD for enhanced indexation with sector constraints</i></b>

The following files are available:

 **US stocks data**
 
 -  `marketDataUS.csv`: A csv file containing prices for every asset in the S&P500 index, from the end of 2018 to the end of 2023. Each row represents a date and each columns an asset; assets are identifier by their ticker. A missing price means that either the price did not exist at the time or was not found. A negative price means that the asset was not part of the S&P500 at the time.
 -  `marketDataUS_benchmarks.csv`: A csv file containing prices for the S&P500 index and all 11 sector subindices.
 -  `marketDataUS_tags.csv`: A csv file containing the sector to which each asset belongs.

**Fama-French 49 industry portfolios**

 -  `marketDataFF.csv`: A csv file containing prices for every one of the 49 Fama-French industry portfolios, from the end of 2018 to the end of 2023. Each row represents a date and each columns an asset; assets are identifier by their ticker. A missing price means that the corresponding portfolio was not computed at the time. Note that the original data is given as daily returns, we computed prices assuming an initial price of $0.1 in 1926 (when the data begins) and compounded the returns accordingly.
 -  `marketDataFF_CRSP_benchmarks.csv`: A csv file containing prices for CRSP benchmarks, including the CRSP NYSE Value-Weighted Market Index (code: CRSPVWMI) and the CRSP US sector indices.
 -  `marketDataFF_EW_benchmarks.csv`: A csv file containing prices for the equally-weighted benchmarks as calculated in our paper, including the equally-weighted benchmark of all 49 portfolios (code: EW) and the equally-weighted sector indices.
 -  `marketDataFF_tags.csv`: A csv file containing the sector to which each portfolio belongs, as classified by us. Note that since `real estate` is a single portfolio, it was put into the financials sector. So effectivelly there are 10 Fama-French sectors instead of 11 as above in the US data.

In the paper, the experiments were run from 2018-12-31 until 2023-12-31. Every rebalance uses 60-days of historical returns ending at the day of the rebalance, hence the data also includes 60 prices prior to 2018-12-31.
