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
   
- Inspecting the Data
- Data Transformation (Standardizing Scores for Clustering)
- Outlier Identification (used boxplots for each numeric column helps in identifying potential outliers)

#### 4. Key Findings
      
- Students who completed the test preparation course have higher average scores across all subjects compared to those who didn’t.
- Females tend to perform better in reading and writing scores, whereas males perform better in math.
- Students with standard lunch (proxy for higher socioeconomic status) perform significantly better across all subjects than those with free/reduced lunch (proxy for lower socioeconomic status).
- High Performers tend to have parents with higher educational backgrounds (e.g., associate's degree), are more likely to have taken the test preparation course, and tend to have standard lunch.
- Low Performers are more likely to have parents with lower education (e.g., high school), tend to have free/reduced lunch, and more often did not take the test preparation course.

*High Performers Top Characteristics:*

- Gender: More likely to be female.
- Race: More students from group D.
- Lunch: Most have standard lunch.
- Test Prep: More likely to have completed the test preparation course.

*Low Performers Top Characteristics:*

- Gender: More likely to be male.
- Race: More students from group C.
- Lunch: Most have free/reduced lunch.
- Test Prep: More likely to not have completed the test preparation course.

#### 5. Future Work

- Exploratory Data Analysis (EDA): Plot distributions of scores. Examine relationships between different features.
- Feature Engineering: Create new features, if necessary. Encode categorical variables.
- Modeling: Train machine learning models on the cleaned data. Evaluate model performance.

#### 6.  Source

https://www.kaggle.com/datasets/adepvenugopal/students-performance
