# Project 4: Causal Inference

### [Project Description](doc/project4_desc.md)

Term: Spring 2021

+ Team Group4
+ Projec title: Causal Inference
+ Team members
	+ Cao, Jingbin: jc5514@columbia.edu
	+ Chen, Pin-Chun: pc2939@columbia.edu
	+ Gosmant, Aurore: apg2170@columbia.edu
	+ Song, Weiwei: ws2621@columbia.edu
	+ Zhuang, Zikun: zz2762@columbia.edu   

+ Project summary:  
In this project, we compare Inverse Propensity Weighting (PS: Logistic Regression), Regression Estimate (doesn't need PS), Stratification (PS: Logistic Regression), and Regression Adjustment (PS: Logistic Regression).

Performance -

| Low Dim. Dataset |
| Algorithm      |Computational Cost| Performance (Squared Error) |
| ----------- | ----------- | ------    |
| Inverse Propensity Weighting (IPW) + Logistic Regression     |  0    |  0.6331     |
| Regression Estimate (Dont need Propensity Score)      |  0.013      |   0.1872   |
| Stratification + Logistic Regressionn      |   0.008    |   0.2524   |
| Regression Adjustment + Logistic Regressionn      |  0.001    |   0.5727    |


| High Dim. Dataset |
| Algorithm      |Computational Cost| Performance (Squared Error) |
| ----------- | ----------- | ------    |
| Inverse Propensity Weighting (IPW) + Logistic Regression     |  0.004    |  1.6484     |
| Regression Estimate (Dont need Propensity Score)      |  0.179      |   1.6034   |
| Stratification + Logistic Regressionn      |   0.064    |   2.0325    |
| Regression Adjustment + Logistic Regressionn      |   0.001    |   2.1356    |

+ Project Conclusion:  
Among four different algorithms, Regression Estimate has the best performances with both high and low dimension datasets since it has the lowest squared errors in both cases. However, Regression Adjustment algorithm will take more computational cost than other algorithms (longer run-time). Besides, the squared errors for high dimensional dataset are all larger than the squared errors of low dimensional dataset for all four algorithms. In terms of computational cost, for Regression Estimate and Stratification (with LR), the run-times of high dimensional dataset is longer than the run-times for low dimensional dataset, but for Regression Adjustment (with LR) and IPW (with LR), the run-times of both datasets are similar. However, since the run-times for all four algorithms are lower than 0.18 seconds even when calculating the ATE for high dimentianl dataset, we can ignore their differences in computational costs. Therefore, we think Regression Estimate is the best algorithm when estimating the ATE of both datasets.  

+ Here are some useful graphs that we constructed from this project:
![ATE Comparison (Low Dim)](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/ATE.jpeg)
![Performance Comparison](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/performance.jpeg)
![Runtime Comparison](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/runtime.jpeg)
![PS Low](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/ps_low.jpeg)
![PS High](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/ps_high.jpeg)

**Contribution statement**:  

Zikun Zhuang - be responsible for algorithm 1 - Inverse Propensity Weighting and Logistic Regression.  

Pin-Chun Chen - be responsible for algorithm 3 - Stratification and Logistic Regression, implemented the parameter “k” as the strata for the visualization.   

Jingbin Cao - be responsible for algorithm 2 - Regression Estimate; structured the Rmd file; worte Propensity Scores, wrote Model Comparisons, wrote Conclusion, wrote Starter-Code for all visualization graphs, and wrote Readme file.  

Weiwei Song - be responsible for algorithm 4 - Regression Estimate and Logistic Regression.  

Aurore Gosmant - Responsible for the formatting of the visualizations graphs, relating the project to a concrete medical research case and presentations slides.  


Following [suggestions](http://nicercode.github.io/blog/2013-04-05-projects/) by [RICH FITZJOHN](http://nicercode.github.io/about/#Team) (@richfitz). This folder is orgarnized as follows.

```
proj/
├── lib/
├── data/
├── doc/
├── figs/
└── output/
```

Please see each subfolder for a README file.
