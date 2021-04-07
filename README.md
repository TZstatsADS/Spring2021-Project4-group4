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

+ Project summary:  Pairing Combination: 10,15,16,22. Compare Inverse Propensity Weighting (PS: Logistic Regression), Regression Estimate (doesn't need PS), Stratification (PS: Logistic Regression), and Regression Adjustment (PS: Logistic Regression).

Performance -

| Low Dim. Dataset |
| Algorithm      |Computational Cost| Performance (Squared Error) |
| ----------- | ----------- | ------    |
| Inverse Propensity Weighting (IPW) + Logistic Regression     |  0    |  0.6331     |
| Regression Adjustment + Logistic Regressionn      |  0.001    |   0.5727    |
| Regression Estimate (Dont need Propensity Score)      |  0.012      |   0.1872   |
| Stratification + Logistic Regressionn      |   0.007    |   0.2524   |


| High Dim. Dataset |
| Algorithm      |Computational Cost| Performance (Squared Error) |
| ----------- | ----------- | ------    |
| Inverse Propensity Weighting (IPW) + Logistic Regression     |  0.0009    |  1.6484     |
| Regression Adjustment + Logistic Regressionn      |   0.0010    |   2.1356    |
| Regression Estimate (Dont need Propensity Score)      |  0.1825      |   1.6034   |
| Stratification + Logistic Regressionn      |   0.0727    |   2.0325    |

Here are some useful graphs that we constructed from this project:
![ATE Comparison (Low Dim)](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/ATE.jpeg)
![Performance Comparison](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/performance.jpeg)
![Runtime Comparison](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/runtime.jpeg)
![PS Low](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/ps_low.jpeg)
![PS High](https://github.com/TZstatsADS/Spring2021-Project4-project5_group4/blob/main/figs/ps_high.jpeg)

**Contribution statement**: Waiting to upload

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
