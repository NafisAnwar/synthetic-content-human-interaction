# Data

Raw Reddit data is **not included** in this repository. Raw comments may contain sensitive user-generated content, particularly from communities such as r/AskDocs and r/Advice.

## Local Data Structure

<img width="280" height="530" alt="image" src="https://github.com/user-attachments/assets/98a820b9-cef9-409e-955a-09d626b3524b" />

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
