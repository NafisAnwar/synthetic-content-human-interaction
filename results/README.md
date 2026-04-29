# Results

This folder stores result tables, model evaluation outputs, regression summaries, and generated figures.

## Model Performance

**Best model: Sentence Embeddings + Logistic Regression**

| Metric | Value |
|--------|-------|
| Accuracy | 0.8172 |
| F1 Score | 0.3288 |
| ROC-AUC | 0.8491 |

## Main Aggregate Finding

| Statistic | Value |
|-----------|-------|
| Correlation | −0.9009 |
| Regression coefficient on synthetic prevalence | −1.4913 |
| p-value | < 0.001 |
| R² | 0.863 |

## Subreddit-Level Summary

| Subreddit | Synthetic Prevalence | h2h_ratio |
|-----------|--------------------:|----------:|
| TodayILearned | 0.1204 | 0.9680 |
| Advice | 0.2722 | 0.8142 |
| AskDocs | 0.3241 | 0.6128 |
| AskScience | 0.4061 | 0.5216 |

## Recommended File Structure
results/
│
├── model_results.csv
├── subreddit_summary.csv
├── regression_summary.txt
├── synthetic_prevalence_vs_h2h_ratio.png
└── weekly_subreddit_trends.png

## Suggested Figures

- Scatter plot of `synthetic_prevalence` vs. `h2h_ratio` (colored by subreddit)
- Bar chart of average synthetic prevalence by subreddit
- Bar chart of average h2h_ratio by subreddit
- Weekly trend lines of synthetic prevalence by subreddit
- Weekly trend lines of h2h_ratio by subreddit

> **Reminder:** Results are observational. The project finds an association between synthetic-like prevalence and lower human-to-human interaction — it does not prove causation or verified AI authorship.
