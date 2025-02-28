# Anime Rating Analysis

![Data Analysis](https://img.shields.io/badge/Data-Analysis-green)
![Machine Learning](https://img.shields.io/badge/Machine-Learning-blue)
![Python](https://img.shields.io/badge/Python-3.9-yellow)
![Status](https://img.shields.io/badge/Status-Completed-success)

## 📊 Project Overview

This project analyzes a comprehensive anime dataset to understand various factors affecting anime ratings and to build a predictive model. The analysis explores correlations between anime ratings and various features such as type, number of episodes, studio, release year, content warnings, and more.

## 🔍 Dataset Description

The dataset (`anime.csv`) contains over 15,000 anime entries with the following attributes:

- **Rating**: Average user rating (0.96-4.6)
- **Type**: Format of the anime (TV, Movie, OVA, Web, etc.)
- **Episodes**: Number of episodes
- **Studio**: Animation studio that produced the anime
- **Release_season**: Season when the anime was released (Fall, Spring, Summer, Winter)
- **Tags**: Categories and genres associated with the anime
- **Release_year**: Year when the anime was released (1907-2022)
- **Content_Warning**: Content warnings associated with the anime
- **staff**: People involved in the production (directors, writers, etc.)

## 🛠️ Installation & Setup

### Prerequisites
- Python 3.9 or higher
- Jupyter Notebook/Lab or Google Colab

### Required Libraries
```bash
pip install pandas
pip install numpy
pip install matplotlib
pip install seaborn
pip install scikit-learn
pip install catboost
pip install shap
```

### How to Run
1. Clone the repository:
   ```bash
   git clone https://github.com/mviswa12/anime-rating-analysis.git
   cd anime-rating-analysis
   ```

2. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:
   ```bash
   jupyter notebook Anime_Rating_Analysis.ipynb
   ```

## 📈 Analysis Performed

### Data Preprocessing
- Checked for and removed duplicate values (87 duplicates found)
- Handled missing values across various columns
- Converted categorical features to appropriate formats
- Created flag columns to track missing data patterns
- Implemented rare label encoding for categorical variables with low frequencies

### Exploratory Data Analysis (EDA)
1. **Distribution Analysis**
   - Rating distribution across different anime types
   - Episode count distribution
   - Release year timeline
   - Content warning distribution

2. **Bar Plots**
   - Average episodes by anime type
   - Top 10 studios by number of productions
   - Rating trends by release year

3. **Trend Analysis**
   - Evolution of top 5 tags over years
   - Content warnings prevalence by year
   - Average rating changes over time

4. **Correlation Analysis**
   - Relationship between episodes and ratings
   - Impact of studios on ratings
   - Influence of content warnings on ratings

### Predictive Modeling
- Built a CatBoost regression model to predict anime ratings
- Applied tree-based model to handle mixed data types effectively
- Used categorical feature processing for optimal performance
- Performed model evaluation with RMSE and R² metrics
- Implemented SHAP (SHapley Additive exPlanations) for model interpretation

## 🔑 Key Findings

1. **Rating Trends**:
   - Average anime ratings have shown an upward trend from 1907 to 2022
   - Modern anime (post-2010) generally receives higher ratings
   - Notable improvement in average ratings during the 2010s and 2020s

2. **Influential Factors**:
   - Studio is the most important predictor of anime ratings (26.9% importance)
   - Release year significantly impacts ratings (23.2% importance)
   - Type of anime and episode count are also strong predictors

3. **Content Analysis**:
   - Certain content warnings correlate with rating patterns
   - The presence of explicit content shows varied impact on ratings
   - Genre trends show evolution over decades of anime production

4. **Model Performance**:
   - The CatBoost model achieved a test RMSE of 0.31 (on a scale of 0.96-4.6)
   - 21.3% improvement over baseline predictions
   - Model explains approximately 38% of the variance in ratings (R² of 0.38)

## 📊 Visualizations

The project includes multiple visualization types:
- Distribution plots of anime ratings
- Episode count histograms
- Studio production bar charts
- Tags and genre trends over time
- Content warning prevalence charts
- Feature importance plots
- SHAP value analysis plots

## 🔄 Future Work

1. Include temporal analysis to track rating trends by season and month
2. Build recommendation systems based on the identified patterns
3. Incorporate viewer demographic data to analyze preference patterns
4. Create interactive dashboards for exploring the anime dataset
5. Develop neural network models for improved predictive performance
6. Analyze the impact of specific staff members (directors, writers) on ratings

## 🔗 References

- Anime Industry Database
- MyAnimeList Data Standards
- Animation Production Analysis Framework

## 👤 Author

- Mega Viswanathan

## 📄 License

This project is licensed under the MIT License - see the LICENSE file for details.

---

For questions or feedback, please open an issue or contact me at [megavishy@gmail.com](megavishy@gmail.com).
