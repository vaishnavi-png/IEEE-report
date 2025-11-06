# IEEE-report

n output graphs where indicated.

🧾 IEEE REPORT
Analysis of Factors Influencing Adult Income Levels

Author: Vaish
Institution: [Your College Name]
Course: Data Analytics / AI Lab Project
GitHub Repository: [Add your GitHub repo link here]

Abstract

This project analyzes the Adult Census Income Dataset to determine how demographic, educational, and occupational factors influence an individual's likelihood of earning more than $50,000 annually. The dataset was cleaned and analyzed using Python for preprocessing and Power BI for interactive visualization. Findings reveal that education level, occupation, and work hours are the most influential predictors of income level, while demographic attributes such as age and gender also play supporting roles. The integration of Python and Power BI provided a balanced approach for both statistical rigor and visual interpretability.

Keywords

Income Prediction, Data Visualization, Python, Power BI, Demographics, Education, Occupation, Machine Learning

I. INTRODUCTION

Income inequality and career advancement opportunities are influenced by several factors including education, work type, and personal demographics. Understanding these relationships helps identify patterns that contribute to higher earning potential.

The Adult Census Income Dataset from the UCI Machine Learning Repository contains over 48,000 records describing individuals’ demographics, education, and employment details, along with their income category (≤$50K or >$50K).

The primary objective of this study is to determine which personal and professional characteristics most strongly predict higher income levels. Python was used for data cleaning and exploration, while Power BI was used for visualization and dashboard development to uncover hidden relationships between attributes.

II. DATASET DESCRIPTION

The dataset includes the following attributes:

Category	Features
Demographic	age, sex, race, marital.status, native.country
Educational	education, education.num
Occupational	workclass, occupation, hours.per.week
Financial	capital.gain, capital.loss
Target	income (≤50K or >50K)

A total of 48,842 records were used for analysis after cleaning and preprocessing. The dataset is balanced enough for both visualization and predictive analytics.

III. METHODOLOGY
A. Data Cleaning and Preprocessing (Python)

The dataset contained missing and inconsistent values, represented as ‘?’. These were replaced with NaN and handled appropriately. Key cleaning steps included:

Removing duplicates and rows with missing occupation or workclass.

Stripping extra spaces from categorical values.

Creating derived columns:

income_flag: Encoded as 1 for >50K, 0 for ≤50K.

age_group: Created categorical bins (e.g., 18–25, 26–35, etc.).

capital_net: Difference between capital_gain and capital_loss.

The cleaned dataset was then exported as cleaned_adult_income.csv for visualization.

B. Exploratory Data Analysis (Python)

Python visualizations using Matplotlib and Seaborn were conducted to understand variable distributions.

Age Distribution: Displayed age frequencies and their relation to income.

Box Plot (Hours vs Income): Compared working hours between high- and low-income groups.

Correlation Heatmap: Revealed numeric relationships between variables and income.

The EDA confirmed that education_num, hours_per_week, and capital_gain have the strongest positive correlation with income.

C. Modeling Approach (Python)

A Logistic Regression model was implemented to test feature importance. Top contributing features included:

Education level (education_num)

Occupation type

Capital gain

Hours worked per week

The model achieved a precision score of 0.85 and AUC of 0.88, confirming high predictive strength of educational and occupational features.

D. Visualization and Insights (Power BI)

The cleaned dataset was visualized in Power BI to build an interactive dashboard that allows users to filter by demographics and instantly observe the impact on income.

1. Demographic Factors

Gender vs Income (100% Stacked Bar Chart): Showed males have a larger share of >50K earners.

Age Group vs Average Income (Column Chart): Displayed that individuals aged 30–50 have the highest proportion of high earners.

2. Educational Factors

Education vs High-Income Rate (Column Chart): Revealed a clear rise in earnings with education level.

Education Number vs Income (Line Chart): Demonstrated a linear correlation between academic qualification and income.

3. Occupational Factors

Occupation vs Income (Bar Chart): Highlighted managerial and professional roles as top-earning categories.

Workclass vs Income (Stacked Chart): Showed government and private sectors dominate high-income groups.

Hours Worked vs Income (Box Plot): Higher earners generally work longer hours on average.

4. Financial Factors

Capital Gain vs Loss (Scatter Plot): High-income individuals cluster in regions of higher capital gain.

Occupation × Education (Matrix Chart): Provided a combined view showing income differences across education and occupation types.

IV. RESULTS AND DISCUSSION
A. Key Insights

Education: Individuals with Bachelor’s and Master’s degrees are more likely to earn above $50K.

Occupation: Executive, managerial, and professional roles have the highest earning probabilities.

Work Hours: While higher earners tend to work more hours, occupation type matters more than time alone.

Age: Income peaks between 30–50 years, reflecting career progression.

Gender: Males have slightly higher income representation than females, indicating an ongoing wage gap.

B. Power BI Advantages

Power BI proved advantageous for:

Dynamic filtering (e.g., selecting gender, occupation, or country).

Interactivity, enabling user-driven insights.

Aesthetic dashboards that present complex data simply.

Comparative analysis using real-time chart interlinks, unlike static Python plots.

V. CONCLUSION

This project demonstrates that education level, occupation type, and work hours per week are the most significant predictors of adult income. Python provided analytical accuracy through preprocessing and correlation modeling, while Power BI added interpretive depth via dynamic visual dashboards.

Together, these tools bridge the gap between data science and decision-making, transforming raw census data into actionable insights about income patterns.

Future work could integrate geographic or industry-level factors to improve model accuracy and deepen socio-economic understanding.

VI. REFERENCES

[1] UCI Machine Learning Repository – Adult Census Income Dataset
[2] Kaggle – Adult Income Dataset for Analysis
[3] M. Waskom, “Seaborn: Statistical Data Visualization,” Journal of Open Source Software, 2021
[4] Microsoft Documentation – Power BI User Guide (2024)
[5] MAQ Software – Box and Whisker Chart for Power BI

AUTHOR INFORMATION

Name: Vaish
Institution: [Insert your college name]
Course: Data Analytics / AI Lab Project
Semester: [Insert semester here]
GitHub Repository: [Insert GitHub link]
