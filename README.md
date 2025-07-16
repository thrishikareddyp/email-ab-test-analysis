# 📬 A/B Test Analysis: Do Subject Lines Impact Open Rates?

# Overview
Curious about how small changes in marketing affect engagement, I analyzed a real-world email campaign dataset to test whether different subject lines influenced open rates.

Using real campaign data from Kaggle, I simulated an A/B test comparing two email subject line variants (Campaign_Type A vs B). I measured user engagement using clicks as a proxy for opens and applied a 2-proportion z-test to assess statistical significance.

# Dataset
- Source: [Marketing Campaign Performance Dataset](https://www.kaggle.com/datasets/manishabhatt22/marketing-campaign-performance-dataset)
- Filtered for `Channel_Used = Email`
- Two most common `Campaign_Type`s used as A/B test groups
- Created binary `opened_email` column from click data

# A/B Test Details

| Group | Opened | Total | Conversion Rate |
|-------|--------|-------|-----------------|
| A     | 5048   | 6760  | 74.67%          |
| B     | 5012   | 6722  | 74.56%          |

- **Z-score**: 0.151  
- **P-value**: 0.8797  
- ✅ Conclusion: No statistically significant difference (p > 0.05)

# Key Learnings
- Not every change drives a measurable impact — and that’s important to know
- A/B testing is powerful, but it's also about recognizing when the needle *doesn’t* move
- Translating results into a clear business recommendation is just as valuable as finding a win

# Tools Used
- Python (Pandas, NumPy, SciPy, Matplotlib)
- Google Colab
- Kaggle API

# Files
- `email_ab_real_cleaned.csv` – Cleaned dataset
- `ab_test_analysis.ipynb` – Notebook with analysis, charts, and interpretation

# Credits
Inspired by real-world questions in marketing analytics. Dataset from Kaggle. Analysis and write-up by [Your Name].
