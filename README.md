# AIML_Task-1
Titanic dataset

The goal of this task is to take the raw Titanic Dataset and transform it into a clean, structured format suitable for Machine Learning models. This involves handling missing data, encoding categorical variables, and ensuring all numerical features are on a similar scale.

 Tasks Performed
 1. Exploratory Data Analysis (EDA)Identified missing values across the dataset.Visualized feature distributions and identified outliers using Boxplots.Dropped columns like Cabin that had more than 70% missing data and Name/Ticket which don't provide direct predictive power for a baseline model.
 2. Handling Missing ValuesAge: Filled missing values with the Median. Median was chosen over mean because it is more robust to the age outliers in the dataset.Embarked: Filled missing values with the Mode (the most frequent port of entry).
 3. Feature EncodingMachine Learning models require numerical input. I converted:Sex: Mapped male to 0 and female to 1.Embarked: Used One-Hot Encoding to create dummy variables for the different ports (C, Q, S).
 4. Outlier RemovalUsing the Interquartile Range (IQR) method, I filtered out extreme values in the Fare and Age columns. This prevents the model from being biased by "noise" or rare extreme cases.
 5. Feature ScalingSince Age and Fare have vastly different ranges, I applied Standardization

 Technologies Used - 
-> PythonPandas (Data manipulation)
-> NumPy (Mathematical operations)
-> Scikit-Learn (Preprocessing & Scaling)
-> Seaborn/Matplotlib (Data visualization)
