Overview
This project analyzes data from pregnant women in Wales to understand the factors that influence their intent to breastfeed. The analysis follows a full data science workflow—from data import and cleaning, through exploratory analysis, to predictive modeling and survival analysis. In addition to building a decision tree to predict breastfeeding intent, the project uses follow‐up data to perform survival analysis and Cox regression to investigate time‐to-event outcomes.

What the Project Does
Data Import & Cleaning:
The project starts by reading a CSV file containing demographic, clinical, and psychosocial data. Date variables are converted into proper formats and continuous variables (such as weight) are processed (for example, calculating BMI). Irrelevant columns are removed, and categorical variables are recoded to prepare the data for analysis. (​Assignment-A2---Annotat…)

Exploratory Data Analysis (EDA):
Summary statistics and tables are generated to examine data distributions, missing values, and variable recoding. Special attention is given to the breastfeeding intent variable to ensure it is properly configured for subsequent modeling. (​Assignment-A2---Annotat…)

Predictive Modeling:
A decision tree is built using the rpart package to predict whether a mother intends to breastfeed. The dataset is split into training (80%) and testing (20%) sets, and the tree is visualized with rpart.plot. Model performance is evaluated using a confusion matrix, providing metrics such as accuracy and sensitivity. (​Assignment-A2---Annotat…)

Survival Analysis & Cox Regression:
Using follow‐up data, the project also investigates time‐to-event outcomes with survival analysis. The follow‐up information (e.g., duration until an event like breastfeeding cessation or another clinical outcome) is analyzed using Kaplan–Meier survival curves and Cox proportional hazards regression. This Cox regression helps assess the impact of various predictor variables on the hazard rate, while the survival and survminer packages are used to fit the model and create visualizations. (​Assignment-A2---Annotat…)

Why This Analysis Was Done
Insight Generation:
The analysis seeks to identify key factors that influence a mother's decision to breastfeed and to understand how these factors affect outcomes over time.

End-to-End Demonstration:
The project demonstrates a complete and reproducible data analysis workflow—from cleaning raw data and performing EDA to predictive and survival modeling.

Practical Impact:
By revealing insights from both cross-sectional and follow-up data, the study may help inform future public health interventions in maternal and infant care.

Tools and Technologies
R & RStudio: For writing and executing the analysis.
Tidyverse: For data manipulation and visualization.
Lubridate: For date-time data processing.
rpart & rpart.plot: For decision tree modeling and visualization.
Caret: For evaluating model performance.
Survival & survminer: For conducting survival analysis and Cox regression.
Table1 & gtsummary: For creating descriptive tables.
Conclusion
This project provides a comprehensive analysis of factors influencing breastfeeding intent among pregnant women in Wales. It showcases robust data science practices, including data cleaning, exploratory analysis, predictive modeling, and survival analysis. The inclusion of follow-up data and Cox regression offers deeper insights into time-to-event outcomes, demonstrating the potential for informed public health strategies. The script is thoroughly annotated, making the methodology transparent and the project easy to follow for both academic audiences and potential employers.
