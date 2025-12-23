Global Terrorism Database (GTD) Analysis & EDA
Project Description
This project focuses on the Exploratory Data Analysis (EDA) and Feature Engineering of the Global Terrorism Database. The dataset contains detailed information on terrorist attacks worldwide from 1970 to 2017, including over 180,000 recorded incidents. The objective is to identify temporal and geographical patterns, understand the impact of different attack types, and clean the complex data for meaningful analytical insights.

Dataset
The dataset is highly complex, featuring over 100 attributes including qualitative and quantitative features such as attack types, weapon types, casualty counts, and precise geographical coordinates.

Dataset is available here: https://www.kaggle.com/datasets/START-UMD/gtd

Key Steps Performed:
1. Data Cleaning
Handling Missing Values: Addressed significant gaps in Killed and Wounded columns by imputing them with 0, ensuring numerical analysis remains intact.

Text Imputation: Cleaned geographical features like City and State by filling missing values with "Unknown" to maintain dataset integrity.

Chronological Correction: Replaced invalid "0" values in Month and Day columns with "1" to allow for proper time-series conversion.

2. Feature Engineering
Casualties Metric: Engineered a new feature Casualties by summing Killed and Wounded to provide a holistic view of an attack's impact.

DateTime Object: Created a unified Date column using pd.to_datetime for advanced temporal plotting.

Decade Mapping: Categorized years into Decades to simplify long-term global trend analysis.

3. Exploratory Data Analysis (EDA)
Time-Series Analysis: Visualized the evolution of global terrorism, highlighting the sharp surge in incidents post-2010.

Geographical Mapping: Identified high-intensity zones, specifically in the Middle East, South Asia, and North Africa.

Methodology Profiling: Analyzed the correlation between Attack Type and Weapon Type, discovering that "Bombing/Explosion" is the most frequent tactic used.

Key Findings
Peak Activity: 2014 was identified as the most active year in terms of both the total number of attacks and casualties globally.

Lethality Trends: While bombings are the most common, armed assaults often result in a higher casualty rate per individual incident.

Hotspot Shifts: The analysis reveals a significant geographical shift in terrorism activity from Central/South America (1980s) to the Middle East and Africa in the current decade.

Technologies Used
Language: Python

Libraries: Pandas, NumPy, Matplotlib, Seaborn

Environment: Google Colab / Jupyter Notebook

How to Run
Clone this repository to your local machine or open it in Google Colab.

Download the globalterrorismdb_0718dist.csv from the Kaggle link provided.

Ensure all Python libraries listed in the Technologies section are installed.

Run the notebook cells sequentially to reproduce the analysis and visualizations.
