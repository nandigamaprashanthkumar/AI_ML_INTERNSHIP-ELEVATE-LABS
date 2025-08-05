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

👤 Author
Nandigama Prashanth Kumar
AI & ML Internship – Task 2: Exploratory Data Analysis