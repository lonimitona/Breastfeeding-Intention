**Overview**

This project explores the factors influencing pregnant women's intention to breastfeed in Wales. This analysis allowed me to apply a full data science workflow—from data cleaning and exploratory analysis all the way through to predictive modeling and survival analysis.

**What I did**

- **Data Import & Cleaning:**
I started by importing a CSV file that included demographic, clinical, and psychosocial information from a cohort of pregnant women. I cleaned and preprocessed the dataset by converting date variables, calculating BMI from height and weight, removing irrelevant columns, and recoding categorical variables to prepare for analysis.

- **Exploratory Data Analysis (EDA):**
Next, I explored the data through summary statistics and tables. A big focus during this phase was on the breastfeeding intent variable, ensuring it was clean and well-defined for the predictive modeling step.

- **Predictive Modeling:**
ATo better understand what predicts breastfeeding intent, I built a decision tree using the rpart package. I split the data into training and testing sets (80/20), and then visualized the decision tree with rpart.plot. I evaluated the model using a confusion matrix, which gave insights into accuracy and sensitivity.

- **Survival Analysis & Cox Regression:**
I also had access to follow-up data that captured how long mothers continued breastfeeding. I used Kaplan-Meier survival curves and Cox proportional hazards regression to understand what factors might influence the duration of breastfeeding. The survival models helped me look beyond just intent—to actual behavioral outcomes over time.

**Why I Did This**

- **Insight Generation:**
I was curious about what factors—whether clinical, social, or psychological—influence a mother’s choice and ability to breastfeed. I wanted to go beyond simple correlations and uncover patterns that might help shape future public health programs or interventions.

More importantly, this project gave me the opportunity to walk through the full data lifecycle, from messy raw files to meaningful insights—something I deeply enjoy.

**Tools I Used**

- R & RStudio: My go-to tools for analysis and scripting
- Tidyverse: For data wrangling and visualization
- Lubridate: For handling messy date-time data
- rpart & rpart.plot: To build and visualize the decision tree
- Caret: For model evaluation
- Survival & survminer: For running and visualizing survival analysis
- Table1 & gtsummary: For creating descriptive tables.
  
**What I Learned**

One major takeaway was how predictive factors like BMI, maternal age, and employment status shaped the intention to breastfeed. But beyond that, survival analysis showed me something deeper: stress levels and lower socioeconomic status significantly increased the likelihood of early breastfeeding cessation. On the flip side, older age and a healthier BMI seemed to act as protective factors.

**So, Why Does This Matter?**

Public health efforts around maternal and infant care often focus on promotion, but tailored support is where impact really happens. Insights from this project could help identify mothers at higher risk of early breastfeeding drop-off, allowing healthcare professionals to offer personalized interventions that actually make a difference.
