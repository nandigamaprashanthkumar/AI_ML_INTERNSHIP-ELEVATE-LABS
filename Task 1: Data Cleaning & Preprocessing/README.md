Titanic Data Cleaning & Preprocessing – Internship Task 1
Overview
This project is part of my AI & ML Internship (Task 1: Data Cleaning & Preprocessing), where I worked with the Titanic Dataset to demonstrate the essential steps required for preparing real-world data for machine learning.

The project focuses on:

✅ Handling missing values

✅ Encoding categorical features

✅ Normalizing numerical variables

✅ Visualizing and removing outliers

The ultimate goal is to produce a clean and structured dataset ready for further analysis or model training.

Workflow & Explanations
1. Importing Libraries & Dataset
Utilized Python libraries: Pandas, NumPy, Matplotlib, Seaborn, and Scikit-learn.

Loaded the Titanic dataset and performed an initial inspection of data shape, column types, and missing values.

2. Data Exploration
Explored dataset structure to understand features.

Identified missing values and columns needing special preprocessing.

3. Handling Missing Values
Numerical Features (e.g., Age): Filled missing values using the median to prevent skewness.

Categorical Features (e.g., Embarked): Filled missing values using the mode (most frequent value).

Columns with excessive missing values (e.g., Cabin): Created a missingness indicator and dropped the column for simplicity.

4. Encoding Categorical Variables
Converted categorical columns (e.g., Sex, Embarked) into numerical form using:

Label Encoding

One-Hot Encoding

5. Normalization & Standardization
Applied StandardScaler to numerical features (Age, Fare) so they have mean = 0 and standard deviation = 1.

This ensures better performance for ML models that are sensitive to feature scaling.

6. Outlier Detection & Removal
Visualized potential outliers using boxplots.

Applied the IQR (Interquartile Range) method to remove extreme outliers, ensuring robust model performance.

7. Exporting Clean Data
Saved the cleaned dataset for use in subsequent machine learning tasks.

How to Run the Project
1. Clone the Repository
bash
git clone https://github.com/nandigamaprashanthkumar/AI_ML_INTERNSHIP-ELEVATE-LABS
cd AI_ML_INTERNSHIP-ELEVATE-LABS
2. (Optional) Create a Virtual Environment
bash
python -m venv venv
On Windows:

bash
venv\Scripts\activate
On Mac/Linux:

bash
source venv/bin/activate
3. Install Dependencies
Install all required packages:

bash
pip install pandas numpy matplotlib seaborn scikit-learn
(If you already have most packages, just run:)

bash
pip install seaborn scikit-learn
4. Run the Notebook or Script
For Jupyter Notebook:
Open and execute cells step by step.

For Python Script:

bash
python your_file_name.py
Screenshots
📌 <img width="1089" height="496" alt="image" src="https://github.com/user-attachments/assets/fbed66c8-9e71-46ab-8c80-6105dd8dd4ea" />
<img width="959" height="670" alt="image" src="https://github.com/user-attachments/assets/61ab8a37-0459-49fc-9862-91f36eae41ff" />
<img width="540" height="806" alt="image" src="https://github.com/user-attachments/assets/0e319edb-2bc3-4d93-880b-b392f10d0871" />
<img width="712" height="598" alt="image" src="https://github.com/user-attachments/assets/6733573b-edef-4917-b5bd-e0b231e451af" />



Key Learnings
✔️ How to systematically clean and preprocess raw data for machine learning
✔️ The importance of handling missing values and outliers
✔️ Techniques to encode categorical features and standardize numerical values
✔️ Preparing data for modeling while avoiding common Python warnings/errors

Dataset
The project uses the Titanic Dataset, provided under the repository/assignment instructions.
Ensure the dataset file (Titanic-Dataset.csv) is placed in the same folder as your code for smooth execution.

Author
Nandigama Prashanth Kumar
AI & ML Internship – Task 1
