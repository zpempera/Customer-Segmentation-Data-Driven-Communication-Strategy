# Customer Segmentation for Data-Driven Marketing

**RFM Analysis & K-Means Clustering on two years of retail customer data**

End-to-end customer analytics project: from data audit to actionable segment-level
communication strategy. Built on the Customer Personality Analysis dataset (~2,200
customers, 2 years of transactions).

## Objective

A retail company collected two years of customer data but lacked a framework to act on
it. This project cleans the data, engineers RFM features, segments customers using both a
rule-based heuristic and unsupervised learning, and recommends a tailored communication
channel and tone for each segment.

## Workflow

1. **Data Audit & Cleaning** — handled missing income values, removed implausible birth
   years and an extreme income outlier, engineered features (age, tenure, total spend),
   one-hot encoded categoricals.
2. **Exploratory Data Analysis** — correlation of socio-demographics with spending,
   channel distribution, and a hidden trend (low-income households with young children
   are budget-conscious and discount-driven).
3. **RFM Segmentation** — quintile scoring on Recency, Frequency, Monetary; four heuristic
   segments (Champions, Loyal, At Risk, Lost / Low-Value).
4. **K-Means Clustering** — standardised features, k selected via Elbow + Silhouette
   (k=4); clusters profiled and cross-compared with RFM.
5. **Communication Strategy** — channel and message tone recommended per cluster.

## Key Insight

K-Means revealed structure RFM missed: the single "Lost / Low-Value" RFM segment actually
splits into two behaviourally distinct groups — recent low-spenders worth nurturing, and
genuinely dormant customers worth little investment — separated mainly by recency.

## Tech Stack

Python · pandas · NumPy · scikit-learn · matplotlib · seaborn

## How to Run

Open `notebook.ipynb` in Google Colab or Jupyter. The dataset loads directly from this
repository, so no manual download is required.

\`\`\`bash
pip install -r requirements.txt
\`\`\`


## Author

[Imię Nazwisko] — B.Sc. in Artificial Intelligence
