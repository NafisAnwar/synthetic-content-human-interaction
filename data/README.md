# Data

Raw Reddit data is **not included** in this repository. Raw comments may contain sensitive user-generated content, particularly from communities such as r/AskDocs and r/Advice.

## Local Data Structure

If reproducing the project locally, organize data as follows:
data/
│
├── raw/
│   ├── askscience_raw_comments.csv
│   ├── todayilearned_raw_comments.csv
│   ├── askdocs_raw_comments.csv
│   └── advice_raw_comments.csv
│
├── clean/
│   ├── askscience_clean_comments.csv
│   ├── todayilearned_clean_comments.csv
│   ├── askdocs_clean_comments.csv
│   └── advice_clean_comments.csv
│
├── labels/
│   ├── balanced_label_sample.csv
│   ├── overlap_label_sample.csv
│   └── final_labeled_comments.csv
│
├── processed/
│   ├── scored_comments.csv
│   └── subreddit_week_analysis.csv
│
└── logs/
├── comment_exclusions.csv
├── template_removed_comments.csv
└── removed_meta_threads.csv

## Data Stages

| Stage | Contents |
|-------|----------|
| **Raw** | Collected Reddit comments before any filtering |
| **Clean** | Comments after removing blank, deleted, removed, moderator/system, template, meta-thread, and broken-chain rows |
| **Labels** | Comments selected for manual annotation with human-like (`0`) / synthetic-like (`1`) / unsure (`-1`) labels |
| **Processed** | Model scores and final subreddit-week metrics used in regression analysis |

The main file used in the final analysis is `processed/subreddit_week_analysis.csv`.

## Privacy Note

Do not publicly upload raw Reddit comments unless required and you have removed unnecessary personal identifiers. The preferred public-facing version of this project focuses on methodology, aggregate results, and reproducible code.
