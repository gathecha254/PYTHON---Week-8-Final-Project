## 🌍 COVID-19 Global Data Tracker
This project analyzes global trends of the COVID-19 pandemic using real-world data from Our World in Data via the owid-covid-data.csv dataset. It explores confirmed cases, deaths, vaccination progress, and socio-economic indicators across countries over time.

The goal is to:

- Import and clean case, death, and vaccination data
- Analyze time-based trends
- Compare metrics across selected countries
- Visualize findings with charts and maps
- Communicate insights clearly through narrative explanations

🎯 Project Objectives

- Import and Clean Data
- Load the OWID dataset and handle missing values appropriately.
- Analyze Time Trends
- Explore how cases and deaths evolved globally and per country.
- Compare Metrics Across Countries
- Highlight differences in infection rates, death rates, and vaccine coverage.
- Visualize Trends
- Use line charts, bar plots, choropleth maps, and correlation matrices.
- Generate Insights
- Document key observations derived from visualizations and analysis.
- Present Findings
- Combine code, visuals, and narrative in a well-documented notebook.

🛠️ Tools & Libraries Used

- Python: Core language
- Pandas: Data manipulation and cleaning
- NumPy: Mathematical operations
- Matplotlib / Seaborn: Static visualization (line charts, bar charts, pie charts)
- Plotly Express: Interactive visualization (choropleth map)
- Jupyter Notebook / Google Colab: Interactive analysis environment

 How to Run the Project

Option 1: Using Google Colab (Recommended)
- Open Google Colab
- Create a new notebook or upload an existing .ipynb file
- Upload the owid-covid-data.csv file
- Run each cell sequentially
- View visualizations directly in the notebook

🔗 Direct link to dataset: https://www.kaggle.com/datasets/sk1812/owidcoviddata

Option 2: Locally with Jupyter Notebook
- Clone this repository:
git clone https://github.com/yourusername/covid-tracker.git

- Install required libraries:
pip install pandas numpy matplotlib seaborn plotly jupyter

- Launch Jupyter Notebook:
jupyter notebook

- Open the covid_analysis.ipynb file
Run all cells to view charts and insights


🧠 Key Insights

1. Global Case Growth Was Exponential
- Early 2020 saw rapid increases in confirmed cases worldwide.
- The growth slowed after 2021 due to vaccines and public health measures.
2. Death Rates Vary Significantly Between Countries
- Yemen, Italy, and Peru had some of the highest average death rates during the initial wave.
- Germany and South Korea maintained relatively low death rates despite high case counts.
3. Vaccination Progress Was Uneven
- High-income countries like Israel and the USA achieved high vaccination coverage early.
- Many African and developing nations lagged behind due to limited supply and distribution challenges.
4. Population Size Correlates with Total Cases and Deaths
- Larger populations tend to report more infections and fatalities.
- This reflects broader exposure risk rather than higher vulnerability.
5. Wealth Alone Did Not Protect Against Infections
- GDP per capita showed little correlation with total cases or deaths.
- Other factors such as testing, policy response, and timing of interventions played bigger roles.
6. Vaccinations Helped Reduce Case Growth
- A slight negative correlation between vaccination rate and case count suggests that vaccines helped curb spread.
- However, the effect was not very strong, possibly due to variant emergence or delayed rollout.
7. Correlation ≠ Causation
- While GDP per capita correlates with life expectancy, it does not strongly predict health outcomes during the pandemic.
- Economic indicators should be interpreted alongside healthcare policies and social factors.
  
⚠️ Limitations and Challenges

1. Missing Data Affected Analysis
- Some small countries (e.g., Saint Vincent and the Grenadines) have incomplete historical records.
- Vaccination data is sparse before 2021; results reflect later rollouts.
- ICU usage, hospitalization, and detailed demographic data are only available for certain regions.
2. Pie Charts Were Not Suitable for Country Comparisons
- Pie charts became cluttered and hard to interpret when many countries were included.
- They were replaced with bar charts and line graphs , which better highlight differences.
3. Temporal Aggregation Masks Short-Term Trends
- The dataset aggregates data over time, making it difficult to track the impact of short-term events like lockdowns or variants.
4. Country-Level Variability
- Different reporting practices affected accuracy and consistency across countries.
- Some entries may contain duplicate or inconsistent values and were handled during grouping/summing.
5. Visualization Limitations
- Certain visualizations (like choropleth maps) can be misleading if not normalized by population.
Pie charts are good for proportions but poor for comparative analysis.

# Repository Structure
1. covid-tracker/
2. ├── owid-covid-data.csv        # Source dataset
3. ├── covid_analysis.ipynb       # Main Jupyter Notebook
4. ├── README.md                  # This file
5. └── images/                    # Optional: Screenshots or exported visuals

This project reinforced the importance of:
* Data transparency : Many countries had inconsistent reporting practices.
* Responsible data handling : Missing values must be acknowledged and documented.
* Visual storytelling : Charts help communicate complex trends effectively.
*Reproducibility : A well-documented notebook makes it easy for others to understand and build upon the analysis.

# Future Improvements (Stretch Goals)
* Convert the notebook into a Django web app for interactive dashboards.
* Add user input forms to select country/date ranges dynamically.
* Use Streamlit/Dash for interactive visualization.
* Export reports automatically as PDF or HTML.
* Normalize data per million people for fairer comparisons.
* Build animated charts to show change over time.
