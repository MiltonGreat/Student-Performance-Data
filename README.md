# Student-Performance-Data

### Summary and Recommendations

#### 1. Overview

This project demonstrates data cleaning techniques using Python (Pandas and NumPy) to process a dataset of students' performance on standardized tests. The goal is to prepare the data for analysis by handling missing values, smoothing noisy data, and removing outliers.

#### 2. Data

The dataset used in this project contains information on students, such as:

- gender: Gender of the student.
- race_ethnicity: Group identifier for race/ethnicity.
- parental_level_of_education: Highest education level of the parents.
- lunch: Type of lunch the student receives (standard or free/reduced).
- test_preparation_course: Whether the student completed a test preparation course.
- math_score, reading_score, writing_score: Scores in respective subjects.

#### 3. Data Cleaning Process
   
- Handling Missing Values: Numerical Columns: Missing values in numerical columns (scores) were filled with the median.
- Handling Missing Values: Categorical Columns: Missing values in categorical columns (like gender and lunch) were filled with the most frequent value (mode).
- Smoothing Noisy Data: To reduce noise in the scores, a rolling mean (window size of 3) was applied to the math_score, reading_score, and writing_score columns.
- Removing Outliers: Outliers were identified and removed using the Interquartile Range (IQR) method for numeric columns. This helped remove extreme values that could distort the analysis.

#### 4. Key Findings
      
The final cleaned dataset contains 978 entries and is ready for further analysis. Descriptive statistics after cleaning:

- Math Score: Mean = 66.49, Std = 8.06
- Reading Score: Mean = 69.55, Std = 7.93
- Writing Score: Mean = 68.46, Std = 8.25

#### 5. Future Work

- Exploratory Data Analysis (EDA): Plot distributions of scores. Examine relationships between different features.
- Feature Engineering: Create new features, if necessary. Encode categorical variables.
- Modeling: Train machine learning models on the cleaned data. Evaluate model performance.

#### 6.  Source

https://www.kaggle.com/datasets/adepvenugopal/students-performance
