COVID-19 Data Analysis (India)
🧱 Project Goal

Use real-world COVID-19 data to practice data cleaning and basic analysis with NumPy and Pandas.
Focus on India, preparing the dataset for future visualization and insights.

Day 1 Progress
Data Loading & Inspection

Imported libraries: pandas, numpy

Loaded dataset: df = pd.read_csv("data/owid-covid-data.csv")

Checked first rows and structure: df.head(), df.info(), df.shape

Set Pandas option to display all columns: pd.set_option('display.max_columns', None)

3️⃣ Data Filtering & Cleaning

Filtered data for India only: india_df = df[df['location'] == 'India'].copy()

Converted date column to datetime: india_df['date'] = pd.to_datetime(india_df['date'])

Verified column types and basic structure

4️⃣ Git Commit – Day 1

Stage files: git add notebooks/covid_analysis.ipynb and git add README.md

Commit: git commit -m "Day 1: Loaded dataset, filtered for India, converted date column, added README"

Rename branch if needed: git branch -M main

Push to GitHub: git push -u origin main
