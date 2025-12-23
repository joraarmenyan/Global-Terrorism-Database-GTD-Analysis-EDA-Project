# 🌍 Global Terrorism Database (GTD) Analysis & EDA

[![Python](https://img.shields.io/badge/Python-3.x-blue?style=flat&logo=python)](https://www.python.org/)
![Library](https://img.shields.io/badge/Library-Pandas%20%7C%20Seaborn-orange)
![Status](https://img.shields.io/badge/Status-Completed-success)
[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/ՔՈ_USERNAME/ՔՈ_REPO_ԱՆՈՒՆԸ/blob/main/ՔՈ_ՖԱՅԼԻ_ԱՆՈՒՆԸ.ipynb)

## 📌 Project Overview
This project focuses on the Exploratory Data Analysis (EDA) and Feature Engineering of the Global Terrorism Database (GTD). The dataset covers over 180,000 recorded incidents of terrorist attacks worldwide from 1970 to 2017.

The primary objective is to identify temporal and geographical patterns, analyze the lethality of different attack types, and clean complex data to derive meaningful analytical insights.

## 📂 Dataset
The dataset is sourced from the START Consortium and is available on Kaggle. It is highly complex, featuring over 100 attributes (qualitative and quantitative).

* Source: [Kaggle: Global Terrorism Database](https://www.kaggle.com/datasets/START-UMD/gtd)
* Key Features: Attack types, Weapon types, Casualty counts (Killed/Wounded), Geographical coordinates, Target types.

## 🛠️ Key Techniques Applied

### 1. Data Cleaning
To ensure the integrity of the analysis, the following cleaning steps were performed:
* Handling Missing Values:
    * Killed and Wounded: Significant gaps were imputed with 0 to ensure numerical analysis and summations remained intact without dropping valuable rows.
    * City and State: Textual gaps were filled with "Unknown" to maintain dataset completeness.
* Chronological Correction:
    * Addressed data inconsistencies where Month or Day contained invalid "0" values. These were replaced with "1" to allow for proper conversion to DateTime objects.

### 2. Feature Engineering
* Casualties Metric: Engineered a new feature Casualties by summing Killed and Wounded. This provides a more holistic view of an attack's impact than looking at fatalities alone.
* DateTime Creation: Merged separate Year, Month, and Day columns into a unified pandas datetime object for advanced time-series plotting.
* Decade Mapping: Created a Decade category to simplify long-term trend analysis and visualize shifts over 10-year periods.

### 3. Exploratory Data Analysis (EDA)
* Time-Series Analysis: Visualized the evolution of global terrorism, highlighting the sharp surge in incidents post-2010.
* Geographical Mapping: Used coordinate data to identify high-intensity zones, specifically highlighting hotspots in the Middle East, South Asia, and North Africa.
* Methodology Profiling: Analyzed correlations between *Attack Type* and *Weapon Type*.

## 📊 Key Findings
Based on the data analysis, the following conclusions were drawn:

1.  Peak Activity: 2014 was identified as the most active year globally, both in terms of the total number of attacks and total casualties.
2.  Lethality Trends: While "Bombing/Explosion" is the most frequent tactic, "Armed Assaults" often result in a higher casualty rate per individual incident.
3.  Geographical Shift: There has been a significant shift in terrorism hotspots over the decades: moving from Central/South America (in the 1980s) to the Middle East and Africa in the current decade.

## ⚙️ Technologies Used
* Language: Python
* Libraries: Pandas, NumPy, Matplotlib, Seaborn
* Environment: Google Colab / Jupyter Notebook

## 🚀 How to Run
1.  Clone this repository.
2.  Download the globalterrorismdb_0718dist.csv file from the [Kaggle link](https://www.kaggle.com/datasets/START-UMD/gtd).
3.  Install necessary libraries:
    bash
    pip install pandas numpy matplotlib seaborn
    
4.  Open the notebook (.ipynb) and run the cells sequentially.


