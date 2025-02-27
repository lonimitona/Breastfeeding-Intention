**Overview**

This project analyzes data from pregnant women in Wales to understand the factors that influence their intent to breastfeed. The analysis follows a full data science workflow—from data import and cleaning, through exploratory analysis, to predictive modeling and survival analysis. In addition to building a decision tree to predict breastfeeding intent, the project utilizes follow‐up data to perform survival analysis and Cox regression to investigate time‐to-event outcomes.

**What the Project Does**

- **Data Import & Cleaning:**
The project starts by reading a CSV file containing demographic, clinical, and psychosocial data. Date variables are converted into proper formats and continuous variables, such as weight and height are processed (for example, calculating BMI). Irrelevant columns are removed, and categorical variables are recoded to prepare the data for analysis. 

- **Exploratory Data Analysis (EDA):**
Summary statistics and tables are generated to examine data distributions, missing values, and variable recoding. Special attention is given to the breastfeeding intent variable to ensure it is properly configured for subsequent modeling.

- **Predictive Modeling:**
A decision tree is built using the rpart package to predict whether a mother intends to breastfeed. The dataset is split into training (80%) and testing (20%) sets, and the tree is visualized with rpart.plot. Model performance is evaluated using a confusion matrix, providing metrics such as accuracy and sensitivity.

- **Survival Analysis & Cox Regression:**
Using follow‐up data, the project also investigates time‐to-event outcomes with survival analysis. The follow‐up information (e.g., duration until an event like breastfeeding cessation) is analyzed using Kaplan–Meier survival curves and Cox proportional hazards regression. This Cox regression helps assess the impact of various predictor variables (e.g. full time employment) on the hazard rate, while the survival and survminer packages are used to fit the model and create visualizations.

**Why This Analysis Was Done**

- **Insight Generation:**
The analysis seeks to identify key factors that influence a mother's decision to breastfeed and to understand how these factors affect outcomes over time.

- **End-to-End Demonstration:**
The project demonstrates a complete and reproducible data analysis workflow—from cleaning raw data and performing EDA to predictive and survival modeling.

- **Practical Impact:**
By revealing insights from both cross-sectional and follow-up data, the study may help inform future public health interventions in maternal and infant care.

**Tools and Technologies**

- R & RStudio: For writing and executing the analysis.
- Tidyverse: For data manipulation and visualization.
- Lubridate: For date-time data processing.
- rpart & rpart.plot: For decision tree modeling and visualization.
- Caret: For evaluating model performance.
- Survival & survminer: For conducting survival analysis and Cox regression.
- Table1 & gtsummary: For creating descriptive tables.
  
**Conclusion**

The analysis revealed that certain factors strongly influence both the intent to breastfeed and the timing of subsequent events. The decision tree model established that variables such as BMI, maternal age, and key demographic features significantly impact a mother's breastfeeding intent. 

Also, the survival analysis provided deeper insights: Cox regression results demonstrated that higher stress levels and lower socioeconomic status were associated with an increased hazard rate, meaning these factors tend to shorten the time until events (such as breastfeeding cessation or other adverse outcomes) occur. On the contrary, higher maternal age and a healthier BMI profile were linked to longer durations before such events, suggesting a protective effect.

These findings offer actionable insights for healthcare professionals and public health policymakers. By identifying mothers who are at greater risk for early adverse outcomes, tailored support programs and interventions can be developed to promote sustained breastfeeding and improve maternal and infant health outcomes.

