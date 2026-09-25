# Netflix Data Analysis | Exploratory Data Analysis

## Project Overview

This project performs exploratory data analysis (EDA) on the **Netflix Titles** dataset to examine patterns in the catalog across content type, countries, ratings, genres, directors, and duration.

The analysis focuses on what the dataset can directly show about Netflix's catalog composition and historical content additions. It does **not** attempt to infer Netflix's internal investment decisions, audience preferences, or viewer engagement from catalog metadata alone.

---

## Dataset

**Source:** Kaggle — Netflix Titles dataset

The notebook loads the dataset from the Kaggle environment. If you run the notebook outside Kaggle, update the dataset path to the local location of `netflix_titles.csv`.

The dataset contains title-level metadata including:

- Content type
- Title
- Director
- Cast
- Country
- Date added
- Release year
- Rating
- Duration
- Genres
- Description

---

## Tools & Technologies

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Jupyter Notebook

---

## Analysis Workflow

1. Dataset understanding
2. Missing-value and duplicate analysis
3. Data cleaning
4. Date conversion and time-based analysis
5. Movie vs. TV Show distribution
6. Country representation
7. Year-wise content additions
8. Rating distribution
9. Director analysis
10. Cast analysis
11. Genre analysis
12. Duration analysis
13. Summary of findings and analytical limitations

---

## Key Findings

- **Movies represent the majority of titles** in the dataset, accounting for about 69.62% of titles, while TV Shows account for about 30.38%.
- **The United States is the most frequently represented country** after multi-country entries are split into individual country values.
- **TV-MA is the most common rating** in the dataset. This describes catalog composition and does not, by itself, establish Netflix's overall audience-targeting strategy.
- **International Movies, Dramas, and Comedies** are among the most frequently represented genre labels after multi-genre entries are split.
- Common duration labels include **1 Season, 2 Seasons, 3 Seasons, and 90-minute movies**.
- The yearly `date_added` analysis shows substantial variation in the number of titles added across the years represented in the dataset.

---

## Data Cleaning & Analysis Notes

Several fields contain multiple values in a single row. For meaningful category-level analysis, the notebook splits and explodes:

- Countries
- Directors
- Genres

The `date_added` field is parsed using mixed-format date handling to avoid unnecessarily losing valid date values.

Missing values are handled where appropriate, while the original catalog structure is preserved for exploratory analysis.

---

## Skills Demonstrated

- Data Cleaning
- Exploratory Data Analysis (EDA)
- Data Visualization
- Missing-Value Analysis
- Categorical Data Analysis
- Time-Series/Date-Based Analysis
- Business-Oriented Data Interpretation
- Handling Multi-Value Categorical Fields

---

## Repository Structure

```
netflix-business-insights/
├── README.md
└── netflix-business-insights.ipynb
```

---

## Analytical Limitations

This project analyzes **catalog metadata**, not Netflix's internal business or user-level data.

Therefore, the dataset alone cannot establish:

- Netflix's actual content investment decisions
- Viewer preferences or engagement
- Causal relationships between catalog characteristics and business outcomes
- Netflix's current strategy
- Whether a particular genre, rating, or format performs better with viewers

The findings should therefore be interpreted as **descriptive observations about the dataset**.

---

## Project Outcome

This project provided practical experience with real-world data cleaning, exploratory analysis, visualization, categorical data handling, date-based analysis, and communicating data-driven observations without overstating what the dataset can support.

## Author

**Sachin Kumar**
