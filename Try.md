# Machine Learning in Asset Pricing — Literature Review

This repository presents a comprehensive collection of academic papers exploring the intersection of **machine learning** and **asset pricing**.  
Each paper entry includes a collapsible summary with data descriptions, limitations, and potential future research directions.

## Table of Contents

- [Accounting / NLP](#accounting-/-nlp)
- [Accounting / fraud detection (ML applied)](#accounting-/-fraud-detection-(ml-applied))
- [Accounting / misstatement detection](#accounting-/-misstatement-detection)
- [Alternative data / NLP](#alternative-data-/-nlp)
- [Alternative data / computer vision (asset pricing application)](#alternative-data-/-computer-vision-(asset-pricing-application))
- [Alternative data / narrative factors](#alternative-data-/-narrative-factors)
- [Alternative data / news NLP](#alternative-data-/-news-nlp)
- [Corporate disclosure / NLP](#corporate-disclosure-/-nlp)
- [Factor construction / tree-based methods](#factor-construction-/-tree-based-methods)
- [Factor discovery / representation learning/Latent factor models](#factor-discovery-/-representation-learning/latent-factor-models)
- [Fixed income / macro-finance](#fixed-income-/-macro-finance)
- [Fixed income / prediction](#fixed-income-/-prediction)
- [Fundamental analysis / ML](#fundamental-analysis-/-ml)
- [High-frequency / microstructure ML](#high-frequency-/-microstructure-ml)
- [Human+AI / analyst forecasting](#human+ai-/-analyst-forecasting)
- [Macroeconomic expectations / ML](#macroeconomic-expectations-/-ml)
- [Methodology / inference with ML](#methodology-/-inference-with-ml)
- [Momentum / deep learning](#momentum-/-deep-learning)
- [Prediction / economic restrictions](#prediction-/-economic-restrictions)
- [Prediction / forecasting](#prediction-/-forecasting)
- [Prediction / forecasting (market-specific)](#prediction-/-forecasting-(market-specific))
- [Prediction / industry-focused methods](#prediction-/-industry-focused-methods)
- [SDF estimation / deep learning](#sdf-estimation-/-deep-learning)
- [Structural estimation / deep learning](#structural-estimation-/-deep-learning)
- [Uncategorized](#uncategorized)

---



<style>
body {
  font-family: 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;
  background-color: #ffffff;
  line-height: 1.6;
  color: #222;
}

.paper-card {
  background-color: #f9fafb;
  border-left: 4px solid #004aad;
  border-radius: 8px;
  padding: 1.2em 1.4em;
  margin-bottom: 1.5em;
  box-shadow: 0 1px 3px rgba(0,0,0,0.06);
  transition: all 0.25s ease;
}

.paper-card:hover {
  background-color: #f3f6fb;
  box-shadow: 0 4px 8px rgba(0,0,0,0.08);
}

details {
  background-color: #fdfdfd;
  border: 1px solid #ddd;
  border-radius: 6px;
  padding: 0.7em 1em;
  margin-top: 0.8em;
  transition: background-color 0.3s ease;
}

summary {
  font-weight: 600;
  color: #003366;
  cursor: pointer;
}

.content-block {
  margin-top: 0.5em;
  color: #333;
  line-height: 1.55;
  font-size: 0.96em;
}

hr.section {
  border: none;
  height: 1px;
  background-color: #e0e0e0;
  margin: 1.5em 0;
}

h2 {
  border-bottom: 2px solid #ddd;
  padding-bottom: 0.3em;
  margin-top: 1.4em;
  color: #004aad;
}
</style>


## Accounting / NLP


<div class="paper-card">

### [Brown, N. C., Crowley, R. M., & Elliot, W. B. (2019). What are You Saying? Using topic to Detect Financial Misreporting. Journal of Accounting Research.](Wiley / SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=2803733)
**Year:** 2019/2020  **Category:** Accounting / NLP


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Introduces topic-based textual features to detect financial misreporting and shows topic models significantly improve out-of-sample detection performance. Demonstrates text topics add information beyond traditional style and financial features. </p>
    <p><strong>Data Used:</strong> 10-K filings text, SEC enforcement actions (AAERs), restatements, and financial statement data.</p>
    <p><strong>Challenges / Limitations:</strong> Topic models capture co-occurrence patterns but may miss nuanced or cleverly disguised language.
- Label and event-timing uncertainty for misreporting cases complicate evaluation.
- Language drift over time may require periodic model retraining.</p>
    <p><strong>Future Research Directions:</strong> Combine topic models with supervised deep-learning classifiers for richer feature sets.
- Develop time-adaptive topic models to handle language evolution.
- Evaluate cross-lingual transferability for international filings.</p>
  </div>
</details>

</div>


## Accounting / fraud detection (ML applied)


<div class="paper-card">

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

</div>


## Accounting / misstatement detection


<div class="paper-card">

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

</div>


## Alternative data / NLP


<div class="paper-card">

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

</div>


## Alternative data / computer vision (asset pricing application)


<div class="paper-card">

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

</div>


## Alternative data / narrative factors


<div class="paper-card">

### [Bybee, L., Kelly, B., Su, Y. (2022). Narrative Asset Pricing: Interpretable Systematic Risk Factors from News Text. SSRN.](https://onlinelibrary.wiley.com/doi/full/10.1111/jofi.13377)
**Year:** 2022/2023  **Category:** Alternative data / narrative factors


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Extracts narrative factors from WSJ news text using LDA + IPCA + group lasso and shows these news-derived factors have strong pricing performance and high out-of-sample Sharpe ratios. Shows that news attention topics track macroeconomic activity and help forecast aggregate stock market returns.</p>
    <p><strong>Data Used:</strong> Wall Street Journal text, returns on anomaly portfolios, macro variables.</p>
    <p><strong>Challenges / Limitations:</strong> Dependence on a single news source (WSJ) and LDA hyperparameters.
- Risk of overfitting when selecting narrative topics.
- Economic interpretation beyond correlations requires care.</p>
    <p><strong>Future Research Directions:</strong>  Cross-validate across news sources and years.
- Link narrative factors more tightly to macro-investment opportunities.</p>
  </div>
</details>

</div>


## Alternative data / news NLP


<div class="paper-card">

### [Bybee, L., Kelly, B., Manela, A. (2021). Business News and Business Cycles](SSRN: https://papers.ssrn.com/sol3/papers.cfm?abstract_id=3446225 ; Journal link: https://onlinelibrary.wiley.com/doi/full/10.1111/jofi.13377)
**Year:** 2024  **Category:** Alternative data / news NLP


<details class="paper-details">
  <summary><strong>View Details</strong></summary>
  <div class="content-block">
    <p><strong>Summary:</strong> Constructs topical measures from Wall Street Journal business news and shows that news attention topics track macroeconomic activity and help forecast aggregate stock market returns.</p>
    <p><strong>Data Used:</strong> Full text of Wall Street Journal articles (1984‚Äì2017), macro series, and market returns.</p>
    <p><strong>Challenges / Limitations:</strong> - News coverage may itself be endogenous to economic events.
- Topic modeling choices and coverage biases influence results.
- Limited to WSJ; generalizability to other media uncertain.</p>
    <p><strong>Future Research Directions:</strong> Apply method to broader news sources and international outlets.
- Investigate causal channels between news narratives and real economic activity.</p>
  </div>
</details>

</div>
