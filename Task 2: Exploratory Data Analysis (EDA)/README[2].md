Titanic Dataset – Exploratory Data Analysis (EDA)
📌 Overview
This project is part of my AI & ML Internship (Task 2: Exploratory Data Analysis), where I performed a detailed EDA on the Titanic dataset.
The objective was to explore the data using statistics and visualizations to uncover patterns, trends, anomalies, and relationships between features that influence survival.

🎯 Objectives
✅ Understand data distributions and compute summary statistics

✅ Visualize relationships between key features

✅ Detect patterns, trends, and anomalies in the dataset

✅ Make basic feature-level inferences to guide further machine learning tasks

🔍 Workflow
1. Summary Statistics
Used Pandas to generate summary statistics (mean, median, standard deviation, percentiles) for numerical features.

Reviewed counts, unique values, and frequency distributions for categorical variables.

2. Visualizations
Histograms & Boxplots: Analyzed distributions and detected outliers for features like Age and Fare.

Bar Plots: Compared survival rates across categorical variables such as Sex and Pclass.

Correlation Matrix (Heatmap): Identified relationships between numerical features.

Pair Plots: Explored multivariate relationships, e.g., how Age and Fare relate to survival.

3. Pattern & Anomaly Detection
Detected outliers using boxplots and statistical methods.

Uncovered correlations between features using a heatmap.

Observed patterns such as:

Higher survival rates among females

Better survival chances for first-class passengers

4. Feature-Level Inferences
Most passengers were adults aged 20–40.

Survivors tended to pay higher fares and were often from upper classes.

Certain categorical features (e.g., Embarked, SibSp) showed significant relationships with survival.

💻 Example Code Snippets
python
Copy
Edit
# ✅ Summary Statistics
print(df.describe())
print(df.describe(include=['object']))

# ✅ Histogram - Age Distribution
import matplotlib.pyplot as plt
import seaborn as sns
plt.figure(figsize=(6,4))
sns.histplot(df['Age'], bins=30, kde=True)
plt.title('Age Distribution')
plt.show()

# ✅ Correlation Matrix - Heatmap
corr = df.select_dtypes(include=['number']).corr()
plt.figure(figsize=(8,6))
sns.heatmap(corr, annot=True, cmap='coolwarm')
plt.title('Correlation Matrix')
plt.show()
⚙️ Installation
Make sure the required Python packages are installed before running the analysis:

bash
Copy
Edit
pip install pandas numpy matplotlib seaborn scikit-learn plotly
(For Jupyter Notebook, you can prefix with !pip install ...)

🚀 How to Use
Clone this repository and place the Titanic dataset (Titanic-Dataset.csv) in the project folder.

Open the EDA Jupyter Notebook or Python script.

Run the code cells step by step to generate insights and visualizations.

Explore the patterns and observations from the analysis.

📊 Insights & Learning
Gained hands-on experience in statistical analysis and data visualization.

Identified strong patterns, e.g., gender and passenger class significantly impact survival.

Strengthened understanding of EDA techniques to prepare data for machine learning tasks.

🖼️ Screenshots
📌

<img width="830" height="573" alt="image" src="https://github.com/user-attachments/assets/e42cd210-4b92-44d1-b9af-0d21968ebbbf" />
<img width="790" height="591" alt="image" src="https://github.com/user-attachments/assets/1469427d-0518-4301-b5e0-4d458b74292e" />
<img width="728" height="807" alt="image" src="https://github.com/user-attachments/assets/a53444f3-3c47-430f-bdc6-02fa11712e69" />
<img width="816" height="807" alt="image" src="https://github.com/user-attachments/assets/fbfe791b-8c92-4452-9aa5-9bcfd9d456a2" />
<img width="836" height="799" alt="image" src="https://github.com/user-attachments/assets/e5fba49b-5b3c-491d-9080-1315642a5d14" />
<img width="853" height="799" alt="image" src="https://github.com/user-attachments/assets/7827a12a-517b-406c-a13b-4afe8f680e17" />
<img width="875" height="801" alt="image" src="https://github.com/user-attachments/assets/e5fbd732-8729-4203-820b-05ad36e2c12b" />
<img width="555" height="798" alt="image" src="https://github.com/user-attachments/assets/eabbfc17-b386-423d-808d-ce44f9915b87" />
<img width="581" height="483" alt="image" src="https://github.com/user-attachments/assets/856f17d3-d6d7-4e94-bc43-6de131879b8f" />
<img width="624" height="483" alt="image" src="https://github.com/user-attachments/assets/337df54c-7770-4fde-aeb7-b2efa017015c" />
<img width="544" height="419" alt="image" src="https://github.com/user-attachments/assets/25e63dd1-d596-4e56-b658-d0ce2974f4b4" />



👤 Author
Nandigama Prashanth Kumar
AI & ML Internship – Task 2: Exploratory Data Analysis
