# Overview
This project analyzes opioid-related Facebook ads to understand how digital advertising interacts with the U.S. opioid epidemic. Using natural language processing (NLP), topic modeling, and causal inference techniques, I explored how ad exposure by category and geography correlates with opioid-related deaths across states. (If you would like to see all the ad data files please email me at daikisai77@gmail.com)

# Data Pipeline
## Data Collection:
    - Scraped opioid-related ads from the Facebook Ads Library using APIFY.
    - Extracted ad body text, timestamps, and engagement metadata.
## Preprocessing:
    - Cleaned and tokenized ad text.
    - Extracted hashtags, keywords, and geographic mentions.
    - Removed stopwords and standardized text formatting.
## Categorization:
    - Classified ads into Treatment & Recovery, Prevention & Awareness, Products, and Research/Support using:
    - Latent Dirichlet Allocation (LDA) topic modeling.
    - Sentence-BERT embeddings for semantic clustering.

## Geolocation Extraction:
    - Used spaCy Named Entity Recognition (NER) to identify U.S. states and cities.
    - Mapped ads to regional exposure levels.
    
# Analysis
## Difference-in-Differences (DiD) Regression:
    - Compared states with high vs. low ad exposure.
    - Incorporated opioid settlement payouts as a treatment variable.
    - Estimated category-specific effects on opioid mortality trends.
## Word2Vec Visualizations:
    - Highlighted narrative shifts in opioid-related discussions pre- vs. post-2022.
## Trend Plots with Confidence Intervals:
    - Visualized pre- and post-treatment trends across ad categories.

# Tools & Libraries
    - **Python:** pandas, scikit-learn, statsmodels, matplotlib, seaborn
    - **NLP:** spaCy, gensim (LDA), sentence-transformers (BERT), Word2Vec
    - **Causal Inference:** statsmodels (Difference-in-Differences)

# Results & Insights
    - **Prevention & Awareness ads** correlated with greater reductions in opioid deaths than product-based ads.
    - Settlement payouts amplified the relationship between ad exposure and mortality outcomes.
    - Text embeddings revealed evolving narratives around opioids after 2022.

# Author
## Daiki Sai
daikisai77@gmail.com | https://www.linkedin.com/in/daiki-sai/

  

Visualized pre- and post-treatment trends across ad categories.

