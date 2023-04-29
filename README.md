# Machine-Learning-in-Assset-Pricing-Scholarly-Papers-with-Notes
This repo contains the list and a constructive summary of seminal and important scholarly research papers in the area of Machine Learning in Asset Pricing. 
This purpose of this initiative to provide a conmphesive repo for the subject area. For interactive reading experience do visit this repo’s [**GitHub Page**](https://ajim63.github.io/Machine-Learning-in-Asset-Pricing-Papers/). If you like the repo, please star. This motivates us to update the repo frequently.



## Asset Return Predication
| Paper   | Summary | Data   | Issues     |
| ---     | ---     |  ---   |   ---      |
|[Gu, Shihao, Bryan Kelly, and Dacheng Xiu. "Autoencoder asset pricing models." Journal of Econometrics 222, no. 1 (2021): 429-450.](https://www.sciencedirect.com/science/article/pii/S0304407620301998) |Add Summary|  <ul><li> 94 characteristics29 (61 of which are updated annually, 13 are updated quarterly, and 20 are updated monthly) </li> <li> 74 industry dummies corresponding to the first two digits of SIC codes </li> <li> Eight macroeconomic predictors </li> <li> </ul> |


|[Gu, Shihao, Bryan Kelly, and Dacheng Xiu. "Empirical asset pricing via machine learning." The Review of Financial Studies 33, no. 5 (2020): 2223-2273](https://academic.oup.com/rfs/article/33/5/2223/5758276) |Add Summary|  <ul><li> 94 characteristics29 (61 of which are updated annually, 13 are updated quarterly, and 20 are updated monthly) </li> <li> 74 industry dummies corresponding to the first two digits of SIC codes </li> <li> Eight macroeconomic predictors </li> <li> $ x_{i,t} \otimes c_{i,t} $ Total 94×(8+1)+74=920 </ul> 

|   [Chen, Luyang, Markus Pelger, and Jason Zhu. "Deep learning in asset pricing." Management Science (2023)](https://pubsonline.informs.org/doi/full/10.1287/mnsc.2023.4695?casa_token=diOIUo7s9XcAAAAA%3Alo9f4mKnjbsQtbvR28zS6n9hipGDYRP_xTLSgvbe0s7tuFoJzEJU72wEjULvUTJOeu_weS_ymq5N)      |    This paper proposes a GAN based deep learning   model for moeling stock return. The authors craftully connect no arbitrage condition for asset pricing with deep learning. In sort, they use generative adversarial network to find SDF stochastic discount factor. Where the asset pricing modeler wants to choose an asset pricing model, whereas the adversary wants to choose conditions under which the asset pricing model performs badly. In each iteration, the advarsary select the moment conditions that lead to the largest mispricing, and the modeler revise the candidate SDF to encorporate the identifed factor . In addition, they use LSTM and take the final output layer as a summarized state of the time varing macroeconomic condition  |   46 time-varying, firm-specific characteristics and 178 macroeconomic time series     |            | 
|[Leippold, Markus, Qian Wang, and Wenyu Zhou. "Machine learning in the Chinese stock market." Journal of Financial Economics 145, no. 2 (2022): 64-82] (https://www.sciencedirect.com/science/article/pii/S0304405X21003743)  |         |        |            |
