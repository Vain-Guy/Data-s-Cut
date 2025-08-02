<p align="center">
  <img src="https://images.unsplash.com/photo-1626814026160-2237a95fc5a0?w=600&auto=format&fit=crop&q=60&ixlib=rb-4.1.0&ixid=M3wxMjA3fDB8MHxzZWFyY2h8MzJ8fG1vdmllJTIwdGhlYXRlcnxlbnwwfDB8MHx8fDA%3D" width="300">
</p>


# BOX OFFICE INTELLIGENCE: AHJIN STUDIOS' DEBUT PLAN

## 🎬 Project Overview

Ahjin Studios is entering the original film industry at a pivotal moment. With major studios and streaming platforms in a high-stakes race to capture audience attention, the battle for box office dominance has never been more fierce, or more data-driven. While storytelling remains the heart of cinema, strategic decision-making has become its backbone.

This project is designed to fuse creativity with commercial intelligence. By analyzing industry-wide trends across genres, release timing, budgets, and audience reception, we aim to decode the anatomy of a box office hit - not just artistically, but financially. The outcome will be a tactical playbook to guide Ahjin Studios as it takes its first bold steps into feature film production.

## 🎯 Business Problem

The entertainment industry is undergoing a seismic shift. Legacy franchises, tentpole films, and algorithm-fed content have saturated screens, making it harder for newcomers to break through the noise. Audiences are fragmented. Competition is global. And content fatigue is real.

For Ahjin Studios, a rising player with ambition but no prior production history, entering this landscape blind would be risky. Production budgets often stretch into the tens or hundreds of millions, and missteps in genre, budget, cast, or release timing can spell financial disaster.

**Key Questions to Answer:**
- Which genres consistently yield strong financial returns?
- What budget ranges offer the best cost-to-revenue efficiency?
- How does release timing (month, season) affect box office performance?
- To what extent do maturity ratings or runtime influence success?
- Can lower-budget films compete globally, or is scale a requirement?

## 📊 Data Understanding and Sources

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

## 🔬 Analysis Methodology

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

## 📁 Repository Structure

```
Data-s-Cut/
├── README.md                          # Project documentation
├── AHJIN Studio Data Analysis - Tableau.pdf  # Tableau visualization report
├── notebooks/
│   ├── exploratory.ipynb            # Initial data exploration and analysis
│   └── final.ipynb                  # Final analysis and recommendations
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

## 🚀 Getting Started

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
3. Navigate to the `notebooks/` directory
4. Open `exploratory.ipynb` to begin analysis

### Running the Analysis
1. Start with `exploratory.ipynb` for initial data exploration
2. Review `final.ipynb` for comprehensive analysis and recommendations
3. Examine the Tableau report for advanced visualizations

### 📊 Interactive Dashboard
Explore the interactive Tableau dashboard: [AHJIN Studios Data Analysis Dashboard](https://public.tableau.com/views/AHJINStudiosDataAnalysis/AHJINStudiosDataAnalysis?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

## 📈 Key Findings & Insights

### 🎬 Release Strategy Optimization

#### **Seasonal Release Patterns**
- **December dominates** with 745 releases, capitalizing on holiday box office and award-season positioning
- **October shows strong activity** (573 releases) driven by horror/thriller genre popularity around Halloween
- **January and February are quieter periods** (347 and 392 releases respectively), representing strategic cooldown after holidays
- **Friday releases account for 4,539 theatrical premieres** - the clear industry standard maximizing weekend box office potential

#### **International vs. Domestic Revenue Dynamics**
- **Foreign revenue consistently outpaces domestic** across multiple films, with international audiences often leading revenue generation
- **Some films achieve international success despite modest U.S. performance**, indicating diverse regional preferences
- **Most commercially viable films generate $100M-$600M** in combined domestic and foreign gross revenue
- **Success isn't tied to release year** - films from 2010 still compete effectively with 2018 releases

### 🎭 Genre Performance Intelligence

#### **High-Performing Genre Categories**
- **Romance and Thriller genres** occasionally achieve exceptional popularity (80+ popularity scores) with strong audience ratings
- **Drama and Science Fiction** consistently earn quality ratings (7.5+ vote averages) even when not dominating popularity charts
- **Documentary, TV Movies, and War genres** serve niche but loyal audiences with more modest performance metrics
- **Action and Adventure films** show consistent presence across multiple revenue tiers

#### **Audience Engagement Patterns**
- **Quality and popularity don't always correlate** - some genres excel in critical reception while others dominate mass appeal
- **Genre diversification across international markets** shows different regional preferences for storytelling styles
- **Seasonal genre preferences** influence October release strategies (horror/thriller optimization)

### 💰 Budget and ROI Strategic Insights

#### **Budget Range Performance**
- **Mid-range budget films ($10M-$100M)** show optimal cost-to-revenue efficiency for new studio entry
- **Blockbuster budgets (hundreds of millions)** carry high risk without established franchise or A-list talent
- **Lower-budget films can compete globally** when targeting specific genre niches and international markets
- **Production budget allocation** should consider international market potential from project inception

#### **Revenue Optimization Factors**
- **Runtime and maturity ratings** influence box office performance across different audience segments
- **Release timing coordination** with genre preferences maximizes market penetration
- **International market prioritization** can offset domestic underperformance for strategic content

### 🎯 Market Positioning Recommendations

#### **New Studio Entry Strategy**
- **Focus on mid-budget original content** rather than competing directly with established blockbuster franchises
- **Prioritize genres with consistent international appeal** (Drama, Science Fiction, Thriller)
- **Leverage strategic release timing** (October for thrillers, December for prestige content)
- **Develop content with global storytelling elements** to maximize international revenue potential

#### **Risk Mitigation Approaches**
- **Diversify genre portfolio** to balance critical acclaim with commercial viability
- **Consider co-production strategies** for international market penetration
- **Plan release strategies 12-18 months in advance** to secure optimal calendar positioning
- **Invest in data-driven decision making** for budget allocation and genre selection

### Strategic Recommendations

- **Genre Focus**: Prioritize Drama, Thriller, and Science Fiction for consistent performance with international appeal
- **Budget Allocation**: Target $15M-$75M production budgets for optimal ROI without excessive risk
- **Release Timing**: Secure December slots for prestige content, October for genre films, avoid January/February
- **Market Positioning**: Develop internationally-minded content from conception, not as an afterthought

## 🎯 Deliverables

- ✅ Cleaned and integrated datasets from five industry sources
- ✅ Comprehensive exploratory data analysis
- ✅ Data visualizations illustrating box office trends and ROI benchmarks
- ✅ Strategic summary with investment-ready recommendations
- ✅ Executive-ready presentation materials

## 🔮 Future Enhancements

- Integration of streaming platform data
- Real-time market sentiment analysis
- Predictive modeling for box office forecasting
- International market expansion analysis

## 📞 Contact

For questions about this analysis or Ahjin Studios' strategic planning, please contact the data science team.

---

**Note**: This analysis is designed to inform strategic decision-making at Ahjin Studios. All recommendations should be considered alongside creative vision and market intuition.

