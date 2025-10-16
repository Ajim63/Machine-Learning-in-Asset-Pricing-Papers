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


# 🧠 Machine Learning in Asset Pricing — Literature Review

A curated academic literature collection on **machine learning applications in asset pricing**.  
Each entry includes collapsible sections with summaries, data details, limitations, and future directions — all styled for readability.

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

<p align="center">
<sub>Compiled for educational and research purposes. © Machine Learning in Asset Pricing Repository</sub>
</p>
