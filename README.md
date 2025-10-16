# 🧠 Machine Learning in Asset Pricing — Literature Review



## Table of Contents

- [Alternative Data](#alternative-data)
- [Asset Pricing](#asset-pricing)
- [Forecasting](#forecasting)
- [Latent Factor Model](#latent-factor-model)
- [Microstructure](#microstructure)
- [NLP](#nlp)
- [Network](#network)
- [Survey](#survey)

---




## Alternative Data


---

### <a href="https://academic.oup.com/rfs/article/32/5/2021/5427775" target="_blank">Zhu, C. (2019). Big Data as a Governance Mechanism. The Review of Financial Studies, 32, 2021-2061.</a>
**Year:** 2019  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Zhu studies whether access to alternative 'big data' affects price informativeness and corporate governance. Greater big-data availability is associated with more informative prices and disciplining effects on managerial actions.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Firm-level governance & performance measures; proxies for alternative data adoption; stock price informativeness metrics.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Measuring firms’ access to alternative data relies on indirect proxies.
  - Causal identification is difficult due to unobserved firm differences.
  - Generalizability beyond large public firms is uncertain.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Use direct adoption measures via procurement records.
  - Apply difference-in-differences around adoption events.
  - Study real decision impacts and privacy implications.

  </div>
</details>



---

### <a href="https://www.nber.org/papers/w29048" target="_blank">Hu, A., & Ma, S. (2020). Persuading Investors: A Video-Based Study . SSRN Electronic Journal.</a>
**Year:** 2020  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Hu & Ma study how nonverbal and delivery-related features in pitch videos affect investor decisions, exploiting a large dataset of startup pitch videos (e.g., accelerator applications) merged with subsequent funding outcomes. They extract multimodal features from video — facial expressions, vocal tone, gestural dynamics — using computer-vision and audio-processing ML pipelines, and construct composite metrics of persuasiveness (warmth, passion, confidence). The authors then relate these quantified delivery features to investor actions (funding probability, amount) while controlling for textual content and firm fundamentals, isolating the incremental effect of presentation style. They find that positive delivery characteristics (enthusiasm, warmth) increase the likelihood of obtaining funding, but conditional on funding, those with excessive positivity may underperform later — suggesting a trade-off between persuasion and information quality. The paper carefully addresses selection concerns (which startups choose to publish videos) and shows robustness across different investor groups and pitch contexts. Methodologically, the work illustrates how modern ML tools for video/audio feature extraction can be rigorously combined with econometric designs to identify behavioral effects in financial settings. The authors also discuss privacy and ethical considerations around using video and biometric-like measures for economic decisions. The dataset and code usually accompany the working-paper release to facilitate replication.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Pitch videos from accelerators / crowdfunding platforms or VC pitch archives (raw video and audio).
  - Firm-level meta-data (founder characteristics, business descriptions) and subsequent funding outcomes (dates, amounts).
  - Preprocessing: face-tracking, voice-feature extraction (prosody), and natural-language transcripts (ASR) to separate delivery vs content.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Sample selection: startups that record and share video pitches may differ systematically from those that don’t.
  - Video/audio processing may be sensitive to recording quality, camera angle, and background noise, potentially biasing feature extraction.
  - Ethical/privacy issues: inferring traits from video may raise consent and fairness concerns if used in hiring/financing decisions.
  - Causal inference: while the paper controls for many observables, unobserved attributes correlated with both delivery style and success remain plausible.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Field experiments randomizing video exposure or coaching to test causal effects of delivery on investment decisions.
  - Cross-platform and cross-country tests to study cultural differences in delivery effectiveness.
  - Combine video-derived measures with investor-level heterogeneity (e.g., experience, risk aversion) to personalize persuasion models.\

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/pii/S0304405X21004566" target="_blank">Martin, I. W. R., & Nagel, S. (2021). Market efficiency in the age of big data. Journal of Financial Economics.</a>
**Year:** 2021  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Martin & Nagel analyze how the availability of massive, granular data interacts with market efficiency, arguing that bigger data can both uncover previously hidden predictive signals and accelerate their arbitrage away, affecting the dynamic of inefficiencies. They combine theoretical modeling with empirical tests that leverage expanded datasets (textual data, high-frequency microstructure, alternative indicators) to examine whether and how markets incorporate information from large-scale sources. The authors document that while big data can improve ex-ante predictability for certain short horizons, practical frictions (transaction costs, capacity limits, and crowding) prevent instant exploitation, thereby leaving room for economically meaningful persistence. They also show that big-data-driven strategies can amplify volatility during stress periods if many agents react to the same signals simultaneously. Martin & Nagel stress the importance of distinguishing statistical predictability from economic arbitrageability and propose measures for testing efficiency in presence of high-dimensional signals. Policy and market-design implications are discussed, including data-access asymmetries and platform effects. Overall, the contribution is to bring a balanced analytical framework to assess the impact of big data on finance, combining normative concerns with empirical evidence.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Diverse large datasets: textual news corpora, high-frequency trade data, alternative data (satellite, transaction), and standard return series for empirical illustrations.
  - Simulations and calibrated models to assess arbitrage dynamics.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Empirical results can be sensitive to the particular big-data sources selected.
  - Measuring “arbitrageability” in practice requires strong assumptions about agents’ strategies and capacity.
  - Policy recommendations depend on regulatory and market-structure specifics.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Empirical work quantifying data-access inequality and its implications for market fairness.
  - Experiments on how coordinated use of common alternative-data signals affects volatility and liquidity.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article-abstract/34/7/3226/6239715?redirectedFrom=fulltext" target="_blank">Erel, I., Stern, L. H., Tan, C., & Weisbach, M. S. (2021). Selecting Directors Using Machine Learning. The Review of Financial Studies, 34, 3226-3264.</a>
**Year:** 2021  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  The authors apply machine-learning methods to predict director effectiveness and shareholder approval outcomes and compare algorithmic (ML-suggested) director slates with management’s choices. Their results suggest ML can identify director candidates more likely to gain shareholder approval and who would perform better on certain outcome measures, highlighting biases in current selection practices.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Director candidate characteristics (demographics, experience, networks), director election outcomes, firm performance and governance data, possibly board-level covariates

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Outcome labels (e.g., “good director”) are noisy and depend on the performance metrics chosen.
  - ML predictions may reinforce existing biases if training labels or features reflect historical discrimination.
  - Practical adoption interacts with legal/regulatory constraints and firms’ governance incentives.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Fairness-aware ML for director selection (mitigate demographic or network-based bias).
  - Field experiments or pilot deployments to evaluate ML-assisted director search in practice.
  - Link predicted director characteristics to long-run corporate outcomes (beyond short-term approval)

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/abs/pii/S0304405X21003718" target="_blank">Edmans, A., Fernandez-Perez, A., Garel, A., & Indriawan, I. (2021). Music sentiment and stock returns around the world. Journal of Financial Economics.</a>
**Year:** 2021  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  he authors develop a language-free, continuous national sentiment measure based on the positivity of the most popular songs (music sentiment) and show it correlates with same-week equity returns and predicts subsequent returns in some horizons and markets. They provide evidence that music sentiment contains macro- and investor-sentiment information that is useful across countries because it bypasses language barriers.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Streaming / chart data on popular songs by country (song lists and lyrics/audio-derived sentiment measures), country-level stock returns and macro series

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Music consumption may proxy for many social/economic phenomena (e.g., leisure spending, cultural cycles) — causality is hard to establish.
  - Popular-music sampling may reflect biased demographics (younger listeners), limiting representativeness.
  - Measurement choices for music “positivity” (lyric vs. audio features) and song selection matter for results.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Use instrumental / natural-experiment designs to disentangle sentiment from real economic shocks.
  - Combine music sentiment with other alternative signals (news, social media) to form multimodal sentiment indices.
  - Test intra-country heterogeneity (regions, age groups) and impact on specific sectors.

  </div>
</details>



---

### <a href="https://www.aeaweb.org/articles?id=10.1257/aer.20201713" target="_blank">Bianchi, F., Ludvigson, S. C., & Ma, S. (2020). Belief Distortions and Macroeconomic Fluctuations. SSRN / NBER / AER.</a>
**Year:** 2022  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Combines survey data with ML to estimate time-varying belief distortions in professional forecasts and studies their macroeconomic consequences. Finds sizable distortions and shows they affect macro fluctuations and forecast errors.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Survey expectation data, macroeconomic time series, and asset returns (see paper appendix).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Identification: separating true belief distortions from model misspecification is delicate.
  - Dependence on survey construction and sample coverage for external validity.
  - Interpreting ML-derived distortions in structural macro models requires care.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Embed estimated distortion processes in structural DSGE models for policy analysis.
  - Apply methods to cross-country survey panels to study heterogeneity.
  - Explore real-time predictive uses for policy and asset allocation.

  </div>
</details>



---

### <a href="https://onlinelibrary.wiley.com/doi/full/10.1111/jofi.13203" target="_blank">Aubry, Mathieu, Roman Kräussl, Gustavo Manso, and Christophe Spaenjers. "Biased auctioneers." The Journal of Finance (2023).</a>
**Year:** 2023  **Category:** Alternative Data


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Uses neural-network based image and metadata analysis to predict art auction prices and documents systematic auctioneer biases in pricing. Combines visual and non-visual features.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Proprietary data from Blouin Art Sales Index, has information on buyins and data from 2008 to 2015 (2015 as the test set). 1,2 mil lots, 130k individual artists. Has inmformation about the artist, the artwork, the auction. The amounts are converted to USD using a spot rate at the time of sale and also a high quality image of the artwork for analysis.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - External validity: art markets are niche and results may not generalize to other asset classes.
  - Image-based valuation models can be sensitive to sample selection and feature extraction choices.
  - Causality: disentangling information effects vs. behavioral reactions to published estimates.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Explore ML valuation feedback loops across other illiquid markets (collectibles, real estate).
  - Use experimental settings to test causal mechanisms behind auctioneer bias.
  - Combine alternative data (provenance, exhibition history) with image features.

  </div>
</details>




## Asset Pricing


---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2740751" target="_blank">Moritz, B., & Zimmermann, T. (2016). Tree-Based Conditional Portfolio Sorts: The Relation between Past and Future Stock Returns. SSRN Electronic Journal.</a>
**Year:** 2016  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Moritz & Zimmermann develop tree-based conditional portfolio sorts as a nonparametric alternative to classical characteristic sorts, allowing for flexible partitioning of the sample by multiple conditioning variables. The method builds decision trees that segment stocks into bins according to predictive characteristics (momentum, size, value, etc.), and then examines future returns across the leaves to estimate conditional effects. This approach avoids arbitrary bin-count choices and allows discovery of interactions between characteristics (e.g., momentum matters more for small caps). They demonstrate that tree-based sorts can reveal richer cross-sectional patterns and improve economic interpretability by presenting decision rules for when certain anomalies are most potent. The authors validate the method by replicating canonical anomaly effects and uncovering new conditional relationships, and they provide out-of-sample performance checks to avoid overfitting. The paper also discusses statistical inference for tree-based sorts and how to incorporate transaction-cost considerations in practical portfolio formation. The method contributes a machine-learning flavored but interpretable approach to empirical asset pricing and anomaly exploration.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Firm characteristics (momentum, size, value, profitability) and subsequent returns (monthly CRSP/Compustat panels).
  - Cross-validation via rolling windows for out-of-sample tests.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Tree methods can be unstable; small changes in data can lead to different splits if not regularized.
  - Interpretability of deep trees decreases; pruning and ensemble considerations are important.
  - Transaction costs and liquidity constraints for small-cap leaves need careful handling.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Combine tree-based sorts with ensemble methods (random forests) to stabilize selection while retaining interpretability.
  - Apply the method to cross-asset settings (bonds, options) for conditional anomaly detection.

  </div>
</details>



---

### <a href="https://doi.org/10.1111/jofi.12733" target="_blank">Chinco, A., Clark‚ÄêJoseph, A. D., & Ye, M. (2018). Sparse Signals in the Cross‚ÄêSection of Returns. The Journal of Finance, 74, 449-492.</a>
**Year:** 2018  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Chinco, Clark-Joseph, and Ye explore how “sparse signals” — rare, short-lived predictors — can be identified and exploited in the cross-section of stock returns using penalized regression (LASSO). They argue that many predictive relationships may exist only fleetingly and across few stocks, so standard regressions fail to capture them. They apply LASSO on lagged returns from the full cross-section (many thousands of candidate predictors) to forecast one-minute-ahead returns. Their backtests show that the LASSO improves out-of-sample fit and implied Sharpe ratios relative to OLS, particularly by selecting a small subset of predictive stocks (sparsity). They document that the selected predictors often correspond to stocks that had news or earnings surprises, lending economic interpretation to the statistical picks. The results suggest that profitable short-horizon signals are seldom persistent and that successful forecasting relies on timely detection of transient effects. They carefully analyze the stability of selected signals (turnover, predicted persistence) and show performance degrades if signals last more than a few minutes. The study contributes to understanding how micro-level cross-sectional predictability can exist despite competition, by focusing on transient, sparse effects rather than long-persistent factors.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - High-frequency return data (1-minute returns) across many stocks (CRSP / exchange-level tick data).
  - Candidate predictors are the lagged returns of all individual stocks (i.e. broad cross-sectional lag structure).
  - They also draw on event/announcement data to validate whether selected predictors are linked to news-driven events.
  - Rolling windows for estimation, cross-validation and out-of-sample tests are crucial to avoid look-ahead bias.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - The success of LASSO depends on tuning of penalty parameter and model stability; results may vary across hyperparameter choices.
  - Short-lived signals are hard to trade in practice due to latency, transaction costs, and execution constraints.
  - The approach may miss more persistent or nonlinear signals not well captured by linear LASSO.
  - The method focuses on very short horizons; scalability to longer horizons is unclear.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Extend sparse-signal approach to incorporate nonlinear or interaction terms (e.g. sparse + machine-learning hybrids).
  - Test whether similar transient signals exist at intraday but longer horizons (e.g. 5–15 min).
  - Explore real-time implementation constraints (latency, market impact) and whether signals can survive in live trading.

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/abs/pii/S0304405X24000606" target="_blank">Kan, R., Wang, X., & Zheng, X. (2019). In-Sample and Out-of-Sample Sharpe Ratios of Multi-Factor Asset Pricing Models. Journal of Financial Economics</a>
**Year:** 2019  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Kan, Wang, and Zheng study how estimation error affects the empirical Sharpe ratios reported for factor-investing strategies, deriving exact finite-sample distributions (or analytic approximations) for in-sample and out-of-sample Sharpe ratios of portfolios formed from estimated factor models. They show that the in-sample Sharpe ratio is an upward-biased estimator of true out-of-sample performance due to estimation noise, and they provide corrections and distributional results that quantify this discrepancy. Using both analytic derivations and Monte-Carlo simulations, they illustrate how portfolio construction choices (e.g., using sample tangent portfolios vs constrained portfolios) alter the bias and variance of Sharpe estimates. The paper offers practical guidance on inference — recommending adjusted test statistics and confidence intervals for reported Sharpe ratios — which is crucial when comparing competing ML-driven factor models. They also explore the role of look-ahead bias, overfitting due to many candidate factors, and the need to account for parameter uncertainty in backtests. Empirical illustrations using canonical factor datasets demonstrate how naive in-sample Sharpe reporting can mislead practitioners. The theoretical results are useful for both researchers and portfolio managers to set realistic expectations for performance persistence.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - The paper is primarily theoretical / simulation-based but uses canonical factor/returns datasets in illustrations (CRSP returns, Fama–French factors) to show practical magnitudes of Sharpe biases.
  - Monte-Carlo experiments calibrate noise levels to realistic return volatilities.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - The analytic corrections rely on model assumptions (Gaussian returns, particular estimator distributions) that may not hold in heavy-tailed real-world returns.
  - Adjustments for Sharpe bias do not alone solve problems arising from data-snooping or model-selection over thousands of candidate signals.
  - Implementation requires accurate estimation of estimation risk parameters, which can be delicate in small samples.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Extend distributional corrections to heavy-tailed or time-varying return distributions.
  - Incorporate multiple-testing adjustments for large candidate-signal pools common in ML pipelines.
  - Link Sharpe-bias corrections to utility-based metrics to evaluate economic (not just statistical) significance.

  </div>
</details>



---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3726609" target="_blank">Liu, Y., Zhou, G., & Zhu, Y. (2020). Maximizing the Sharpe Ratio: A Genetic Programming Approach. SSRN Electronic Journal.</a>
**Year:** 2020  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Liu, Zhou, and Zhu use genetic-programming (GP) algorithms to evolve trading rules and portfolio-construction formulas that directly target maximizing Sharpe ratio rather than surrogate objective functions. The GP framework searches over a space of symbolic expressions combining standard technical indicators and fundamental signals, using evolutionary operators (mutation, crossover) to iteratively improve a population of candidate strategies under out-of-sample validation. The authors emphasize the need to use walk-forward optimization and strict holdout periods to avoid overfitting, and they incorporate penalty terms for turnover to control spurious short-term Sharpe boosts. Empirically, they show GP can discover interpretable, compact rules that rival or beat some black-box models on historical data, but they also stress that many discovered rules are fragile out-of-sample. The paper examines robustness to parameter settings and tests across multiple asset classes. It highlights that GP’s symbolic outputs can aid interpretability relative to deep nets, but also that GP requires careful regularization and computational budgets. The authors discuss how GP complements other ML methods in exploring the space of nonlinear trading rules with clear objective alignment.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Historical returns (intraday or daily depending on the experiments), technical indicators, and optional fundamental signals.
  - Walk-forward rolling windows used for validation to mimic realistic deployment.'

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - GP is computationally heavy and prone to overfitting without aggressive validation.
  - Strategies optimized for Sharpe may be sensitive to tail events that Sharpe does not penalize sufficiently.
  - Transaction-cost and capacity considerations can materially change results.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Multi-objective GP optimizing for Sharpe, drawdown, and turnover simultaneously.
  - Hybrid GP + ensemble methods combining symbolic rules with statistical learners.

  </div>
</details>



---

### <a href="Large set of firm characteristics, CRSP/Compustat; uses tree-based methods to construct basis assets." target="_blank">Bryzgalova, S., Pelger, M., & Zhu, J. (2020). Forest Through the Trees: Building Cross-Sections of Stock Returns. SSRN / Journal.</a>
**Year:** 2020  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Proposes a decision-tree-based method to construct a compact set of basis assets (test assets) from a large set of characteristics, improving cross-sectional modeling and interpretability. Combines ensemble tree approaches with financial-sorting intuition to produce robust cross-sections.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Large set of firm characteristics, CRSP/Compustat; uses tree-based methods to construct basis assets.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Construction of basis assets depends on algorithm choices and hyperparameters.
  - May be sensitive to correlated characteristics and changing economic regimes.
  - Translating constructed basis assets into economically meaningful factors requires post-hoc analysis.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Automate economic labeling of basis assets via post-hoc interpretability methods.
  - Apply approach to multi-asset cross-sections (bonds, options).
  - Study stability of basis assets across subsamples and crises.

  </div>
</details>



---

### <a href="https://doi.org/10.1016/j.finmar.2020.100588" target="_blank">Tobek, O., & Hronec, M. (2021). Does it pay to follow anomalies research? Machine learning approach with international evidence. Journal of Financial Markets, 56, 100588.</a>
**Year:** 2021  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Tobek and Hronec (2021) investigate whether investors can profit by systematically following newly published asset pricing anomalies. They apply machine learning models to a global dataset of stock returns and firm characteristics to assess anomaly persistence and decay. Using ensemble methods and regularization, the authors analyze how the publication of new anomalies influences future return predictability. They find that many anomalies exhibit declining profitability post-publication, suggesting market learning effects. ML algorithms identify combinations of anomalies that remain robust across regions and time. The study demonstrates that integrating ML allows more efficient anomaly selection and weighting than traditional portfolio sorts. Their results have implications for both academics and practitioners seeking to exploit cross-sectional return predictability. The paper extends the literature on data-mining bias and post-publication anomaly performance.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Global equity data from 40+ markets (MSCI and Datastream), anomaly signals from published academic papers, and firm characteristics from Compustat Global covering 1980–2018.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Potential survivorship bias in anomaly database.
  - ML models may implicitly learn from data-mined relationships.
  - Difficult to separate market adaptation from statistical noise.
  - High dimensionality requires strong regularization.
  - Model complexity limits economic interpretation.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Apply causal ML to distinguish learning effects from data snooping.
  - Explore dynamic anomaly portfolios with reinforcement learning.
  - Investigate anomaly interactions under transaction cost constraints.

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/abs/pii/S2452306222000016" target="_blank">Hafner, C. M., & Wang, L. (2022). Dynamic portfolio selection with sector-specific regularization. Econometrics and Statistics.</a>
**Year:** 2022  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Hafner & Wang develop a dynamic portfolio selection framework that explicitly incorporates sector structure into regularization and optimization, arguing that treating assets wholly independently loses useful grouping information. They propose penalty terms that shrink weight differences within sectors differently from those across sectors, and combine these with sparsity and transaction-cost controls to produce portfolios that are simultaneously stable, interpretable, and sector-aware. The model nests familiar benchmarks (equal-weighted portfolios, conditional-correlation shrinkage estimators) as special cases, allowing clear comparisons. Estimation proceeds with rolling-window updates and regularized sample covariances; the authors emphasize practical implementation details such as calibration of penalty parameters and use of cross-validation. Empirically, they show that sector-aware regularization improves out-of-sample risk-adjusted returns and reduces turnover relative to unconstrained dynamic optimization in a realistic U.S. equity sample. They also analyze the trade-off between targeting sector neutrality and extracting cross-sectional alpha, showing that sector penalties can reduce concentration risk while preserving economic signals. Robustness checks include alternative sector definitions and transaction-cost assumptions. Overall, the paper supplies both a principled econometric framework and a practical algorithm for portfolio managers who want to respect industry structure when applying dynamic allocation rules.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - U.S. equities (CRSP/Compustat identifiers commonly used for such studies), daily or monthly returns across a broad cross-section.
  - Industry / sector classification (GICS/NAICS) used to define sector groups.
  - Rolling-sample covariance estimates and historical return series to calibrate shrinkage and transaction-cost parameters. (Authors provide code or appendices on sample construction in their preprint.)

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Selection of sector taxonomy (GICS vs SIC) and granularity materially affects which cross-sectional patterns are treated as within- vs across-sector; results can be sensitive.
  - Choice and calibration of regularization parameters (within- vs between-sector shrinkage) requires careful cross-validation and may overfit in small samples.
  - The approach still depends on historical covariances which may not capture rapid regime shifts; regularization reduces but does not eliminate estimation risk.
  - Transaction-cost modeling is approximate — real-world execution, market impact, and liquidity constraints may change net performance.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Extend to multi-level grouping (industry → sector → region) with hierarchical regularization and automatic hyperparameter selection.
  - Integrate dynamic macro state variables to allow time-varying sector-shrinkage strength that adapts to crises.
  - Develop Bayesian or fully probabilistic sector-regularized portfolio estimators with posterior uncertainty for risk management.

  </div>
</details>



---

### <a href="https://onlinelibrary.wiley.com/doi/full/10.1111/jofi.13298" target="_blank">Kelly, liyan T., et al. (2023) The Virtue of Complexity in Machine Learning Portfolios. Journal of Finance</a>
**Year:** 2023  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Kelly and coauthors examine whether more complex ML models necessarily lead to better portfolio performance, revisiting conventional wisdom about bias–variance tradeoffs with evidence that, in some cases, larger model complexity (more variables or parameters) can continue to improve predictive power up to computational limits. They compare a taxonomy of model complexities — from simple linear models to deep ensembles — across return-prediction and portfolio-construction tasks using large feature sets. Their empirical pipeline stresses rigorous out-of-sample testing with transaction-cost aware performance metrics and stability diagnostics. The findings indicate that, under certain conditions (large, informative datasets; proper regularization; cross-fitting), complexity can be beneficial, but the gains often hinge on data scope and preprocessing. The authors are careful to show counter-examples where complexity leads to overfitting or where gains evaporate once real-world frictions are included. Additionally, the paper discusses theoretical explanations (double-descent phenomena) and the circumstances that make complexity attractive for finance. They also provide practical guidance on model selection, ensembling, and how to interpret the apparent benefits of complexity in light of turnover and implementation costs. The contribution is both empirical and conceptual, informing debates on whether financial ML should favor simpler, interpretable models or embrace larger, black-box architectures.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Large cross-sectional predictor panels (characteristics, macro variables) and historical returns (CRSP/Compustat).
  - Simulated and empirical experiments across multiple datasets to test scaling of complexity.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Results depend on datasets used; complex models benefit most when large, high-quality signals exist.
  - Implementation costs and model maintenance complexity are nontrivial for practitioners.
  - Interpretability and regulatory considerations may constrain usable model complexity.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Formalize conditions under which complexity aids predictive inference in finance (data-size thresholds, signal-to-noise regimes).
  - Explore robustness to structural breaks and regime shifts for large models.
  - Balance complexity benefits with explainability methods designed for portfolio managers.

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/pii/S0304405X23001770" target="_blank">DeMiguel, V., Gil-Bazo, J., Nogales, F. J., & A. P. Santos, A. (2021). Machine learning and fund characteristics help to select mutual funds with positive alpha. Journal of Financial Economics (2023)</a>
**Year:** 2023  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Applies ML methods to mutual-fund selection and constructs tradable long-only portfolios that earn positive out-of-sample alphas after accounting for costs in some specifications. Highlights the role of fund characteristics and robust cross-validation.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Survivorship and backfill biases in fund databases.
  - Net-of-fee performance varies across samples and time periods.
  - Transaction costs and capacity constraints matter for large allocations.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Use vintage-aware evaluation to avoid backfill bias.
  - Incorporate fund holdings and flows for richer predictive features.
  - Test across international fund universes.

  </div>
</details>



---

### Gopalakrishna, G. (2020). Asset Pricing with Realistic Crises Dynamics. SSRN
**Year:** 2024  **Category:** Asset Pricing


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  : Gopalakrishna constructs a macro-finance model featuring stochastic productivity for “experts” (intermediaries) and state-dependent exit of experts to generate amplified and persistent crisis dynamics. The model is calibrated to match features of real financial crises (large risk premia, output drops, slow recoveries) and shows how expert exit and productivity dynamics can create a net-worth trap and long-lasting distress.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Calibration to aggregate macroeconomic / financial moments (e.g., output, risk premia, intermediary turnover) — model is primarily theoretical with calibration to observed crisis features; numerical examples use aggregated macro/financial statistics.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Model calibration depends on selected moments and assumed parametric structures.
  - The structural assumptions (expert exit dynamics) may be difficult to identify directly from data.
  - As with many macro models, quantitative conclusions depend on calibration choices and omitted frictions.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Micro-level empirical validation using firm- or bank-level data on expert turnover and productivity.
  - Extend to richer financial networks and endogenous entry/exit mechanisms.
  - Policy experiments within the model (capital injections, resolution regimes) to evaluate interventions.

  </div>
</details>




## Forecasting


---

### Zhang, Z., Zohren, S., & Roberts, S. (2019). DeepLOB: Deep Convolutional Neural Networks for Limit Order Books. IEEE Transactions on Signal Processing, 1-1.
**Year:** 2019  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  DeepLOB proposes a CNN+LSTM architecture that learns spatial representations from LOB snapshots and temporal dependencies. It outperforms prior methods for short-horizon price-movement prediction.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Limit order book benchmark datasets; mid-price labels; short-horizon price movements.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Results may not translate to live trading.
  - Overfitting risk due to benchmark datasets.
  - Microstructure idiosyncrasies limit portability.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Evaluate with realistic transaction costs.
  - Extend with transformer architectures.
  - Combine with execution-aware objectives.

  </div>
</details>



---

### <a href="SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3424793" target="_blank">Borisenko, D. (2019). Dissecting Momentum: We Need to Go Deeper. SSRN.</a>
**Year:** 2019  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Argues that simple momentum strategies mask richer dynamics: deeper, state-dependent, and industry-specific drivers matter. Suggests using richer ML-style partitioning to uncover the conditional structure of momentum.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - U.S. stock returns and momentum-related characteristics (see SSRN paper).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Momentum is sensitive to market regimes; state-dependence complicates out-of-sample robustness.
  - Transaction costs and crowding are important for momentum implementations.
  - ML partitioning can overfit if not constrained by economic structure.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Merge regime detection with momentum strategies to adapt to crash risk.
  - Use interpretable ML to separate information-driven vs. behavioral momentum.
  - Evaluate cross-country consistency of dissected momentum drivers.

  </div>
</details>



---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3747238" target="_blank">Goyenko, R., & Zhang, C. (2020). The Joint Cross Section of Option and Stock Returns Predictability with Big Data and Machine Learning. SSRN Electronic Journal.</a>
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Investigates predictability in the joint cross-section of option and stock returns using many predictors and ML models; finds option-based predictors often outperform stock-only predictors for forecasting option returns and can improve economic performance net of costs in some settings.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Option and stock returns, option-implied variables, and a large set of option & stock characteristics (multi-million observation panel).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - High-dimensional option datasets require careful cleaning and selection.
  - Transaction costs and liquidity in options can erode implementable profits.
  - Model complexity increases risk of overfitting on millions of observations.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Integrate implied-volatility-surface based features with ML for better hedging.
  - Test robustness across option maturities and underlyings.
  - Develop capacity-aware strategies considering liquidity and slippage.

  </div>
</details>



---

### <a href="https://link.springer.com/article/10.1007/s42521-020-00019-x" target="_blank">Dautel, A. J., H√§rdle, W. K., Lessmann, S., & Seow, H.-V. (2020). Forex exchange rate forecasting using deep recurrent neural networks. Digital Finance.</a>
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Compares LSTM/GRU models with traditional recurrent and feedforward networks for exchange-rate directional forecasting. Finds deep recurrent models provide improved directional accuracy but warns about tuning complexity and overfitting risks for trading profits.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - High-frequency and daily FX rates for major currency pairs; engineered macro and technical predictors.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - FX markets have structural shifts and regime changes that complicate model stability.
  - Overfitting and tuning complexity can offset apparent gains.
  - Practical profitability must account for execution costs and spreads.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Robust model selection for regime shifts.
  - Real-time evaluation with transaction-cost accounting.
  - Hybrid econometric-ML models for interpretability.

  </div>
</details>



---

### Cong, L., Tang, K., Wang, J., & Zhang, Y. (2020). Deep Sequence Modeling: Development and Applications in Asset Pricing. SSRN Electronic Journal.
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  U.S. equity time-series and cross-sectional data for empirical comparisons; sequence datasets constructed from returns and predictors.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - U.S. equity time-series and cross-sectional data for empirical comparisons; sequence datasets constructed from returns and predictors.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Sequence models need large amounts of data and careful regularization.
  - Hyperparameter tuning and architecture choice materially affect results.
  - Interpretability of sequence features is difficult.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Apply transformers and attention to longer horizon financial forecasting.
  - Combine sequence models with economic constraints for interpretability.
  - Benchmark against classical econometric models with utility-based metrics.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article-abstract/34/2/1046/5843806?redirectedFrom=fulltext" target="_blank">Bianchi, Daniele, Matthias Büchner, and Andrea Tamoni. "Bond risk premiums with machine learning." The Review of Financial Studies 34, no. 2 (2021): 1046-1089.</a>
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Uses ML tools (extreme trees, NNs) to model bond risk premia and documents improved prediction and economic gains relative to linear models. Highlights macro-financial predictors and nonlinear interactions important for bond premia.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Bond yields, macro variables, and bond-level characteristics (see paper for exact dataset).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Bond markets' low-frequency and illiquidity challenge model training and evaluation.
  - Interpreting macro-driven nonlinear patterns in economic terms is non-trivial.
  - Out-of-sample stability in stressed environments needs further testing.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Integrate term-structure theory constraints into ML algorithms for better interpretability.
  - Test ML models across different bond sectors (sovereign, municipal, corporate).
  - Assess performance during crisis episodes and regimes.

  </div>
</details>



---

### <a href="Working paper / SSRN / SFI links (see paper): https://ideas.repec.org/p/chf/rpseri/rp20110.html ; SSRN entry" target="_blank">Bali, Goyal, Huang, Jiang, & Wen. The Cross-Sectional Pricing of Corporate Bonds Using Big Data and Machine Learning. (2020).</a>
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Applies ML to predict cross-sectional corporate bond returns using a large set of equity and bond characteristics and finds ML methods improve out-of-sample predictive power; imposing economic structure (Merton) helps.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - TRACE transaction-level data for bonds (US), firm equity characteristics, bond fundamentals (see paper for details).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Fixed-coupon securities have special features (callability, illiquidity) requiring careful modeling.
  - Corporate bond datasets are noisier and sparser than equities -> potential overfitting.
  - Transaction costs and dealer intermediation dynamics complicate implementability.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Combine structural credit models (Merton-style) with ML for improved interpretability.
  - Incorporate dealer-level microstructure and liquidity supply measures.
  - Test international bond markets and municipal/corporate subsegments.

  </div>
</details>



---

### <a href="SSRN: https://ssrn.com/abstract=3136368" target="_blank">Bianchi & McAlinn. Divide and Conquer: Financial Ratios and Industry Returns Predictability. SSRN (2020).</a>
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Proposes an ensemble 'divide-and-conquer' approach that groups predictors into small-scale linear models and ensembles them to capture rich information while controlling overfitting. Shows improved predictability of industry returns versus monolithic high-dimensional models.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Industry-level returns, firm financial ratios, and sector classifications; see SSRN paper for details.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Choice of grouping/ensembling may be ad-hoc and require domain knowledge.
  - Performance depends on stability of ratio-industry relationships through time.
  - Relies on high-quality, industry-level financial data which may be noisy.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Automate grouping with hierarchical clustering or Bayesian grouping priors.
  - Combine with causal feature selection to improve robustness.
  - Test in international samples and cross-asset contexts.

  </div>
</details>



---

### <a href="https://doi.org/10.1093/rfs/hhaa009 ; SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3159577" target="_blank">Gu, Shihao, Bryan Kelly, and Dacheng Xiu. Empirical asset pricing via machine learning. Review of Financial Studies (2020).</a>
**Year:** 2020  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  A systematic comparison of machine learning methods for asset pricing problems (predicting risk premia and the cross-section). Finds tree-based and neural-network methods often outperform linear benchmarks; shows nonlinear interactions and model selection matter for economic gains.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - 94 characteristics (61 of which are updated annually, 13 updated quarterly, and 20
  - updated monthly).
  - 8 Macroeconomic predictors that are aggregated time
  - series variables.
  - Average number of stocks per month exceeding 6200
  - Treasury bill rate to proxy the risk-free rate from
  - which the individual excess returns are calculated.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Economic interpretation of ML signals is limited‚Äîhard to link to risk-based primitives.
  - ML strategies may rely heavily on small or illiquid stocks (limits-to-arbitrage concerns).
  - High turnover and transaction costs often not fully accounted for in economic evaluation.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Combine ML with economic restrictions/prior structure to improve interpretability and robustness.
  - Study long-run stability and publication-date effects (post-publication alpha decay).
  - Integrate alternative data sources (text, high-frequency) in a unified ML framework.

  </div>
</details>



---

### <a href="https://pubsonline.informs.org/doi/10.1287/mnsc.2020.3696" target="_blank">Wu, W., Chen, J., Yang, Z. (Ben), & Tindall, M. L. (2021). A Cross-Sectional Machine Learning Approach for Hedge Fund Return Prediction and Selection. Management Science, 67, 4577-4601.</a>
**Year:** 2021  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Applies ML to predict cross-sectional hedge-fund returns. ML-based selection improves out-of-sample performance and highlights idiosyncratic predictive features.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Hedge fund data biases (survivorship, backfill).
  - Managerial behavior affects persistence.
  - Net performance may lag due to fees and costs.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Employ anti-backfill evaluation.
  - Incorporate textual data.
  - Test across strategy buckets globally.

  </div>
</details>



---

### <a href="https://arxiv.org/abs/2102.09209" target="_blank">Chen, H., Didisheim, A., & Scheidegger, S. (2021). Deep Structural Estimation: With an Application to Option Pricing. SSRN.</a>
**Year:** 2021  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Proposes deep structural estimation methods combining structural economic models with deep learning, and applies the framework to option pricing estimation.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Option market data and underlying asset prices;

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Combining structural restrictions and flexible neural nets raises identification issues.
  - Calibration and computational cost can be high.
  - Sensitivity to specification of structural components.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Broader applications to macro-finance structural estimation.
  - Benchmarks comparing deep structural to traditional estimation approaches.

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/abs/pii/S0304405X24001338" target="_blank">Cao, S. S., Jiang, W., Wang, J. L., & Yang, B. (2021). From Man vs. Machine to Man + Machine: The Art and AI of Stock Analyses. SSRN.</a>
**Year:** 2021  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Builds an AI analyst for stock analysis and shows a 'man+machine' hybrid often outperforms either humans or machines alone, reducing extreme errors and improving robustness.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Corporate disclosures, analyst reports, market data; see paper appendix.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Generalizability across firm types and rare-event settings.
  - Human-in-the-loop implementation costs and latency.
  - Potential overfitting to historical analyst behavior.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Field experiments integrating AI assistants with real analysts.
  - Study of human-AI interaction designs for investment decisions.

  </div>
</details>



---

### <a href="https://onlinelibrary.wiley.com/doi/epdf/10.1111/jofi.13090" target="_blank">Fuster, A., Goldsmith‚ÄêPinkham, P., Ramadorai, T., & Walther, A. (2021). Predictably Unequal? The Effects of Machine Learning on Credit Markets. The Journal of Finance, 77, 5-47.</a>
**Year:** 2021  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  This paper develops theory and empirical evidence showing that ML adoption by lenders can produce unequal outcomes across borrower groups even if protected attributes are excluded — improvements in prediction can benefit some groups more than others and change access and pricing in credit markets. The authors highlight channels through which ML can exacerbate or mitigate disparities and provide a framework for assessing distributional consequences of better prediction.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Lending datasets (consumer credit records, loan-level microdata) and simulated / theoretical analyses to show distributional impacts under different informational structures

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Theoretical results depend on model assumptions about lenders’ objectives and market structure.
  - Empirical tests require high-quality granular credit data, often proprietary.
  - Policy implications are sensitive to assumptions about regulator constraints and lender behavior.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Field experiments to measure distributional impacts when ML is deployed in real underwriting.
  - Design of fairness-aware objective functions that align lender incentives with distributional goals.
  - Cross-country studies to see how regulatory environments moderate ML’s effects.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article/36/6/2361/6782974" target="_blank">van Binsbergen, J. H., Han, X., & Lopez-Lira, A. (2020). Man vs. Machine Learning: The Term Structure of Earnings Expectations and Conditional Biases. SSRN Electronic Journal.</a>
**Year:** 2022  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Constructs ML-based benchmarks for firm earnings expectations and compares with analysts’ forecasts. Finds conditional biases linked to return predictability.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - ML benchmarks depend on feature choice.
  - Analyst incentives not modeled.
  - Cross-country validity uncertain.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Field experiments to reduce analyst biases.
  - Extend to other forecast types.
  - Explore regulatory implications.

  </div>
</details>



---

### <a href="https://doi.org/10.1016/j.jfineco.2021.08.017 ; SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3754339" target="_blank">Leippold, Markus, Qian Wang, and Wenyu Zhou. Machine learning in the Chinese stock market. Journal of Financial Economics (2022).</a>
**Year:** 2022  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Applies ML methods to the Chinese stock market to build return-prediction models and factors. Finds liquidity-related predictors and retail-investor effects important; emphasizes transaction-cost considerations.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Daily and monthly total stock returns for all A share stocks listed in Shanghai and Shenzhen stock exchanges from the Wind Database (3900 stocks over a time period of 20 years). yield rate for the one year govt bond in China from CMAR to proxy fopr the risk free rate which is necessary for cvalculating individual excess returns. 94 stock level characteristics (4 are valid chinese specific factors), binary vbariables (4) that indicate ownership types. cross sectional ranking and maping them between -1 and 1 to avoid the effect of outliers along with 80 industry dummies. 11 macroeconomic predictors.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Unique market microstructure (retail dominance) reduces direct transferability of U.S. ML results.
  - Transaction costs and short-sale constraints can materially reduce implementable profits.
  - Data access and quality in emerging/segmented markets can hamper replication.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Adjust ML pipelines for market microstructure and retail behavior when porting methods across countries.
  - Investigate robustness to trading frictions and alternative liquidity measures.
  - Use high-frequency trade-level data to better capture retail vs institutional dynamics.

  </div>
</details>



---

### <a href="SSRN / Management Science: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3450322 ; DOI via Management Science" target="_blank">Avramov, Cheng, & Metzker. Machine Learning versus Economic Restrictions: Evidence from Stock Return Predictability. Management Science (2023).</a>
**Year:** 2023  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Reassesses ML-based predictability claims and shows that imposing economically motivated restrictions (exclude microcaps, distressed stocks, apply trading-cost filters) substantially reduces reported ML profitability. Highlights the importance of realistic economic constraints when evaluating ML strategies. Compares unconstrained ML methods against models with economic restrictions. Finds ML picks up profit mainly from difficult-to-arbitrage stocks and that realistic frictions attenuate economic gains.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - U.S. stock returns and characteristics; check paper for full data appendix.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Demonstrates sensitivity to sample selection—raises questions about prior ML economic gains.
  - Quantifying realistic trading costs and market impact remains challenging.
  - Findings depend on choices around universes (microcaps, penny stocks) and data snooping risks.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Systematically integrate limits-to-arbitrage and market impact into ML evaluation pipelines.
  - Develop standardized robustness checks (economic restrictions) for ML-based asset-pricing studies.
  - Reexamine published ML results under matched economic constraint protocols.

  </div>
</details>



---

### <a href="https://doi.org/10.1287/mnsc.2023.4695 ; arXiv: https://arxiv.org/abs/1904.00745" target="_blank">Chen, Luyang, Markus Pelger, and Jason Zhu. Deep learning in asset pricing. Management Science (2023).</a>
**Year:** 2023  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Estimates a stochastic discount factor (SDF) with deep neural networks using a no-arbitrage loss and an adversarial construction of test assets. Proposes a deep neural-network-based approach to estimate asset-pricing models that enforces no-arbitrage and uses adversarially chosen test assets. The method extracts latent economic states from macro variables and delivers improved out-of-sample pricing and Sharpe ratios compared to benchmarks.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Firm-level returns (CRSP), Compustat, macroeconomic time series; constructs test assets via adversarial selection.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Complex training objectives (no-arbitrage plus adversarial tasks) can be sensitive to hyperparameters.
  - Interpretability of deep networks remains limited; mapping to economic states is empirical rather than structural.
  - Computational intensity and reproducibility concerns for large-scale implementations.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Develop diagnostics that connect learned states to macroeconomic fundamentals.
  - Simplify/adapt the adversarial testing procedure for robust application across markets.
  - Extend framework to multi-period choices and general equilibrium settings.

  </div>
</details>



---

### <a href="https://www.tandfonline.com/doi/full/10.1080/0015198X.2024.2313692" target="_blank">Cao, K., & You, H. (2020). Fundamental Analysis Via Machine Learning. SSRN / journal.</a>
**Year:** 2024  **Category:** Forecasting


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Investigates ML methods for forecasting corporate earnings and fundamental signals; finds ML improves forecast accuracy versus linear baselines when properly tuned.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Firm financials, historical earnings, possibly textual disclosures; details in paper.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Data snooping in feature choice for fundamentals forecasting.
  - Model sensitivity to missing financial history and outliers.
  - Need for real-time applicability and vintage data.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Evaluate performance in real-time vintages and international settings.
  - Combine tabular ML with textual disclosures for improved forecasts.

  </div>
</details>




## Latent Factor Model


---

### <a href="Journal: https://academic.oup.com/ectj/article/21/1/C1/5052706 ; arXiv/SSRN available." target="_blank">Chernozhukov, V., Chetverikov, D., Demirer, M., Duflo, E., Hansen, C., Newey, W., & Robins, J. (2018). Double/debiased machine learning for treatment and structural parameters. Econometrics Journal.</a>
**Year:** 2018  **Category:** Latent Factor Model


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Introduces the Double/Debiased Machine Learning framework to obtain valid inference on low-dimensional parameters in the presence of high-dimensional nuisance functions estimated by ML methods.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Methodological paper (applies to many datasets; theoretical and empirical examples included).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Requires regularity conditions and sample-splitting; finite-sample performance can vary.
  - Implementation choices (cross-fitting folds, ML learners) affect results.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Better finite-sample corrections and guidance for practitioner choices.
  - Extend frameworks to time-series dependence common in finance.

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/abs/pii/S0304407622000914" target="_blank">Xiong, R., & Pelger, M. (2019). Large Dimensional Latent Factor Modeling with Missing Observations and Applications to Causal Inference. SSRN Electronic Journal.</a>
**Year:** 2019  **Category:** Latent Factor Model


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Proposes PCA-based estimators and theory for latent factor models with missing observations. Provides asymptotic results and demonstrates use for imputation and causal inference.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Large panel datasets with missing entries (macro panels, firm panels).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Assumes specific missingness mechanisms.
  - Performance degrades with structured missingness.
  - Covariance adjustment choices affect outcomes.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Extend to dynamic/mixed-frequency models.
  - Develop MNAR-robust methods.
  - Release open-source implementation.

  </div>
</details>



---

### <a href="https://www.cambridge.org/core/journals/journal-of-financial-and-quantitative-analysis/article/abs/uncovering-sparsity-and-heterogeneity-in-firmlevel-return-predictability-using-machine-learning/1B70137EF297066928918332AE663B24" target="_blank">Evgeniou, T., Guecioueur, A., & Prieto, R. (2020). Modeling Heterogeneity in Firm-level Return Predictability with Machine Learning. Journal of Financial and Quantitative Analysis.</a>
**Year:** 2020  **Category:** Latent Factor Model


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  The authors propose ML frameworks that allow for sparsity and latent group heterogeneity in firm-level return predictability: firms can be assigned to latent groups with group-specific predictive relationships. Their approach improves firm-level expected return estimation by capturing heterogeneity in predictive relations across firm types.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Monthly firm returns (CRSP), firm characteristics (Compustat/other), macro predictors; firm grouping inferred from characteristics.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Identifying latent groups relies on chosen features and model tuning; group instability may occur over time.
  - Sparse models can miss weak but economically important signals.
  - Practical portfolio implementation requires accounting for trading frictions and turnover.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Dynamic group assignment (allowing firms to switch groups through time) and regime-conditional models.
  - Integrate textual or alternative data to improve group identification.
  - Evaluate economic value net of realistic transaction costs.

  </div>
</details>



---

### <a href="https://www.sciencedirect.com/science/article/abs/pii/S0304407620301998 ; SSRN: https://ssrn.com/abstract=3335536" target="_blank">Gu, Shihao, Bryan Kelly, and Dacheng Xiu. Autoencoder asset pricing models. Journal of Econometrics</a>
**Year:** 2021  **Category:** Latent Factor Model


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Introduces a conditional autoencoder that learns low-dimensional latent factors and nonlinear factor loadings from firm characteristics. The model improves out-of-sample pricing and produces smaller pricing errors than many linear methods (e.g., IPCA) while allowing flexible nonlinear exposures.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - March 1957 (the start date of the S&P 500) and ends in December 2016, totaling 60 years.
  - 94 characteristics (61 of which are updated annually, 13 updated quarterly, and 20
  - updated monthly).
  - rank-normalize all characteristics into the interval (−1, 1)
  - any filters based on stock prices or share codes, or rule out financial
  - firms. Past literature has imposed these filters in large part because they find it difficult to reconcile the return behavior
  - of low-price stocks, uncommon share codes, and financial sector stocks with the rest of the sample
  - Median imputation throughout the dataset so they have the full range of 30000 company data.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Model interpretability: learned latent factors are nonlinear and harder to economically interpret.
  - Overfitting risk if not carefully regularized or validated (autoencoders can memorize noise).
  - Requires large cross-sectional and time-series data; performance may degrade for smaller markets.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Develop methods to map learned latent factors to economic primitives (interpretability tools).
  - Extend to multi-asset settings (bonds, options) and mixed-frequency data.
  - Robustness checks under transaction costs and limits-to-arbitrage constraints.

  </div>
</details>



---

### <a href="https://www.cambridge.org/core/journals/journal-of-financial-and-quantitative-analysis/article/abs/deep-learning-in-characteristicssorted-factor-models/DD410814792E49E271957E8C87C1D763" target="_blank">Feng, G., Polson, N., & Xu, J. (2021). Deep Learning in Characteristics-Sorted Factor Models. Journal of Financial and Quantitative Analysis</a>
**Year:** 2021  **Category:** Latent Factor Model


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  The paper introduces a structural deep-learning framework that replaces ad-hoc characteristics sorting with deep nets that generate latent risk factors from high-dimensional characteristics. The model aims to reconcile the intuition behind characteristic-sorted factor construction and leverage representational power of DL while optimizing an economic objective (pricing error minimization

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Deep networks are less interpretable than classical factor constructions (economic labeling of latent factors is hard).
  - Tuning, regularization, and sample splitting choices affect factor stability.
  - Risk of overfitting to backtest anomalies without careful validation.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Methods to map latent deep factors to economic primitives (interpretability / XAI).
  - Cross-sample stability tests and international replication.
  - Hybrid models that incorporate economic constraints (e.g., no-arbitrage penalties).

  </div>
</details>




## Microstructure


---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3710491" target="_blank">Kwan, A., Philip, R., & Shkilko, A. (2020). The Conduits of Price Discovery: A Machine Learning Approach. SSRN Electronic Journal.</a>
**Year:** 2020  **Category:** Microstructure


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Kwan, Philip, and Shkilko apply ML tools to identify which trading venues and participant types act as key conduits for price discovery, using high-frequency data on order flow and trade initiation. They build predictive models that use granular trade and quote variables to forecast short-term price movements and then apply explainability tools (feature attribution) to infer which venues/participants’ actions are most informative. The authors document that certain high-liquidity venues and specific participant classes (e.g., informed proprietary traders) systematically lead price formation, while other venues act primarily as liquidity sinks. Their approach combines supervised learning with counterfactual analyses to test the causal role of particular event types. They conduct robustness across asset classes and market regimes, showing that the set of conduits can change with volatility and regulation. The paper contributes to market-microstructure theory by providing empirical evidence of heterogeneity in venue informativeness and by offering a data-driven toolkit to monitor price-discovery channels. It also highlights implications for regulators and market-designers interested in venue consolidation or fragmentation policies. Limitations include the proprietary nature of participant identifiers and the complexity of mapping model importances to structural causality.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Tick-level trade and quote histories with venue identifiers and (where available) participant identifiers or inferred trader types.
  - Event-level features: trade direction, aggressor type, size, order-book depth.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Participant identifiers are often not publicly available or consistent, constraining replication.
  - Inferring causal direction from predictive importance requires further structural modeling.
  - Results can be sensitive to venue-specific microstructure (tick sizes, matching rules).

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Use natural-experiment events (e.g., venue outages) to strengthen causal claims.
  - Extend to cross-border price-discovery studies with consolidated tick data.

  </div>
</details>



---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3694019" target="_blank">Chaudhry, A., & Oh, S. (2020). High-Frequency Expectations from Asset Prices: A Machine Learning Approach. SSRN.</a>
**Year:** 2020  **Category:** Microstructure


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Uses ML to extract high-frequency expectations embedded in asset prices, leveraging intraday data and novel feature engineering.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - High-frequency intraday price and order-book data (see paper).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Microstructure noise and data-cleaning are crucial and challenging.
  - Overfitting to intraday patterns that are ephemeral.
  - Scalability and latency in real-time systems.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Robustness to microstructure frictions and different sampling frequencies.
  - Integration with execution-aware strategies.

  </div>
</details>



---

### <a href="https://onlinelibrary.wiley.com/doi/10.1111/mafi.12413" target="_blank">Kolm, P. N., Turiel, J., & Westray, N. (2021). Deep Order Flow Imbalance: Extracting Alpha at Multiple Horizons from the Limit Order Book.Mathematical Finance,</a>
**Year:** 2021  **Category:** Microstructure


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Kolm, Turiel, and Westray propose a deep-learning approach to extract order-flow imbalance signals from raw limit order book (LOB) data across multiple horizons to predict short- and medium-term returns. Their architecture combines convolutional layers (to capture spatial LOB patterns) with recurrent or attention mechanisms to model temporal dependencies, producing order-flow imbalance indices that vary by horizon. They demonstrate that horizon-specific imbalance measures predict returns at their respective time scales even after controlling for standard microstructure covariates. The authors carefully address the practicalities of LOB work: normalization across assets, handling missing snapshots, and aligning order-flow events. Out-of-sample tests and transaction-cost adjusted backtests show economically meaningful alpha at short horizons for certain assets, though returns decline as costs and realistic execution constraints are tightened. The paper also examines robustness across stocks, liquidity regimes, and sample periods, showing that the learned imbalance features can generalize with appropriate regularization. It contributes to the literature by providing a horizon-aware, data-driven decomposition of order flow that is more adaptive than fixed-rule imbalance statistics. The authors discuss implementation considerations for real-time systems and highlight limitations related to latency and exchange microstructure differences

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - High-frequency LOB snapshots and trade prints (exchange-level tick data), sometimes public LOB benchmark datasets for replication.
  - Preprocessing: normalization, mid-price labels, and sub-sampling at fixed intervals to produce training examples.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Latency, execution, and market impact can substantially reduce naive backtest alphas.
  - Cross-exchange differences and asset-specific microstructure features limit portability.
  - Training deep models on tick-data is computationally intensive and demands careful overfitting controls.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Multi-asset multi-market studies to test transferability and cross-market contagion of order-flow signals.
  - Incorporate execution-aware losses (market impact models) into the training objective.
  - Explore interpretability of learned imbalance filters to link to economic liquidity measures.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article-abstract/34/7/3316/5868424" target="_blank">Easley, D., López de Prado, M., O’Hara, M., & Zhang, Z. (2020). Microstructure in the Machine Age. Review of Financial Studies.</a>
**Year:** 2021  **Category:** Microstructure


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  The paper surveys and demonstrates how modern market-microstructure research benefits from large, high-frequency datasets and advanced ML methods; it documents both promise and pitfalls of applying ML in microstructure (e.g., prediction vs. interpretability). The authors show that some classical microstructure measures remain informative while others lose predictive power in complex, high-dimensional environments; they emphasize careful validation and causality concerns in ML applications.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - High-frequency trade & quote data (limit order book snapshots, trades), transaction-level datasets used in microstructure studies (venue- and exchange-level data).

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Microstructure datasets are heterogeneous across venues (matching rules, tick sizes), limiting portability.
  - High-frequency noise and asynchronous timestamps complicate ML model training and evaluation.
  - Predictive features with high in-sample explanatory power may have low out-of-sample predictability (overfitting risk).
  - Real-world deployment faces latency, execution, and market-impact constraints that academic backtests often ignore.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Develop standardized, exchange-aware benchmarks and evaluation protocols (including latency and market impact).
  - Causal ML for microstructure (to disentangle prediction from structural mechanisms).
  - Real-time, adaptive models that explicitly optimize execution-aware objectives.

  </div>
</details>




## NLP


---

### <a href="https://academic.oup.com/qje/article-abstract/134/4/2135/5531768" target="_blank">Hassan, T. A., Hollander, S., van Lent, L., & Tahoun, A. (2019). Firm-Level Political Risk: Measurement and Effects. The Quarterly Journal of Economics, 134, 2135-2202.</a>
**Year:** 2019  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Hassan et al. introduce a novel firm-level measure of political risk constructed from the fraction of words in firms’ quarterly earnings conference calls that pertain to political topics (e.g., trade policy, regulation, sanctions). Their approach combines straightforward computational-linguistics classification of political-words with rigorous validation: they show the measure covaries with observable exposures (e.g., revenue share from government contracts) and with aggregate political shocks. Using the constructed panel (quarterly firm-level political-risk scores for thousands of U.S. public firms), they document that elevated firm-level political risk forecasts lower future sales growth, higher stock return volatility, and increased cost of equity, conditional on controls. The analysis also demonstrates cross-sectional heterogeneity: firms more exposed to government procurement and regulated sectors show stronger political-risk effects. The authors employ difference-in-differences and instrumental-variable exercises to provide causal evidence that political events (e.g., legislative changes, trade-policy episodes) drive economic outcomes through firm-level political-risk channels. Robustness checks include alternative political dictionaries, hand-labeled validation samples, and placebo tests. Their dataset, replication files, and code are publicly available through the project page, enabling researchers to extend the measure. The paper thus bridges text-as-data methods with macro- and micro-economic inference to quantify a previously hard-to-measure dimension of firm risk

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Earnings conference-call transcripts (quarterly) for U.S. publicly listed firms (ICE/Thomson/Refinitiv transcript sources).
  - Firm financials and returns (Compustat, CRSP) for outcomes like sales, volatility, and returns.
  - Additional hand-labeled dictionary validation data and event indicators for political episodes (e.g., trade disputes, government shutdowns).
  - The replication/data webpage provides the firm-quarter political-risk panel used in the analyses.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - The political-risk proxy depends on keyword dictionaries and NLP preprocessing choices; misclassification (false positives/negatives) is possible.
  - Conference-call coverage skews toward larger firms and US-centric samples, limiting generalizability to smaller or non-U.S. firms.
  - Identifying causal channels (political risk → firm outcomes) remains challenging despite IV/DiD; unobserved confounders can persist.
  - The measure captures discussion of political topics, which may reflect management signaling rather than exogenous exposure.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Apply the methodology to multi-lingual or international conference calls to study country heterogeneity in political-risk transmission.
  - Use natural experiments (e.g., sudden policy shocks) and firm-level cross-border variation to strengthen causal identification.
  - Combine text-based political-risk measures with other alternative-data sources (lobbying disclosures, PAC donations) to triangulate exposure.

  </div>
</details>



---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3740954" target="_blank">Lee, G. M., Naughton, J. P., Zheng, X., & Zhou, D. (2020). Predicting Litigation Risk via Machine Learning. SSRN Electronic Journal.</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Lee et al. develop ML classifiers to predict firm-level litigation risk using a combination of firm financials, textual disclosures, and governance variables. Their pipeline integrates textual features (MD&A and 10-K language), accounting anomalies, and past litigation histories to predict future lawsuits or regulatory investigations. They train ensemble models and emphasize careful handling of extreme class imbalance (litigation is relatively rare) via sampling techniques and cost-sensitive losses. The models achieve improved discrimination over standard logistic baselines and identify salient predictors (e.g., language indicating managerial obfuscation, sudden revenue recognition changes). The authors validate model predictions by correlating predicted litigation risk with future abnormal returns and realized legal outcomes, and they show that high predicted risk firms experience distinct pricing and trading patterns. Robustness exercises include alternative text embeddings and exclusion of obviously predictive post-event variables to avoid look-ahead bias. The paper contributes to litigation risk modeling for investors and auditors, showing ML can provide early warning signals when applied carefully. They also discuss deployment challenges for auditors and compliance teams.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - 10-K / MD&A textual disclosures from EDGAR, parsed into linguistic features or embeddings.
  - Firm accounting and market variables from Compustat and CRSP.
  - Litigation labels from legal databases (court filings, enforcement actions) used as positive events.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Label noise: not all litigation events are captured equally, and some firms settle quietly, causing underreporting.
  - Severe class imbalance requires careful validation and leads to potential false positives.
  - Causal interpretation (text → litigation) is challenging; text may proxy for other risks.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Semi-supervised and anomaly-detection methods to detect early signals with limited labeled litigation cases.
  - Integration with auditor workflow and cost-sensitive learning to manage false-positive costs.

  </div>
</details>



---

### <a href="https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3389884" target="_blank">Ke, Zheng Tracy, et al. Predicting Returns with Text Data. (2020) Available at SSRN: https://ssrn.com/abstract=3389884.</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Ke et al. investigate whether and how unstructured text data (news, filings, transcripts) can enhance return prediction over traditional numeric predictors. They assemble large text corpora and apply modern text representation approaches (document embeddings, topic models, and supervised text features) combined with ML learners (trees, neural nets) to forecast both short- and medium-horizon returns. The authors emphasize careful evaluation: vintage text/time splits, realistic information sets, and transaction-cost adjusted utility metrics to assess economic significance. Results indicate that certain text-derived features (event counts, tone shifts, and latent topics tied to fundamentals) can add incremental predictive power, particularly for short-horizon and event-driven returns. They further analyze interpretability via attention or feature-importance diagnostics to link text features to economic stories (earnings surprises, policy events). Robustness tests cover multiple corpora and alternative model classes, and the paper often reports both statistical and economic magnitudes of gains. Methodological contributions include a pipeline for integrating text embeddings with tabular firm characteristics in a unified forecasting model. Overall, the work helps set standards for validly testing text-based predictive claims in finance.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Diverse textual corpora: press releases, news wires, 8-K/10-K/10-Q filings, and earnings-call transcripts.
  - Matched return series at daily, weekly, and monthly horizons (CRSP) and firm fundamentals from Compustat.
  - Preprocessing and embedding choices carefully documented for vintage-feasible backtesting.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Textual embeddings and features are sensitive to model architecture and training corpus; portability is not guaranteed.
  - Event-driven signals may be ephemeral — gains may not persist out-of-sample without retraining.
  - High-dimensional text features increase the risk of multiple-testing and spurious results.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Systematic comparison of embedding approaches (word2vec, transformers) for financial prediction tasks.
  - Hybrid architectures that jointly model text and numeric time series with attention to vintage data issues.
  - Development of public benchmark datasets for text+returns tasks.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article-abstract/33/3/1184/5735305" target="_blank">Engle, R. F., Giglio, S., Kelly, B., Lee, H., & Stroebel, J. (2020). Hedging Climate Change News. The Review Of Financial Studies, 33, 1184-1216.</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  he paper constructs climate-change news series using textual analysis and extracts news innovations; it then designs dynamic hedging portfolios (mimicking portfolios) that target exposure to climate-news shocks using cross-sectional asset exposures and third-party ESG scores. The authors document that climate-news innovations are economically meaningful and that hedges built from them have pricing and insurance implications when disciplined by ESG measures.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Large newspaper/text corpora for climate-change mentions (news text), constructed climate-news time series, firm-level returns, ESG/climate exposure scores from third-party providers

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Text-derived climate measures depend on preprocessing and keyword/lexicon choices (sensitivity).
  - Hedging strategies rely on cross-sectional exposures estimated from historical data which may change in regimes.
  - ESG/climate scores are imperfect proxies and vary across providers, affecting hedge construction and interpretation.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Robustness checks across multiple news sources and alternative climate lexicons or transformer-based text models.
  - Study the interplay between climate-news hedging and regulatory/policy shocks (e.g., carbon taxes).
  - Evaluation of hedges under stress scenarios and long-horizon climate risks.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article-abstract/34/7/3265/5869446" target="_blank">Li, K., Mai, F., Shen, R., & Yan, X. (2020). Measuring Corporate Culture Using Machine Learning. The Review of Financial Studies.</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Li et al. build quantitative measures of corporate culture using ML-driven analysis of firm disclosures, internal documents, and other textual sources, arguing that culture manifests in repeated patterns of language and sentiment that are predictive of long-term firm outcomes. Their methodology extracts culture dimensions using unsupervised and supervised text techniques, including embeddings, topic models, and dictionary-based measures, which are then validated against managerial-behavior proxies (turnover, investment choices) and firm performance. They find certain culture dimensions (e.g., innovation orientation, conservatism) have robust relations with investment policies and cross-sectional returns, after controlling for standard characteristics. The authors emphasize the careful construction of culture measures to avoid conflating culture with short-run sentiment or managerial PR language, performing placebo tests and hand annotations to validate constructs. Instrumental-variable strategies or natural experiments (e.g., leadership changes) are used to argue for causal pathways from culture to outcomes. They also document that culture measures can help predict the firm's response to shocks and explain heterogeneity in outcomes across similar firms. The paper contributes to the measurement literature by turning a previously fuzzy concept—corporate culture—into reproducible, multi-dimensional metrics that can be used in asset pricing and governance studies.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Firm disclosures (10-K, MD&A), earnings call transcripts, and possibly internal employee-review aggregates if available.
  - Firm accounting, governance, and performance variables from Compustat/CRSP.
  - Hand-labeled validation samples to calibrate culture dimensions.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Culture is latent and persistent; textual proxies may capture surface-level rhetoric rather than deep behavioral norms.
  - Cross-firm comparability is difficult due to industry-specific language use.
  - Causal evidence is hard; leadership changes may be endogenous.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Linking culture measures to micro-level outcomes (employee turnover, product development timelines) with firm-internal data.
  - Cross-country studies to understand cultural variation and disclosure norms.
  - Use network or social-media data to enrich culture metrics.

  </div>
</details>



---

### <a href="https://link.springer.com/article/10.1007/s11142-020-09563-8" target="_blank">Bertomeu, Cheynel, Floyd, & Pan. Using machine learning to detect misstatements. Review of Accounting Studies (2020).</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Applies various ML methods to detect financial misstatements and misreporting, comparing performance to traditional models and highlighting useful features.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Financial statement data and enforcement/SEC restatement records; see paper for details.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - False positives have real costs; need to balance precision vs recall in operational settings.
  - Heterogeneity across firms/industries may reduce generalization of trained models.
  - Regulatory and privacy constraints limit access to rich features in practice.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Better calibration and cost-sensitive learning tailored to audit priorities.
  - Cross-firm transfer learning to improve small-sample performance.
  - Integrate explainable AI for audit trail documentation.

  </div>
</details>



---

### <a href="https://onlinelibrary.wiley.com/doi/full/10.1111/1475-679X.12292" target="_blank">Bao, Ke, Li, Yu, & Zhang. Detecting Accounting Fraud in Publicly Traded U.S. Firms Using a Machine Learning Approach. Journal of Accounting Research (2020).</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Uses ML classifiers to detect accounting fraud in US firms, leveraging financial statement features and textual signals; reports improved detection relative to standard benchmarks.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Compustat/CRSP financials, audit reports, possibly text of filings; see paper for dataset and labeling procedure.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Label quality: fraud/misstatement labels are noisy and subject to detection biases.
  - Class imbalance (fraud events are rare) complicates training and evaluation.
  - Potential adverse incentives if algorithms are used operationally without human oversight.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Develop causal/interpretability tools to explain flagged cases to auditors.
  - Use multi-source signals (text, network, alternative data) to improve robustness.
  - Evaluate real-world deployment impacts on audit selection and false-positive costs.

  </div>
</details>



---

### <a href="Wiley / SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2803733" target="_blank">Brown, N. C., Crowley, R. M., & Elliot, W. B. (2019). What are You Saying? Using topic to Detect Financial Misreporting. Journal of Accounting Research.</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Introduces topic-based textual features to detect financial misreporting and shows topic models significantly improve out-of-sample detection performance. Demonstrates text topics add information beyond traditional style and financial features.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - 10-K filings text, SEC enforcement actions (AAERs), restatements, and financial statement data.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Topic models capture co-occurrence patterns but may miss nuanced or cleverly disguised language.
  - Label and event-timing uncertainty for misreporting cases complicate evaluation.
  - Language drift over time may require periodic model retraining.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Combine topic models with supervised deep-learning classifiers for richer feature sets.
  - Develop time-adaptive topic models to handle language evolution.
  - Evaluate cross-lingual transferability for international filings.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article-abstract/36/9/3603/7087110" target="_blank">Cao, S. S., Jiang, W., Yang, B., & Zhang, A. (2020). How to Talk When a Machine is Listening: Corporate Disclosure in the Age of AI. SSRN.</a>
**Year:** 2020  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Studies how corporate disclosure strategies change when firms anticipate machine-based text processing; analyzes disclosure wording and informativeness.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Corporate filings and disclosure texts, market reactions.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Measuring firms' anticipatory behavior is difficult and may be confounded by other disclosure incentives.
  - NLP model evolution over time affects measured behavior.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Longitudinal analyses as NLP models change.
  - Experimental approaches to detect strategic disclosure.

  </div>
</details>



---

### <a href="https://doi.org/10.2308/TAR-2017-0572" target="_blank">Song, S. (2021). The Informational Value of Segment Data Disaggregated by Underlying Industry: Evidence from the Textual Features of Business Descriptions. The Accounting Review.</a>
**Year:** 2021  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Song (2021) studies how the textual content of firms’ business segment descriptions reveals value-relevant information for investors. Using natural language processing (NLP) and machine learning, the paper extracts linguistic features—such as complexity, tone, and similarity—from segment-level disclosures. The findings suggest that disaggregated textual information enhances predictive power for future earnings and stock returns. The analysis demonstrates that segment disclosures help investors understand firm diversification, risk exposure, and operational focus. Song constructs firm-level measures of disclosure informativeness and links them to subsequent market reactions. Machine learning classifiers identify which textual dimensions (e.g., concreteness or uncertainty) correlate with valuation changes. The paper contributes to the literature on textual analysis and information economics by showing that nuanced segment disclosures play a crucial valuation role. The results have implications for reporting standards and investor behavior.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - U.S. SEC filings (10-K reports) from 1994–2018 obtained from EDGAR, combined with CRSP stock returns and Compustat accounting data. Text processing employs Bag-of-Words, TF-IDF, and readability measures.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - NLP models may misclassify domain-specific terms.
  - Focuses solely on U.S. public firms.
  - Possible endogeneity between disclosure quality and firm performance.
  - Limited interpretability of ML textual features.
  - Does not test cross-market or multilingual disclosures.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Apply multilingual NLP to global segment disclosures.
  - Examine the role of AI-generated disclosures in financial reporting.
  - Combine textual features with structured ESG data for integrated valuation.

  </div>
</details>



---

### <a href="https://doi.org/10.1093/rapstu/raab005 ; SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3258821" target="_blank">Azimi, M., & Agrawal, A. Is Positive Sentiment in Corporate Annual Reports Informative? Evidence from Deep Learning. Review of Asset Pricing Studies (2021).</a>
**Year:** 2021  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Applies deep-learning-based sentiment extraction to 10-K filings and finds both positive and negative sentiments predict abnormal returns and future firm fundamentals around filing dates. Shows finer-grained sentiment measures (vs. simple net-sentiment) contain incremental information.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - EDGAR 10-K filings for U.S. firms, stock returns around filing dates, and firm fundamentals.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Text-sentiment models require careful training and can be sensitive to label noise.
  - Filing-based signals can be confounded by concurrent announcements or news.
  - Generalizing across jurisdictions/time requires retraining sentiment models.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - `- Event-level causal identification strategies (e.g., instrumental variables).
  - Cross-sectional tests across industries and international filings.
  - Release trained models and preprocessing code for reproducibility.  Incorporate multi-modal data (text + earnings calls + management forecasts) for richer signals.
  - Test long-horizon predictive power and economic exploitability after costs.
  - Explore causal mechanisms linking narrative tone to firm fundamentals.

  </div>
</details>



---

### <a href="https://onlinelibrary.wiley.com/doi/full/10.1111/jofi.13377" target="_blank">Bybee, L., Kelly, B., Su, Y. (2022). Narrative Asset Pricing: Interpretable Systematic Risk Factors from News Text. SSRN.</a>
**Year:** 2023  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Extracts narrative factors from WSJ news text using LDA + IPCA + group lasso and shows these news-derived factors have strong pricing performance and high out-of-sample Sharpe ratios. Shows that news attention topics track macroeconomic activity and help forecast aggregate stock market returns.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Wall Street Journal text, returns on anomaly portfolios, macro variables.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Dependence on a single news source (WSJ) and LDA hyperparameters.
  - Risk of overfitting when selecting narrative topics.
  - Economic interpretation beyond correlations requires care.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Cross-validate across news sources and years.
  - Link narrative factors more tightly to macro-investment opportunities.

  </div>
</details>



---

### <a href="https://doi.org/10.1017/S0022109023000716" target="_blank">Loughran, T., & McDonald, B. (2020). Measuring Firm Complexity. .Journal of Financial and Quantitative Analysis</a>
**Year:** 2023  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Loughran & McDonald propose quantitative measures of firm complexity that capture aspects such as product heterogeneity, segmental reporting complexity, and disclosure breadth, using textual analysis of corporate filings and other firm documents. They develop metrics reflecting linguistic complexity, number of distinct product mentions, and heterogeneity of segment reporting, and link these measures to analyst coverage, forecast dispersion, and valuation multiples. The study shows that more complex firms have greater information-processing costs for investors, exhibit higher analyst forecast errors, and command valuation discounts consistent with complexity being a friction. The authors validate metrics using manual annotations and show that complexity has predictive content for future earnings surprise dispersion and price response to news. Their methodology helps operationalize an intuitive concept and provides a reproducible toolkit (dictionaries and preprocessing steps) for replication. They also discuss implications for disclosure policy: more granular reporting might reduce complexity costs, but could simultaneously increase information overload. The paper contributes by offering a systematic, text-based approach to measuring an otherwise nebulous firm attribute and tying it to asset-pricing outcomes.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - 10-K filings, MD&A sections, and segment reporting text from EDGAR.
  - Analyst forecast data and coverage measures from I/B/E/S, plus returns from CRSP.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Complexity proxies based on text could conflate deliberate obfuscation with genuine operational complexity.
  - Industry differences in jargon can bias cross-firm comparisons.
  - Policy implications require caution: more disclosure is not uniformly beneficial.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Link textual complexity to real operating measures (R&D projects, product lines) via firm-level microdata.
  - Study how complexity interacts with investor heterogeneity (institutional vs retail).

  </div>
</details>



---

### <a href="https://www.pm-research.com/content/iijjfds/5/2/100" target="_blank">Katsafados, A. G., Androutsopoulos, I., Chalkidis, I., Fergadiotis, E., Leledakis, G. N., & Pyrgiotakis, E. G. (2020). Textual Information and IPO Underpricing: A Machine Learning Approach. SSRN Electronic Journal.</a>
**Year:** 2023  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  This paper applies machine-learning text-analysis tools to S-1 filings and prospectuses to study whether textual features can predict IPO underpricing and its magnitude. The authors extract a rich set of textual features (bag-of-words, TF-IDF, topic-model scores, sentiment metrics, and linguistic complexity) and feed them into supervised ML classifiers and regression models predicting first-day returns and underpricing probability. They carefully control for standard predictors (firm size, age, proxies for information asymmetry, underwriter reputation) to isolate incremental predictive power from text. Empirically, the study shows that certain textual signals — narrative opacity, excessive promotional language, or high textual complexity — are associated with greater underpricing, consistent with information asymmetry or signaling motives at IPO. The ML models (trees, penalized regressions) outperform simple text-based linear baselines in in-sample and cross-validated performance, and the authors provide robustness checks across subsamples and time periods. They also explore which textual features carry the most economic weight using feature-importance measures and partial-dependence plots. The paper contributes to the literature by demonstrating that S-1 textual disclosures contain information relevant for pricing at IPO beyond traditional numeric controls, and by offering an ML-based toolkit for IPO underpricing research.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - S-1 prospectuses and registration statements for U.S. IPOs (text scraped from EDGAR).
  - IPO outcome variables: first-day returns, offer price, proceeds; firm fundamentals and underwriter data from CRSP/Compustat and IPO datasets; control variables for market conditions.
  - Preprocessing: text cleaning, stemming, stopword removal, TF-IDF matrices, and topic model estimation.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Textual measures are sensitive to preprocessing choices (word lists, lemmatization), and results can depend on models’ hyperparameters.
  - IPO samples vary over time and may reflect regulatory or market-structure shifts; model stability is a concern.
  - Causal interpretation is limited: textual traits may correlate with unobserved firm quality.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Use quasi-experimental variation (e.g., sudden regulatory changes in disclosure requirements) to obtain causal evidence.
  - Combine text from prospectuses with pre-IPO roadshow materials and analyst coverage for richer signal sets.
  - Cross-country comparisons to study language and disclosure regime effects.

  </div>
</details>



---

### <a href="https://doi.org/10.1111/jofi.13377" target="_blank">Bybee, Leland, Bryan Kelly, Asaf Manela, and Dacheng Xiu. Business news and business cycles. The Journal of Finance 79, no. 5 (2024): 3105-3147.</a>
**Year:** 2024  **Category:** NLP


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Constructs topical measures from Wall Street Journal business news and shows that news attention topics track macroeconomic activity and help forecast aggregate stock market returns.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Full text of Wall Street Journal articles (1984‚Äì2017), macro series, and market returns.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - News coverage may itself be endogenous to economic events.
  - Topic modeling choices and coverage biases influence results.
  - Limited to WSJ; generalizability to other media uncertain.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Apply method to broader news sources and international outlets.
  - Investigate causal channels between news narratives and real economic activity.

  </div>
</details>




## Network


---

### <a href="https://onlinelibrary.wiley.com/doi/abs/10.1111/jofi.12755" target="_blank">Richmond, R. J. (2019). Trade Network Centrality and Currency Risk Premia. The Journal of Finance, 74, 1315-1361.</a>
**Year:** 2019  **Category:** Network


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Richmond (2019) explores how countries’ positions in the global trade network explain differences in currency risk premia. The study introduces a novel measure—trade network centrality—to capture macroeconomic interdependence and its role in international asset pricing. Using a network-based econometric framework, Richmond shows that more central economies tend to have lower currency risk premia, suggesting that their currencies act as safe havens. The author integrates network theory into exchange rate modeling, bridging macro-finance and machine learning perspectives on complex interdependence. A series of predictive regressions demonstrate that trade centrality has significant explanatory power beyond standard fundamentals like interest rate differentials. The study highlights the importance of incorporating network effects in pricing models for global assets. Richmond provides robustness checks using various network measures and sub-samples to validate results. Overall, the paper establishes trade network centrality as a core determinant of international asset pricing.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - Bilateral trade flow data from the IMF and UN Comtrade, combined with exchange rates, interest rates, and macroeconomic indicators across 40+ countries spanning 1980–2015.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Trade network data is updated infrequently, limiting real-time use.
  - Model depends on assumptions about the direction and weight of trade links.
  - Difficult to isolate causality from correlation between centrality and risk premia.
  - May omit political and financial network effects.
  - High data requirements make replication challenging.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Extend to financial network centrality (banking and capital flows).
  - Study dynamic evolution of trade centrality and its link to volatility regimes.
  - Incorporate ML-based dynamic network models for real-time monitoring.

  </div>
</details>




## Survey


---

### <a href="https://onlinelibrary.wiley.com/doi/abs/10.1002/9781119751182.ch1" target="_blank">Rapach, D., & Zhou, G. (2019). Time-Series and Cross-Sectional Stock Return Forecasting: New Machine Learning Methods.</a>
**Year:** 2019  **Category:** Survey


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Summarizes and extends ML methods for return forecasting, showing elastic-net and regularization improve predictive performance and stability.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Low signal-to-noise in aggregate prediction.
  - Gains depend on evaluation setup.
  - Model tuning sensitive to breaks.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Utility-based forecast evaluation.
  - Robust model-averaging and stability selection.

  </div>
</details>



---

### <a href="https://doi.org/10.1093/rfs/hhaa019" target="_blank">Karolyi, G. A., & Van Nieuwerburgh, S. (2020). New Methods for the Cross-Section of Returns. The Review of Financial Studies, 33, 1879-1890.</a>
**Year:** 2020  **Category:** Survey


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Karolyi & Van Nieuwerburgh provide an editorial overview of methodological advances for studying the cross-section of returns, motivated by the flood of new high-dimensional data and machine-learning tools available to asset-pricing researchers. They synthesize lessons from the special issue: methods that combine economic structure (no-arbitrage constraints, factor models) with ML regularization perform better and are more interpretable than purely black-box approaches. The editorial highlights three key themes: (1) the rise of high-dimensional predictive regressions and factor discovery methods, (2) the need for transparent evaluation protocols to avoid false discoveries, and (3) the importance of economic theory in guiding ML model design. They also stress data-quality and replication concerns, urging authors to provide replication packages and vintage datasets when possible. The piece summarizes several innovative methods in the issue (IPCA, autoencoders, text-derived factors) and outlines practical research priorities: robustness checks to avoid p-hacking, careful cross-validation, and linking statistical factors to economic primitives. The editorial functions as a roadmap for researchers integrating ML into empirical asset pricing while retaining rigorous economic interpretation and inference. Finally, it calls for more work on the interpretability of ML-discovered factors and on methods to separate spurious from genuine predictive patterns

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - As an overview/editorial, it synthesizes rather than provides new empirical evidence and thus points to open problems rather than resolving them.
  - The rapid pace of ML methods means the recommendations will need updating as new tools (e.g., transformers) emerge.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Develop unified frameworks that incorporate economic constraints (no-arbitrage, investor preferences) into ML factor discovery.
  - Work on replicability standards and vintage-data benchmarks for ML in asset pricing.

  </div>
</details>



---

### <a href="http://dx.doi.org/10.2139/ssrn.3624052" target="_blank">Israel, R., Kelly, B. T., & Moskowitz, T. J. (2020). Can Machines Learn Finance? Journal of Investment Management.</a>
**Year:** 2020  **Category:** Survey


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Israel, Kelly, and Moskowitz provide a conceptual and applied survey exploring the promise and limits of machine learning for asset management, emphasizing domain-specific constraints that distinguish finance from other ML application areas. They argue that the low signal-to-noise ratio in financial returns, structural nonstationarity, and economic-feedback loops require ML practitioners to couple black-box algorithms with economic structure and careful evaluation. The authors illustrate examples where ML improves forecasting (when large high-quality data and stable relationships exist) and contrast these with cases where ML overfits spurious correlations, especially for cross-sectional factor timing and anomaly exploitation. They recommend rigorous out-of-sample testing, transaction-cost-aware evaluation, and model-interpretability diagnostics as essential safeguards. The paper also surveys practical building blocks — feature-engineering for finance, vintage data usage, and nested cross-validation — and discusses the role of ensembles and regularization in improving robustness. Importantly, they highlight operational issues (latency, data engineering) and the need for human oversight to translate model outputs into trading decisions. The piece culminates in a set of best-practice recommendations for financial ML research and industry deployment, balancing optimism with caution. Replication code and examples are often provided in the authors’ companion resources.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - The paper is largely survey/position — it does not present a single new algorithm but synthesizes practice and pitfalls.
  - Its prescriptive advice still leaves open many empirical questions about best practices across subdomains.
  - Rapid changes in ML (large models, foundation models) mean guidance needs periodic updates.

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Development of finance-specific ML benchmarks with vintage data and friction-aware metrics.
  - Work on interpretable ML and diagnostics tailored to economic decisions, including counterfactual and causal tools.
  - Research on how large pre-trained models (e.g., LLMs) can be adapted responsibly to finance while accounting for data nonstationarity.

  </div>
</details>



---

### <a href="https://oxfordre.com/economics/display/10.1093/acrefore/9780190625979.001.0001/acrefore-9780190625979-e-777" target="_blank">Rapach, D., & Zhou, G. (2021). Asset Pricing: Time-Series Predictability. Economics and Finance</a>
**Year:** 2021  **Category:** Survey


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  Rapach and Zhou (2021) offer a detailed survey of time-series predictability in asset pricing, consolidating decades of research into macroeconomic variables, technical indicators, and machine learning approaches. They examine how predictive regressions and non-linear machine learning models capture temporal dependencies in aggregate stock returns. The study revisits the empirical evidence of stock return predictability, accounting for data mining biases and structural breaks. Machine learning techniques such as random forests, boosting, and neural networks are compared with traditional predictive regressions, highlighting trade-offs in interpretability and forecasting accuracy. They show that combining models often yields more stable forecasts. The paper also discusses forecast combination, Bayesian shrinkage, and model averaging techniques in predictive modeling. The authors stress the importance of economic interpretability and out-of-sample validation. Their findings underscore that predictability is often episodic and regime-dependent, implying that consistent forecasting requires dynamic modeling frameworks.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  
  - U.S. stock market data (CRSP) spanning several decades, including returns on market indices, dividend yields, interest rates, term spreads, and macroeconomic predictors. Supplementary macroeconomic series are sourced from FRED.

  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  
  - Predictive power often vanishes out-of-sample.
  - Sensitive to structural breaks and regime shifts.
  - Machine learning models offer limited interpretability in economic terms.
  - Model combination approaches can still overfit if not carefully tuned.
  - Dependence on U.S.-centric data limits generalizability

  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Explore cross-country predictability using harmonized macro-financial data.
  - Develop interpretable ML architectures explicitly incorporating economic theory.
  - Investigate regime-switching deep learning models for adaptive predictability.

  </div>
</details>



---

### <a href="https://academic.oup.com/rfs/article/34/7/3213/6210658" target="_blank">Goldstein, I., Spatt, C. S., & Ye, M. (2021). Big Data in Finance. The Review of Financial Studies.</a>
**Year:** 2021  **Category:** Survey


<details>
  <summary><strong>Click to expand details</strong></summary>

  <div style="margin-left:1em">

  🟦 <strong><span style="color:#1E88E5">Summary</span></strong>  
  This is an overview/introduction to the “Big Data in Finance” special issue: it defines big data in finance (large size, high dimension, complex structure), surveys opportunities and challenges (identification, privacy, market design), and outlines promising directions for empirical and theoretical research at the intersection of big data and financial economics. Survey paper referencing many empirical contexts: high-frequency microstructure data, text and NLP datasets, alternative data sources (satellite, transaction, sensor, audio), and structured big datasets across finance.

  <br>

  🟩 <strong><span style="color:#43A047">Data Used</span></strong>  


  <br>

  🟧 <strong><span style="color:#FB8C00">Challenges / Limitations</span></strong>  


  <br>

  🟪 <strong><span style="color:#8E24AA">Future Research Directions</span></strong>  
  - Methodological advances for causal inference with unstructured high-dimensional data.
  - Policy and institutional studies on data access, privacy, and market fairness.
  - Development of reproducible benchmark datasets and open toolchains for big-data finance.

  </div>
</details>



---
