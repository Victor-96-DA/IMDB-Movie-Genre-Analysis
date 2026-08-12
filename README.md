# IMDB Movie Genre Analysis (1960 - 2015)
 
## Project Overview
A Python-based exploratory data analysis project investigating movie genre 
trends, financial performance, audience popularity and critical ratings 
across 55 years of IMDB movie data.
 
📓 **[View Full Analysis Notebook](Movie_Genre_Data_Analysis.ipynb)**
 
## Tools & Libraries
- Python
- pandas
- matplotlib
- seaborn
- Jupyter Notebook
## Dataset
- **Source:** IMDB Movie Dataset
- **Period:** 1960 - 2015
- **Original size:** 10,865 movies
- **After cleaning:** 3,854 movies with complete financial records
- **Note:** Inflation-adjusted financial values used throughout 
  for cross-year comparability
## Research Questions
1. Which genres are the most common (number of movies made)? 
   Includes trend analysis - are certain genres growing or declining 
   across the 55 years?
2. Which genres have high average budget and revenue? 
   Includes variance analysis - examining whether high averages are 
   reliable or skewed by blockbuster outliers. Also examines average profit.
3. Which genres have high average popularity? 
   Cross-examined with Q1 - a genre can be popular with few movies made, 
   or have many movies but low popularity per film.
4. Which genres have the highest number of movies with a vote average ≥ 8? 
   Includes hit rate analysis - percentage of each genre's total movies 
   hitting the threshold for a fair proportional comparison.
5. What is the average profit per year of each genre? 
   Inflation-adjusted values used throughout to ensure cross-year 
   comparability across the 55-year dataset.
## Hypotheses Tested
1. The best movies by vote average return high profit and revenue
2. The best movies by popularity return high profit and revenue
3. Highly budgeted movies return high revenue and profit
4. Highly budgeted movies have high popularity
## Key Findings
- Drama dominates production volume with 1,756 movies but ranks low in popularity and revenue
- Science Fiction, Adventure and Animation lead in both popularity and commercial returns
- High critical ratings do not correlate with commercial success; popularity is the stronger driver
- Average revenue figures are unreliable across all genres due to blockbuster outliers
- Animation has the highest median revenue of any genre, yet its average is still inflated by outliers, showing that even strong-performing genres aren't immune to this distortion
- Science Fiction, Documentary and Drama show the widest gap between median and mean, making their averages the least reliable in the dataset
- Production budget strongly predicts revenue (0.7 correlation) but not profit (0.3)
## Project Structure
```
IMDB-Movie-Genre-Analysis/
│
├── Movie_Genre_Data_Analysis.ipynb    ← Main analysis notebook
├── README.md                          ← Project documentation
└── charts/                            ← Exported visualizations
    ├── genre_frequency.png
    ├── genre_trend_heatmap.png
    ├── budget_revenue_by_genre.png
    ├── variance_analysis.png
    ├── revenue_boxplot.png
    └── profit_heatmap.png
```
 
## Methodology Notes
- Zero values in budget and revenue treated as missing data and excluded
- Inflation-adjusted values (budget_adj, revenue_adj) used for all 
  financial analysis to ensure fair cross-year comparison
- Variance analysis conducted alongside averages to assess reliability 
  of mean values
- Hit rate analysis added to Q4 to provide proportional comparison 
  beyond raw counts
## Author
**Victor Olatunji**
- GitHub: https://github.com/Victor-96-DA?tab=repositories
- Gmail: reachvictorola@gmail.com
---
© 2026 Victor Olatunji | Data Analyst | Doha, Qatar
