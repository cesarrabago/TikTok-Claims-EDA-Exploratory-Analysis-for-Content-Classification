# TikTok Claims EDA — Exploratory Analysis for Content Classification

> Exploratory data analysis of **19,382 TikTok videos** as the groundwork for a
> *claim vs. opinion* classification model. Carried out under the **PACE**
> framework (Plan, Analyze, Construct, Execute).

📄 **[Read the full analysis (PDF, 11 pages)](TIKTOK_PROJECT.pdf)**

---

## Project context

As part of the **Google Advanced Data Analytics Certificate** (Course 2 — Get
Started with Python), I worked as a data analyst in a simulated TikTok scenario.
Leadership approved the proposal to build a claims classification model, and
this analysis delivers the first structured EDA that the later modeling work
builds on.

## Objectives

- Understand the structure of the dataset (12 columns, 19,382 records)
- Identify null values, outliers, and data quality issues
- Compare engagement between `claim` and `opinion` videos
- Investigate the relationship between `author_ban_status` and engagement metrics
- Compute engagement rates (likes/view, shares/view, comments/view)

## Key insights

| Finding | Figure |
|---|---|
| Claim vs opinion distribution | ~49.6% claims · ~48.9% opinions · ~1.5% unclassified |
| Mean views — claim vs opinion | **501,029** vs 4,956 (≈100× more) |
| Median shares — banned vs active | **14,468** vs 437 (33× more) |
| Mean likes/view — claim vs opinion | 0.33 vs 0.22 |

**Conclusion:** *Claim* videos are significantly more viral and generate higher
engagement per view than opinions. Authors with banned or under-review accounts
show disproportionately high metrics — a critical pattern for content
moderation strategy.

## Methodology (PACE)

- **Plan:** Reviewed the data dictionary and categorized the variables (content
  attributes, author attributes, engagement metrics)
- **Analyze:** `head()`, `info()`, `describe()`, null and outlier detection
- **Construct:** Built derived columns (`likes_per_view`, `shares_per_view`,
  `comments_per_view`)
- **Execute:** Executive synthesis answering the questions raised by the TikTok
  team

## Stack

- Python 3 · pandas · numpy
- Jupyter Notebook
- PACE framework for the structure of the analysis

## Files

- [`TIKTOK_PROJECT.pdf`](TIKTOK_PROJECT.pdf) — Full analysis: code, output, and
  commentary, exported from the notebook

---

*Google Advanced Data Analytics Certificate project · César Rábago Pérez · 2025*
