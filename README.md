Global Terrorism Database (GTD) Analysis & EDA
📌 Project Overview
This project performs a comprehensive Exploratory Data Analysis (EDA) on the Global Terrorism Database (GTD), which contains records of over 180,000 terrorist attacks worldwide from 1970 to 2017. The goal is to uncover global trends, identify high-risk regions, and analyze the methods used in these incidents.

The project demonstrates advanced data cleaning, feature engineering, and storytelling through data visualization.

📊 Key Features
Data Cleaning: Handled extensive missing values (NaN) in sensitive columns like casualties and locations.

Feature Engineering: * Created a Casualties metric (Killed + Wounded).

Engineered a Date timeline by resolving inconsistent year/month/day formats.

Categorized data into Decades for long-term trend analysis.

In-depth EDA: Visualized attack distributions by year, region, and weapon type using Seaborn and Matplotlib.

Insightful Conclusions: Derived logical connections between geopolitical events and the frequency of attacks.

🛠️ Technologies Used
Python (Core analysis)

Pandas (Data manipulation)

NumPy (Numerical operations)

Seaborn & Matplotlib (Advanced visualizations)

Google Colab / Jupyter Notebook

📁 Dataset Information
The dataset used in this project is the Global Terrorism Database (GTD), maintained by the National Consortium for the Study of Terrorism and Responses to Terrorism (START).

Dataset is available here: https://www.kaggle.com/datasets/START-UMD/gtd

📈 Key Findings
Temporal Trends: A significant surge in global terrorist activity was observed post-2010, peaking in 2014.

Regional Impact: The Middle East & North Africa (MENA) and South Asia remain the most affected regions.

Attack Methods: Explosives (Bombing) are the most frequent method of attack, accounting for over 50% of the recorded incidents.

🚀 How to Run
Clone the repository.

Download the dataset from the Kaggle link above.

Place the csv file in the project directory.

Open the .ipynb file in Google Colab or Jupyter Notebook and run the cells.
