# Machine-Learning-in-Assset-Pricing-Scholarly-Papers-with-Notes
This repo contains the list and a constructive summary of seminal and important scholarly research papers in the area of Machine Learning in Asset Pricing. 
This purpose of this initiative to provide a conmphesive repo for the subject area. For interactive reading experience do visit this repo’s [**GitHub Page**](https://ajim63.github.io/Machine-Learning-in-Asset-Pricing-Papers/). If you like the repo, please star. This motivates us to update the repo frequently.



## Asset Return Predication

| **Paper**   | **Summary** | **Data**   | **Issues**     |
| ---     | ---     |  ---   |   ---      |
|[Gu, Shihao, Bryan Kelly, and Dacheng Xiu. "Autoencoder asset pricing models." Journal of Econometrics 222, no. 1 (2021): 429-450.](https://www.sciencedirect.com/science/article/pii/S0304407620301998) |Add Summary|  <ul><li> 94 characteristics29 (61 of which are updated annually, 13 are updated quarterly, and 20 are updated monthly) </li> <li> 74 industry dummies corresponding to the first two digits of SIC codes </li> <li> Eight macroeconomic predictors </li> <li> </ul> |
|[Gu, Shihao, Bryan Kelly, and Dacheng Xiu. "Empirical asset pricing via machine learning." The Review of Financial Studies 33, no. 5 (2020): 2223-2273](https://academic.oup.com/rfs/article/33/5/2223/5758276) |Add Summary|  <ul><li> 94 characteristics29 (61 of which are updated annually, 13 are updated quarterly, and 20 are updated monthly) </li> <li> 74 industry dummies corresponding to the first two digits of SIC codes </li> <li> Eight macroeconomic predictors </li> <li>  $x_{i,t} \otimes c_{i,t}$ Total $94×(8+1)+74=920$</ul> |
|   [Chen, Luyang, Markus Pelger, and Jason Zhu. "Deep learning in asset pricing." Management Science (2023)](https://pubsonline.informs.org/doi/full/10.1287/mnsc.2023.4695?casa_token=diOIUo7s9XcAAAAA%3Alo9f4mKnjbsQtbvR28zS6n9hipGDYRP_xTLSgvbe0s7tuFoJzEJU72wEjULvUTJOeu_weS_ymq5N)      |    This paper proposes a GAN based deep learning   model for moeling stock return. The authors craftully connect no arbitrage condition for asset pricing with deep learning. In sort, they use generative adversarial network to find SDF stochastic discount factor. Where the asset pricing modeler wants to choose an asset pricing model, whereas the adversary wants to choose conditions under which the asset pricing model performs badly. In each iteration, the advarsary select the moment conditions that lead to the largest mispricing, and the modeler revise the candidate SDF to encorporate the identifed factor . In addition, they use LSTM and take the final output layer as a summarized state of the time varing macroeconomic condition  |   46 time-varying, firm-specific characteristics and 178 macroeconomic time series     |            |
|[Leippold, Markus, Qian Wang, and Wenyu Zhou. "Machine learning in the Chinese stock market." Journal of Financial Economics 145, no. 2 (2022): 64-82](https://www.sciencedirect.com/science/article/pii/S0304405X21003743)  |         |        |            |




 # Machine Learning and Finance — Literature Review

This document provides a structured index of key scholarly papers exploring the intersection of **machine learning**, **asset pricing**, and **financial economics**.  
Each entry includes a brief overview, data description, limitations, and suggestions for future research.

<style>
/* --- Professional collapsible styling --- */
details {{
  background-color: #f8f9fa;
  border: 1px solid #d1d1d1;
  border-radius: 6px;
  padding: 0.6em 1em;
  margin-top: 0.5em;
  margin-bottom: 1em;
  transition: all 0.3s ease;
}}

details:hover {{
  background-color: #f0f0f0;
}}

summary {{
  font-weight: 600;
  color: #1a1a1a;
  cursor: pointer;
}}

.content-block {{
  margin-top: 0.5em;
  color: #333;
  line-height: 1.55;
  font-size: 0.96em;
}}

hr.section {{
  border: none;
  height: 1px;
  background-color: #ddd;
  margin: 2em 0;
}}
</style>

<hr class="section">

### [Gu, Shihao, Bryan Kelly, and Dacheng Xiu. Autoencoder asset pricing models. Journal of Econometrics (2021).](https://www.sciencedirect.com/science/article/abs/pii/S0304407620301998 ; SSRN: https://ssrn.com/abstract=3335536)
**Year:** 2021  **Category:** Factor discovery / representation learning/Latent factor models


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Introduces a conditional autoencoder that learns low-dimensional latent factors and nonlinear factor loadings from firm characteristics. The model improves out-of-sample pricing and produces smaller pricing errors than many linear methods (e.g., IPCA) while allowing flexible nonlinear exposures.</p>
    <p><strong>Data Used:</strong> March 1957 (the start date of the S&P 500) and ends in December 2016, totaling 60 years. 
94 characteristics (61 of which are updated annually, 13 updated quarterly, and 20
updated monthly).
rank-normalize all characteristics into the interval (−1, 1)
any filters based on stock prices or share codes, or rule out financial
firms. Past literature has imposed these filters in large part because they find it difficult to reconcile the return behavior
of low-price stocks, uncommon share codes, and financial sector stocks with the rest of the sample
Median imputation throughout the dataset so they have the full range of 30000 company data.</p>
    <p><strong>Challenges / Limitations:</strong> - Model interpretability: learned latent factors are nonlinear and harder to economically interpret.
- Overfitting risk if not carefully regularized or validated (autoencoders can memorize noise).
- Requires large cross-sectional and time-series data; performance may degrade for smaller markets.</p>
    <p><strong>Future Research Directions:</strong> - Develop methods to map learned latent factors to economic primitives (interpretability tools).
- Extend to multi-asset settings (bonds, options) and mixed-frequency data.
- Robustness checks under transaction costs and limits-to-arbitrage constraints.</p>
  </div>
</details>


<hr class="section">

### [Gu, Shihao, Bryan Kelly, and Dacheng Xiu. Empirical asset pricing via machine learning. Review of Financial Studies (2020).](https://doi.org/10.1093/rfs/hhaa009 ; SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3159577)
**Year:** 2020  **Category:** Prediction / forecasting


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> A systematic comparison of machine learning methods for asset pricing problems (predicting risk premia and the cross-section). Finds tree-based and neural-network methods often outperform linear benchmarks; shows nonlinear interactions and model selection matter for economic gains. </p>
    <p><strong>Data Used:</strong> 94 characteristics (61 of which are updated annually, 13 updated quarterly, and 20
updated monthly).
8 Macroeconomic predictors that are aggregated time
series variables.
Average number of stocks per month exceeding 6200
Treasury bill rate to proxy the risk-free rate from
which the individual excess returns are calculated.</p>
    <p><strong>Challenges / Limitations:</strong> - Economic interpretation of ML signals is limited‚Äîhard to link to risk-based primitives.
- ML strategies may rely heavily on small or illiquid stocks (limits-to-arbitrage concerns).
- High turnover and transaction costs often not fully accounted for in economic evaluation.</p>
    <p><strong>Future Research Directions:</strong> - Combine ML with economic restrictions/prior structure to improve interpretability and robustness.
- Study long-run stability and publication-date effects (post-publication alpha decay).
- Integrate alternative data sources (text, high-frequency) in a unified ML framework.</p>
  </div>
</details>


<hr class="section">

### [Chen, Luyang, Markus Pelger, and Jason Zhu. Deep learning in asset pricing. Management Science (2023).](https://doi.org/10.1287/mnsc.2023.4695 ; arXiv: https://arxiv.org/abs/1904.00745)
**Year:** 2023  **Category:** SDF estimation / deep learning


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Estimates a stochastic discount factor (SDF) with deep neural networks using a no-arbitrage loss and an adversarial construction of test assets. Proposes a deep neural-network-based approach to estimate asset-pricing models that enforces no-arbitrage and uses adversarially chosen test assets. The method extracts latent economic states from macro variables and delivers improved out-of-sample pricing and Sharpe ratios compared to benchmarks.  </p>
    <p><strong>Data Used:</strong> Firm-level returns (CRSP), Compustat, macroeconomic time series; constructs test assets via adversarial selection.</p>
    <p><strong>Challenges / Limitations:</strong> - Complex training objectives (no-arbitrage plus adversarial tasks) can be sensitive to hyperparameters.
- Interpretability of deep networks remains limited; mapping to economic states is empirical rather than structural.
- Computational intensity and reproducibility concerns for large-scale implementations.</p>
    <p><strong>Future Research Directions:</strong> Develop diagnostics that connect learned states to macroeconomic fundamentals.
- Simplify/adapt the adversarial testing procedure for robust application across markets.
- Extend framework to multi-period choices and general equilibrium settings.</p>
  </div>
</details>


<hr class="section">

### [Leippold, Markus, Qian Wang, and Wenyu Zhou. Machine learning in the Chinese stock market. Journal of Financial Economics (2022).](https://doi.org/10.1016/j.jfineco.2021.08.017 ; SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3754339)
**Year:** 2022  **Category:** Prediction / forecasting (market-specific)


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Applies ML methods to the Chinese stock market to build return-prediction models and factors. Finds liquidity-related predictors and retail-investor effects important; emphasizes transaction-cost considerations.</p>
    <p><strong>Data Used:</strong> Daily and monthly total stock returns for all A share stocks listed in Shanghai and Shenzhen stock exchanges from the Wind Database (3900 stocks over a time period of 20 years). yield rate for the one year govt bond in China from CMAR to proxy fopr the risk free rate which is necessary for cvalculating individual excess returns. 94 stock level characteristics (4 are valid chinese specific factors), binary vbariables (4) that indicate ownership types. cross sectional ranking and maping them between -1 and 1 to avoid the effect of outliers along with 80 industry dummies. 11 macroeconomic predictors.</p>
    <p><strong>Challenges / Limitations:</strong> Unique market microstructure (retail dominance) reduces direct transferability of U.S. ML results.
- Transaction costs and short-sale constraints can materially reduce implementable profits.
- Data access and quality in emerging/segmented markets can hamper replication.</p>
    <p><strong>Future Research Directions:</strong>  Adjust ML pipelines for market microstructure and retail behavior when porting methods across countries.
- Investigate robustness to trading frictions and alternative liquidity measures.
- Use high-frequency trade-level data to better capture retail vs institutional dynamics.</p>
  </div>
</details>


<hr class="section">

### [Aubry, Mathieu, Roman Kräussl, Gustavo Manso, and Christophe Spaenjers. "Biased auctioneers." The Journal of Finance (2023).](https://onlinelibrary.wiley.com/doi/full/10.1111/jofi.13203)
**Year:** 2023  **Category:** Alternative data / computer vision (asset pricing application)


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Uses neural-network based image and metadata analysis to predict art auction prices and documents systematic auctioneer biases in pricing. Combines visual and non-visual features.</p>
    <p><strong>Data Used:</strong> Proprietary data from Blouin Art Sales Index, has information on buyins and data from 2008 to 2015 (2015 as the test set). 1,2 mil lots, 130k individual artists. Has inmformation about the artist, the artwork, the auction. The amounts are converted to USD using a spot rate at the time of sale and also a high quality image of the artwork for analysis.</p>
    <p><strong>Challenges / Limitations:</strong> External validity: art markets are niche and results may not generalize to other asset classes.
- Image-based valuation models can be sensitive to sample selection and feature extraction choices.
- Causality: disentangling information effects vs. behavioral reactions to published estimates.</p>
    <p><strong>Future Research Directions:</strong> - Explore ML valuation feedback loops across other illiquid markets (collectibles, real estate).
- Use experimental settings to test causal mechanisms behind auctioneer bias.
- Combine alternative data (provenance, exhibition history) with image features.</p>
  </div>
</details>


<hr class="section">

### [Avramov, Cheng, & Metzker. Machine Learning versus Economic Restrictions: Evidence from Stock Return Predictability. Management Science (2023).](SSRN / Management Science: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3450322 ; DOI via Management Science)
**Year:** 2023  **Category:** Prediction / economic restrictions


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Reassesses ML-based predictability claims and shows that imposing economically motivated restrictions (exclude microcaps, distressed stocks, apply trading-cost filters) substantially reduces reported ML profitability. Highlights the importance of realistic economic constraints when evaluating ML strategies. Compares unconstrained ML methods against models with economic restrictions. Finds ML picks up profit mainly from difficult-to-arbitrage stocks and that realistic frictions attenuate economic gains.</p>
    <p><strong>Data Used:</strong> U.S. stock returns and characteristics; check paper for full data appendix.</p>
    <p><strong>Challenges / Limitations:</strong> Demonstrates sensitivity to sample selection—raises questions about prior ML economic gains.
- Quantifying realistic trading costs and market impact remains challenging.
- Findings depend on choices around universes (microcaps, penny stocks) and data snooping risks.</p>
    <p><strong>Future Research Directions:</strong> Systematically integrate limits-to-arbitrage and market impact into ML evaluation pipelines.
- Develop standardized robustness checks (economic restrictions) for ML-based asset-pricing studies.
- Reexamine published ML results under matched economic constraint protocols.</p>
  </div>
</details>


<hr class="section">

### [Azimi, M., & Agrawal, A. Is Positive Sentiment in Corporate Annual Reports Informative? Evidence from Deep Learning. Review of Asset Pricing Studies (2021).](https://doi.org/10.1093/rapstu/raab005 ; SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3258821)
**Year:** 2021  **Category:** Alternative data / NLP


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Applies deep-learning-based sentiment extraction to 10-K filings and finds both positive and negative sentiments predict abnormal returns and future firm fundamentals around filing dates. Shows finer-grained sentiment measures (vs. simple net-sentiment) contain incremental information. </p>
    <p><strong>Data Used:</strong> EDGAR 10-K filings for U.S. firms, stock returns around filing dates, and firm fundamentals.</p>
    <p><strong>Challenges / Limitations:</strong> Text-sentiment models require careful training and can be sensitive to label noise.
- Filing-based signals can be confounded by concurrent announcements or news.
- Generalizing across jurisdictions/time requires retraining sentiment models.</p>
    <p><strong>Future Research Directions:</strong> `- Event-level causal identification strategies (e.g., instrumental variables).
- Cross-sectional tests across industries and international filings.
- Release trained models and preprocessing code for reproducibility.  Incorporate multi-modal data (text + earnings calls + management forecasts) for richer signals.
- Test long-horizon predictive power and economic exploitability after costs.
- Explore causal mechanisms linking narrative tone to firm fundamentals. </p>
  </div>
</details>


<hr class="section">

### [Bali, Goyal, Huang, Jiang, & Wen. The Cross-Sectional Pricing of Corporate Bonds Using Big Data and Machine Learning. (2020).](Working paper / SSRN / SFI links (see paper): https://ideas.repec.org/p/chf/rpseri/rp20110.html ; SSRN entry)
**Year:** 2020  **Category:** Fixed income / prediction


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Applies ML to predict cross-sectional corporate bond returns using a large set of equity and bond characteristics and finds ML methods improve out-of-sample predictive power; imposing economic structure (Merton) helps.</p>
    <p><strong>Data Used:</strong> TRACE transaction-level data for bonds (US), firm equity characteristics, bond fundamentals (see paper for details).</p>
    <p><strong>Challenges / Limitations:</strong> - Fixed-coupon securities have special features (callability, illiquidity) requiring careful modeling.
- Corporate bond datasets are noisier and sparser than equities -> potential overfitting.
- Transaction costs and dealer intermediation dynamics complicate implementability.</p>
    <p><strong>Future Research Directions:</strong> - Combine structural credit models (Merton-style) with ML for improved interpretability.
- Incorporate dealer-level microstructure and liquidity supply measures.
- Test international bond markets and municipal/corporate subsegments.</p>
  </div>
</details>


<hr class="section">

### [Bao, Ke, Li, Yu, & Zhang. Detecting Accounting Fraud in Publicly Traded U.S. Firms Using a Machine Learning Approach. Journal of Accounting Research (2020).](https://onlinelibrary.wiley.com/doi/full/10.1111/1475-679X.12292)
**Year:** 2020  **Category:** Accounting / fraud detection (ML applied)


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Uses ML classifiers to detect accounting fraud in US firms, leveraging financial statement features and textual signals; reports improved detection relative to standard benchmarks.</p>
    <p><strong>Data Used:</strong> Compustat/CRSP financials, audit reports, possibly text of filings; see paper for dataset and labeling procedure.</p>
    <p><strong>Challenges / Limitations:</strong> Label quality: fraud/misstatement labels are noisy and subject to detection biases.
- Class imbalance (fraud events are rare) complicates training and evaluation.
- Potential adverse incentives if algorithms are used operationally without human oversight.</p>
    <p><strong>Future Research Directions:</strong> - Develop causal/interpretability tools to explain flagged cases to auditors.
- Use multi-source signals (text, network, alternative data) to improve robustness.
- Evaluate real-world deployment impacts on audit selection and false-positive costs.</p>
  </div>
</details>


<hr class="section">

### [Bertomeu, Cheynel, Floyd, & Pan. Using machine learning to detect misstatements. Review of Accounting Studies (2020).](https://link.springer.com/article/10.1007/s11142-020-09563-8)
**Year:** 2020  **Category:** Accounting / misstatement detection


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Applies various ML methods to detect financial misstatements and misreporting, comparing performance to traditional models and highlighting useful features.</p>
    <p><strong>Data Used:</strong> Financial statement data and enforcement/SEC restatement records; see paper for details.</p>
    <p><strong>Challenges / Limitations:</strong> - False positives have real costs; need to balance precision vs recall in operational settings.
- Heterogeneity across firms/industries may reduce generalization of trained models.
- Regulatory and privacy constraints limit access to rich features in practice.</p>
    <p><strong>Future Research Directions:</strong> Better calibration and cost-sensitive learning tailored to audit priorities.
- Cross-firm transfer learning to improve small-sample performance.
- Integrate explainable AI for audit trail documentation.</p>
  </div>
</details>


<hr class="section">

### [Bianchi, Daniele, Matthias Büchner, and Andrea Tamoni. "Bond risk premiums with machine learning." The Review of Financial Studies 34, no. 2 (2021): 1046-1089.](https://academic.oup.com/rfs/article-abstract/34/2/1046/5843806?redirectedFrom=fulltext)
**Year:** 2020  **Category:** Fixed income / macro-finance


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Uses ML tools (extreme trees, NNs) to model bond risk premia and documents improved prediction and economic gains relative to linear models. Highlights macro-financial predictors and nonlinear interactions important for bond premia.</p>
    <p><strong>Data Used:</strong> Bond yields, macro variables, and bond-level characteristics (see paper for exact dataset).</p>
    <p><strong>Challenges / Limitations:</strong> - Bond markets' low-frequency and illiquidity challenge model training and evaluation.
- Interpreting macro-driven nonlinear patterns in economic terms is non-trivial.
- Out-of-sample stability in stressed environments needs further testing.</p>
    <p><strong>Future Research Directions:</strong> - Integrate term-structure theory constraints into ML algorithms for better interpretability.
- Test ML models across different bond sectors (sovereign, municipal, corporate).
- Assess performance during crisis episodes and regimes.</p>
  </div>
</details>


<hr class="section">

### [Bianchi & McAlinn. Divide and Conquer: Financial Ratios and Industry Returns Predictability. SSRN (2020).](SSRN: https://ssrn.com/abstract=3136368)
**Year:** 2020  **Category:** Prediction / industry-focused methods


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Proposes an ensemble 'divide-and-conquer' approach that groups predictors into small-scale linear models and ensembles them to capture rich information while controlling overfitting. Shows improved predictability of industry returns versus monolithic high-dimensional models. </p>
    <p><strong>Data Used:</strong> Industry-level returns, firm financial ratios, and sector classifications; see SSRN paper for details.</p>
    <p><strong>Challenges / Limitations:</strong> Choice of grouping/ensembling may be ad-hoc and require domain knowledge.
- Performance depends on stability of ratio-industry relationships through time.
- Relies on high-quality, industry-level financial data which may be noisy.</p>
    <p><strong>Future Research Directions:</strong> Automate grouping with hierarchical clustering or Bayesian grouping priors.
- Combine with causal feature selection to improve robustness.
- Test in international samples and cross-asset contexts.</p>
  </div>
</details>


<hr class="section">

