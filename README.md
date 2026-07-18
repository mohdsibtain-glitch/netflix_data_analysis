netflix_data_analysis
# 🎬 Netflix Data Analysis- (SQL, Python, Power BI)

A fresher-level data analytics portfolio project exploring the Netflix titles dataset (8,807 titles, 1925–2021) using **Python (Pandas/Matplotlib/Seaborn)** and **SQL**, presented as an interactive HTML report.

## 📁 Dataset

- **Source:** [Netflix Movies and TV Shows dataset (Kaggle)](https://www.kaggle.com/datasets/shivamb/netflix-shows) — `netflix_titles.csv`
- **Size:** 8,807 titles
- **Range:** 1925–2021
- **Columns:** type, title, director, cast, country, date_added, release_year, rating, duration, listed_in (genres), description

## 📊 Key Findings

| Metric | Value |
|---|---|
| Total titles | 8,807 |
| Movies | 6,131 (69.6%) |
| TV Shows | 2,676 (30.4%) |
| Unique countries | 748 |
| Peak content year | 2019 (1,424 titles added) |
| Top genre | Drama (36% of titles) |
| Most common rating | TV-MA (3,207 titles) |

**Insights:**
- **Rapid growth 2015–2019** — additions grew from 429 titles (2015) to a peak of 1,424 (2019), then slowed post-COVID.
- **USA dominates production** — the US accounts for 36% of content; India is the #2 producer with 972 titles.
- **Adult-skewed catalog** — TV-MA is the most common rating, signaling an adult-first audience strategy.
- **Movies outnumber shows ~2:1** — despite streaming being TV-native, 70% of the catalog is movies, suggesting heavy licensing of film libraries.
- **January & October are peak add-months** — likely tied to New Year and pre-holiday content strategy.
- **Short-lived TV shows** — 67% of TV shows have only a single season.

## 🧭 Report Sections

The HTML report is organized into five tabs:

1. **Overview** — KPI cards, titles added per year, Movies vs TV Shows split, top 10 genres, content ratings, monthly additions
2. **Content** — top 10 producing countries, season-count distribution, movie duration distribution, movies vs shows trend over time
3. **Insights** — six headline takeaways plus top directors by title count
4. **Python code** — reusable snippets: load/explore, data cleaning, EDA, visualizations (bar/doughnut/heatmap), word cloud, ratings/audience analysis
5. **SQL queries** — 8 analysis queries: type split, top countries, yearly trend, rating distribution, top directors, India vs USA comparison, month-wise additions, TV shows with most seasons

## 🛠️ Tech Stack

- **Python:** pandas, numpy, matplotlib, seaborn, wordcloud
- **SQL:** MySQL-flavored analytical queries (aggregation, `GROUP BY`, `CASE`, string functions)
- **Frontend:** Plain HTML/CSS + [Chart.js 4.4.1](https://www.chartjs.org/) for charts, CSS custom properties for theming, Tabler Icons for iconography

## 🚀 Getting Started

### View the report
No build step needed — it's a self-contained HTML file:
```bash
python3 -m http.server 8000
```
Then open `http://localhost:8000/netflix_data_analysis.html`

### Reproduce the analysis
1. Download `netflix_titles.csv` from Kaggle (link above)
2. Install dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn wordcloud
   ```
3. Run the Python snippets from the **Python code** tab in a Jupyter notebook or script
4. Load the same CSV into a MySQL table named `netflix` to run the **SQL queries** tab

## 📄 License

Feel free to use, adapt, and extend this project for your own portfolio.
