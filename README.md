# Stock Clustering

### Objective
Utilizing the clustering algorithm, we target on the performance of stocks price to statistically understand the stock market with identification of the "similar" stock clusters and informed decision making on the future performance of stock clusters.

### Data
Top 100 company in S&P500
Price value are taken from the Yahoo! historical quotes API
Reason:
- a. representative cross-section of stocks;
- b. have a very large trading volume;
- c. general long-tern trend;
- d.in-sector volatility

### Methodology
Stock Performance(variance)=close price-open price  ---- standardized stock variance
GraphLassoCV - Get the covariance value based on the time series of stock variance
Affinity Propagation - Do not need to provide number of clusters; cluster size is not same
Rand Index - Evaluate the clusters with different length of period in clusters
              Identify the stable clusters

### Visualization
