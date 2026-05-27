# Exploratory Data Analysis - Titanic, Train & IPL Datasets

## Overview
This repository contains comprehensive exploratory data analysis (EDA) of three datasets using Python data science libraries. The analyses systematically explore datasets, examining patterns, trends, and insights through data visualization and statistical analysis.

## Files
- **EDA-Titanic.ipynb** - Jupyter notebook containing complete analysis of the Titanic dataset
- **EDA-Train.ipynb** - Jupyter notebook containing complete analysis of the Train dataset
- **IPL_PROJECT.ipynb** - Jupyter notebook containing complete analysis of IPL 2022 Season dataset

## Libraries Used
- **pandas** (v2.3.3) - Data manipulation and analysis
- **numpy** (v2.3.5) - Numerical computing
- **matplotlib** (v3.10.6) - Data visualization
- **seaborn** (v0.13.2) - Statistical data visualization

---

# EDA - Titanic Dataset

## Dataset Information
The Titanic dataset contains **891 passenger records** with **15 columns** including:

### Columns:
- **survived** - Target variable (0 = Did not survive, 1 = Survived)
- **pclass** - Passenger class (1st, 2nd, 3rd)
- **sex** - Gender of passenger
- **age** - Age of passenger
- **sibsp** - Number of siblings/spouses aboard
- **parch** - Number of parents/children aboard
- **fare** - Ticket fare
- **embarked** - Port of embarkation (C = Cherbourg, Q = Queenstown, S = Southampton)
- **class** - Passenger class category
- **who** - Classification (man, woman, child)
- **adult_male** - Whether passenger is an adult male
- **deck** - Deck location
- **embark_town** - Town of embarkation
- **alive** - Survival status (yes/no)
- **alone** - Whether passenger was traveling alone

## Key Findings

### Survival Rates by Passenger Class
| Class | Survival Rate |
|-------|---------------|
| First Class | 62.96% |
| Second Class | 47.28% |
| Third Class | 24.24% |

**Insight**: Higher passenger class significantly increased chances of survival.

### Survival Rates by Gender
| Gender | Survival Rate |
|--------|---------------|
| Female | 74.20% |
| Male | 18.89% |

**Insight**: Females had substantially higher survival rates, following the "women and children first" evacuation protocol.

### Overall Statistics
- **Total Passengers**: 891
- **Survivors**: 342 (38.38%)
- **Non-survivors**: 549 (61.62%)
- **Missing Values**:
  - Age: 177 missing values
  - Deck: 688 missing values
  - Embarked: 2 missing values

## Analysis Sections Covered
1. Data loading and library imports
2. Dataset overview (head, tail, info, describe)
3. Data types and structure examination
4. Univariate analysis (value counts by class and gender)
5. Survival rate calculations
6. Data aggregation and groupby operations
7. Statistical summaries

---

# EDA - Train Dataset

## Dataset Information
The Train dataset contains comprehensive train passenger records with multiple features for analysis.

### Key Features:
- Passenger demographics (age, gender, class)
- Journey details (departure, arrival, destination)
- Ticket information (fare, class, seat)
- Additional metadata for comprehensive analysis

## Analysis Sections Covered
1. Data loading and library imports
2. Dataset overview (head, tail, info, describe)
3. Data types and structure examination
4. Univariate analysis (value counts and distributions)
5. Feature relationships and correlations
6. Data aggregation and groupby operations
7. Statistical summaries and insights
8. Visualization of key patterns and trends

## Key Analysis Areas
- Passenger demographics distribution
- Journey patterns and trends
- Feature correlations and relationships
- Missing data analysis
- Univariate and multivariate insights

---

# EDA - IPL 2022 Dataset

## Dataset Information
The IPL (Indian Premier League) 2022 Season dataset contains **74 match records** with **20 columns** including comprehensive match-by-match statistics.

### Dataset Structure
- **Rows**: 74 matches
- **Columns**: 20 detailed features
- **Missing Values**: None (clean dataset)

### Key Columns

#### Match Details
- **match_id** - Unique match identifier (1-74)
- **date** - Match date (March 26, 2022 to May 29, 2022)
- **venue** - Stadium/venue name where match was played
- **stage** - Match stage (Group, Playoff, Final)

#### Team Information
- **team1** - First team name
- **team2** - Second team name
- **toss_winner** - Team that won the coin toss
- **toss_decision** - Toss decision (Bat or Field)

#### Scoring Statistics
- **first_ings_score** - First innings total score
- **first_ings_wkts** - First innings wickets lost
- **second_ings_score** - Second innings total score
- **second_ings_wkts** - Second innings wickets lost
- **highscore** - Highest individual score in match

#### Match Outcome
- **match_winner** - Winning team name
- **won_by** - Victory type (Wickets or Runs)
- **margin** - Victory margin (runs or wickets)

#### Player Awards
- **player_of_the_match** - Best performing player
- **top_scorer** - Highest scorer of the match
- **best_bowling** - Bowler with best figures
- **best_bowling_figure** - Best bowling statistics (format: wickets--runs)

## Key Statistics

### Scoring Overview
| Metric | Value |
|--------|-------|
| Avg First Innings Score | 171.12 runs |
| Avg Second Innings Score | 158.54 runs |
| Highest Individual Score | 140 runs |
| Lowest Individual Score | 28 runs |
| Avg Match Margin | 16.97 |

### Performance Metrics
- **Avg Wickets Lost (1st Inn)**: 6.14 wickets
- **Avg Wickets Lost (2nd Inn)**: 6.18 wickets
- **Highest Match Margin**: 91 runs
- **Lowest Match Margin**: 2 runs/wickets

## Analysis Sections Covered
1. Dataset loading and exploration
2. Data shape, structure, and info
3. Missing value analysis
4. Descriptive statistics
5. Team performance analysis
   - Most matches won by each team
   - Home vs Away performance
   - Stage-wise match distribution
6. Toss analysis
   - Toss decision trends (Bat vs Field)
   - Toss winner correlation with match results
7. Scoring analysis
   - First vs Second innings comparison
   - Win margin distribution
   - Venue impact on scoring
8. Player performance analysis
   - Most Player of the Match awards
   - Top scorers analysis
   - Best bowlers
9. Visualizations
   - Bar charts for team wins
   - Distribution plots for scores
   - Venue-wise statistics
   - Stage-wise analysis

## Key Insights Extracted
- Dominant teams in the tournament
- Impact of toss decision on match outcomes
- Scoring patterns and trends across venues
- Player consistency and performance
- Stage-wise performance variation (Group vs Playoff vs Final)
- Win margin distribution across different scenarios

## Teams Analyzed
Chennai, Kolkata, Delhi, Mumbai, Bangalore, Punjab, Gujarat, Lucknow, Hyderabad, Rajasthan

## Tournaments Covered
- **Tournament**: IPL 2022
- **Total Matches**: 74
- **Format**: 20-20 Cricket
- **Period**: March 26, 2022 - May 29, 2022

---

## How to Use
1. Clone the repository
   ```bash
   git clone https://github.com/chaitanya-m-dot/Exploratory-Data-Analysis.git
   ```

2. Install required libraries
   ```bash
   pip install pandas numpy matplotlib seaborn
   ```

3. Open Jupyter Notebook
   ```bash
   jupyter notebook
   ```

4. Navigate to desired notebook:
   - `EDA-Titanic.ipynb` - For Titanic dataset analysis
   - `EDA-Train.ipynb` - For Train dataset analysis
   - `IPL_PROJECT.ipynb` - For IPL 2022 analysis

5. Run all cells to view the analysis and visualizations

## Requirements
- Python 3.7+
- Jupyter Notebook
- pandas
- numpy
- matplotlib
- seaborn

## Dataset Sources
- **Titanic**: Classic dataset containing passenger information
- **Train**: Train passenger records dataset
- **IPL 2022**: Indian Premier League 2022 season match data

## License
This project is open source and available for educational purposes.

## Author
Chaitanya M. (@chaitanya-m-dot)

## Contact & Contributions
Feel free to fork, contribute, or raise issues for improvements to the analysis.
