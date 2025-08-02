<p align="center">
  <img src="https://images.unsplash.com/photo-1626814026160-2237a95fc5a0?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MzJ8fG1vdmllJTIwdGhlYXRlcnxlbnwwfDB8MHx8fDA%3D" width="700" height="350">
</p>


# BOX OFFICE INTELLIGENCE: AHJIN STUDIOS' DEBUT PLAN

## Overview

Ahjin Studios is entering the original film industry at a pivotal moment. With major studios and streaming platforms in a high-stakes race to capture audience attention, the battle for box office dominance has never been more fierce, or more data-driven. While storytelling remains the heart of cinema, strategic decision-making has become its backbone.

This project is designed to fuse creativity with commercial intelligence. By analyzing industry-wide trends across genres, release timing, budgets, and audience reception, we aim to decode the anatomy of a box office hit - not just artistically, but financially. The outcome will be a tactical playbook to guide Ahjin Studios as it takes its first bold steps into feature film production.

## Business Problem

The entertainment industry is undergoing a seismic shift. Legacy franchises, tentpole films, and algorithm-fed content have saturated screens, making it harder for newcomers to break through the noise. Audiences are fragmented. Competition is global. And content fatigue is real.

For Ahjin Studios, a rising player with ambition but no prior production history, entering this landscape blind would be risky. Production budgets often stretch into the tens or hundreds of millions, and missteps in genre, budget, cast, or release timing can spell financial disaster.

**Key Questions to Answer:**
- Which genres consistently yield strong financial returns?
- What budget ranges offer the best cost-to-revenue efficiency?
- How does release timing (month, season) affect box office performance?
- To what extent do maturity ratings or runtime influence success?
- Can lower-budget films compete globally, or is scale a requirement?

## Data Understanding and Sources

This analysis leverages **five robust datasets** from major industry sources to provide a comprehensive 360° view of the modern movie landscape:

### Dataset Overview

| Dataset | Source | Size | Description |
|---------|--------|------|-------------|
| `bom.movie_gross.csv` | Box Office Mojo | 139 KB | Box office gross revenue data |
| `im.db` | IMDb | 162 MB | Comprehensive movie database with ratings, cast, crew |
| `rt.movie_info.tsv` | Rotten Tomatoes | 1.1 MB | Movie information and critic scores |
| `rt.reviews.tsv` | Rotten Tomatoes | 9.0 MB | Individual movie reviews and ratings |
| `tmdb.movies.csv` | The Movie Database | 2.2 MB | Movie metadata including genres, popularity |
| `tn.movie_budgets.csv` | The Numbers | 413 KB | Production budgets and financial data |

### Data Coverage
- **Time Period**: Recent movie releases with historical context
- **Geographic Scope**: Global box office data with focus on major markets
- **Metrics Included**: Revenue, budgets, ratings, genres, release dates, audience scores

## Analysis Methodology

### Data Processing Pipeline
1. **Data Cleaning & Integration**: Merge datasets from multiple sources
2. **Exploratory Data Analysis**: Univariate, bivariate, and multivariate analysis
3. **Trend Identification**: Genre performance, seasonal patterns, budget efficiency
4. **ROI Analysis**: Cost-to-revenue ratios across different film categories
5. **Strategic Insights**: Actionable recommendations for studio decision-making

### Key Analysis Areas
- **Genre Performance Analysis**: Financial returns by movie categories
- **Budget Optimization**: ROI analysis across different budget ranges
- **Release Strategy**: Seasonal and timing impact on box office success
- **Audience Metrics**: Correlation between ratings and commercial success
- **Market Positioning**: Competitive landscape analysis

## Repository Structure

```
Data-s-Cut/
├── README.md                          # Project documentation
├── AHJIN Studio Data Analysis - Tableau.pdf  # Tableau visualization report
├── notebooks/
│   ├── ahjin.ipynb                   # Complete notebook    
├── Raw_Data/                        # Original datasets
│   ├── bom.movie_gross.csv         # Box Office Mojo gross data
│   ├── im.db                       # IMDb database file
│   ├── rt.movie_info.tsv           # Rotten Tomatoes movie info
│   ├── rt.reviews.tsv              # Rotten Tomatoes reviews
│   ├── tmdb.movies.csv             # TMDB movie data
│   └── tn.movie_budgets.csv        # The Numbers budget data
├── zippedData/                     # Compressed dataset backups
└── images/                         # Visualization outputs and charts
```

## Getting Started

### Prerequisites
- Python 3.8+
- Jupyter Notebook
- Pandas, NumPy, Matplotlib, Seaborn
- SQLite (for IMDb database)

### Installation & Setup
1. Clone this repository
2. Install required dependencies:
   ```bash
   pip install pandas numpy matplotlib seaborn jupyter sqlite3
   ```
3. Navigate to the notebooks/ directory
4. Open ahjin.ipynb to begin analysis

### Running the Analysis
1. Run ahjin.ipynb` for initial data exploration
2. Examine the Tableau report for advanced visualizations

### Interactive Dashboard
Explore the interactive Tableau dashboard: [AHJIN Studios Data Analysis Dashboard](https://public.tableau.com/views/AHJINStudiosDataAnalysis/AHJINStudiosDataAnalysis?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## Key Findings

This analysis offers a strategic playbook for emerging studios aiming to compete intelligently in a landscape dominated by blockbuster-heavy majors. Instead of chasing trends, the data advocates for precise positioning, leaning into timing, tone, and format advantages that larger studios often overlook.

### 1. **Timing is Strategic Leverage**

* **Q4** (especially November–December) delivers the highest box office yields - ideal for emotionally rich, cinematic releases.
* **Q1–Q2** present underutilized windows for **mid-budget, high-concept films** to break out with minimal competition.

### 2. **Runtime Influences Perceived Value**

* Films running **150–180 minutes**, particularly with **PG/PG-13 ratings**, outperform shorter or extreme-length films.
* Longer runtimes signal “event cinema” and earn greater audience commitment - short runtimes often feel low-stakes or throwaway.

### 3. **PG–PG-13 is the Commercial Sweet Spot**

* These ratings dominate returns, balancing international appeal and audience breadth.
* **R-rated content** should only be greenlit for prestige plays or culturally specific narratives that demand it.

#### Hypothesis Testing Insights
**Hypothesis 1: PG/PG-13 films significantly outperform G and R-rated content**

- An ANOVA test (F = 384.31, p < 0.001) confirmed maturity ratings meaningfully impact revenue.

- PG-13 and PG films averaged over $65M, more than double the revenue of G and R-rated films (~$30M).

- **Strategic takeaway:** Prioritize PG/PG-13 for broader appeal and higher ROI, especially in early slate development.

**Hypothesis 2: Mid-budget films do not deliver better ROI than high-budget films**

- Regression analysis showed no significant ROI advantage for mid-budget films (p = 0.649).

- However, low-budget films (< $10M) showed ROI nearly 4.2× higher, suggesting strong upside in lean, creative productions.

- **Strategic takeaway:** Avoid assuming mid-budget safety. Instead, target low-budget productions for early capital efficiency.

### 4. **Genre is Financial Strategy**

* While action and comedy top revenue charts, **leaner genres** like thriller, drama, and mystery provide high ROI when strategically positioned.
* Emphasis should be on **genre hybrids** and **story-driven narratives**, not VFX-heavy productions that strain early-stage budgets.

### 5. **Budgeting is a Precision Tool**

* High returns are more closely tied to **budget alignment** than budget size.
* Studios should implement **tiered investment strategies** and **data-driven greenlighting** at the development stage, not just in post-production.

### Strategic Recommendation Summary

* **Time major releases for Q4** to capture holiday box office surges.
* **Default to PG/PG-13 ratings** for broader reach and international viability.
* **Blend genres smartly** — avoid bloated VFX productions until scale permits.
* **Use runtime, tone, and rating as market cues**, not just artistic choices.
* **Build budget discipline into the pipeline**, aligning spend to project scale and market fit.

## Deliverables

- ✅ Cleaned and integrated datasets from five industry sources
- ✅ Comprehensive exploratory data analysis
- ✅ Data visualizations illustrating box office trends and ROI benchmarks
- ✅ Strategic summary with investment-ready recommendations
- ✅ Executive-ready presentation materials

## Future Enhancements

- Integration of streaming platform data
- Real-time market sentiment analysis
- Predictive modeling for box office forecasting
- International market expansion analysis

## Contact

For questions about this analysis, please contact the data science team:

Mary - https://www.linkedin.com/in/marykamithi?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=android_app

Norman - https://www.linkedin.com/in/norman-mwapea-49502a264/



**Note**: This analysis is designed to inform strategic decision-making at a fictional newbie movie studio (Ahjin Studios). All recommendations should be considered alongside creative vision and market intuition.

