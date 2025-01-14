# ✅ PROJECT-08

In today's business world, data analysis plays a key role in making strategic decisions. To solve a specific business problem, this project proposes the union of two powerful data analysis tools: the SQL language and the R language. These tools will be used together to address an important issue related to expenses with hospitalization of patients. Through the "sqldf" package, we will use the SQL language to carry out an exploratory analysis of the data. Data used in this project were obtained from a national survey of hospital costs conducted by the US Agency for Healthcare. These data consist of hospital records of samples of patients hospitalized in the city of Wisconsin, being restricted to the age group of 0 to 17 years. The first step will be to explore the data using the SQL language, in order to answer ten relevant business questions for the hospital network. These questions will help us understand the variables related to spending on hospital stays and provide valuable insights for decision making.

After this initial phase, we will advance to the second stage of the project, in which we will use the R language to carry out more in-depth statistical analyses. We will use ANOVA testing and Linear Regression to answer seven additional business questions. These statistical techniques will allow us to further explore the relationships between variables and gain a more accurate understanding of the factors that influence spending on hospital stays. With the combination of the analytical skills of the SQL language and the R language, this project aims to provide the hospital network with a comprehensive and detailed view of hospitalization expenses. It is expected that the results obtained will help optimize financial resources and improve the services provided, always aiming at the well-being of patients. By uniting these two powerful data analysis tools, this project aims to open new perspectives for making informed and evidence-based decisions. Exploratory data analysis using SQL and statistical analysis using the R language form a comprehensive and effective approach to understanding hospitalization costs.

Data dictionary:

AGE: Patient Age

FEMALE: Binary variable that indicates that the patient is female

LOS: Patient length of stay

RACE: Patient's race

TOTCHG: Cost of hospitalization

APRDRG: Refined Patient Diagnosis Group

Keywords: R Language, Data Analysis, SQL, Linear Regression, ANOVA, Finance Analaysis, Statistics Analysis, sqldf.

# ✅ PROCESS

Business Questions .:. Exploratory Analysis .:. SQL Language

How many races are represented in the dataset?
What is the average age of patients?
What is the age mode of the patients?
What is the variance of the age column?
What is the total expenditure on hospital admissions by age?
What age generates the highest total expenditure on hospital admissions?
What is the total expenditure on hospital admissions by gender?
What is the average expenditure on hospital admissions by patient race?
For patients over 10 years old, what is the average total expenditure on hospitalizations?1
Considering the previous item, which age has an average spending greater than 3000?

Business Questions .:. Statistical Analysis .:. R Language

What is the age distribution of patients attending the hospital?
Which age group has the highest total hospital spending?
Which diagnosis-based group (Aprdrg) has the highest total hospital spend?
Is the patient's race related to the total amount spent on hospital admissions?
Does the combination of age and gender of patients influence the total expenditure on hospital admissions?
As length of stay is the crucial factor for inpatients, we wanted to find out whether length of stay can be predicted from age, gender, and race.
Which variables have the greatest impact on hospitalization costs?

# ✅ CONCLUSION

Exploratory Analysis: All answers from the first stage of questions are present within the algorithm in Language R.

Statistical Analysis: Question 1.
A relevant piece of information that stands out in the analyzed data is that children aged between 0 and 1 year old are the ones who attend the hospital the most. This data underscores the importance of understanding hospitalization costs in this specific age group and identifying the main factors that contribute to these costs. The frequent need for medical care for children in this age group can be attributed to several reasons, such as the early development of the immune system, greater susceptibility to diseases and specific medical conditions related to the neonatal period. In addition, parents or guardians may be more likely to seek hospital care to ensure the health and well-being of their young children.

Question 2: Data analysis reveals that children aged between 0 and 1 year are responsible for the highest expenses in the hospital environment. This fact emphasizes the importance of understanding the factors that influence these costs and seeking efficient strategies to deal with the specific health demands of this age group. Detailed knowledge about spending patterns on these hospitalizations will allow hospitals to direct resources and implement adequate preventive measures, aiming to provide quality care and minimize the financial impact on families and the health system as a whole.

Question 3: When analyzing the data, it is observed that the refined diagnosis group 640 is responsible for the highest total expenditure in the context of hospital admissions. This information underscores the need to understand the factors that contribute to the costs associated with this specific group of patients. Deepening the analysis in this group will allow identifying the main medical conditions, treatments and services involved, enabling the implementation of targeted strategies to optimize resources, improve the quality of care and seek more efficient solutions in terms of cost-benefit.

Question 4: To investigate the relationship between the patient's race and the total cost of hospitalization, we will perform an ANOVA test. The dependent variable will be the total cost (TOTCHG) and the independent variable will be the race (Race). The null hypothesis (H0) states that there is no effect of race on total spending, while the alternative hypothesis (H1) suggests that there is an effect. After the analysis, we get a p-value greater than 0.05, which causes us to fail to reject the null hypothesis (H0). Therefore, we conclude that patient race does not have a significant influence on total hospital stay expenditure, based on available data.

Question 5: To analyze the influence of age (AGE) and gender (FEMALE) on hospital costs (TOTCHG), we will use an ANOVA test. The null hypothesis (H0) states that there is no effect of age and gender on hospital costs, while the alternative hypothesis (H1) suggests that there is a significant effect. After the analysis, we obtain a p-value less than 0.05, which leads us to reject the null hypothesis. We conclude, therefore, that there is a significant effect of age and gender on hospital costs. This indicates that both patient age and gender have a statistically significant influence on hospitalization costs, based on the analyzed data. This information is essential to better understand the factors that affect hospital costs and can provide valuable insights for decision-making and the efficient management of financial resources in a healthcare context.

Question 6: To investigate the relationship between the length of stay (LOS) and the independent variables (AGE, FEMALE and RACE), we will use a Linear Regression model. The null hypothesis (H0) states that there is no linear relationship between the dependent variable and the independent variables, while the alternative hypothesis (H1) suggests that there is a linear relationship. When performing the analysis, we observed that the p-value is greater than 0.05 in all cases, indicating that we failed to reject the null hypothesis (H0). Therefore, we conclude that the length of stay cannot be predicted from the independent variables (AGE, FEMALE and RACE) used in this model. This suggests that other variables or factors not considered in this analysis may be more related to the length of hospital stay. It is important to explore other possible variables or approaches to better understand the determinants of length of stay and provide a more accurate prediction.

Question 7: To analyze the relationship between the total cost of health care (TOTCHG) and the independent variables (AGE, FEMALE, LOS, RACE and APRDRG), we will use a Linear Regression model. The null hypothesis (H0) states that there is no linear relationship between the dependent variable and the independent variables, while the alternative hypothesis (H1) suggests that there is a significant linear relationship. When carrying out the analysis, we can observe that, in the previous models, the variables AGE, LOS and APRDRG were identified as the most relevant to explain and predict expenses with hospitalizations.This tells us that the patient's age, length of stay in the hospital, and refined diagnostic group are key factors that influence health care costs. These three variables demonstrate a significant relationship with the total cost of hospital admissions.

It is important to highlight that, although the variable FEMALE and the variable RACE were also included in the model, they were not significant in explaining the expenses with hospitalizations.Therefore, based on previous analyses, we can conclude that patient age, length of hospital stay and refined diagnosis group (APRDRG) are the most relevant and significant variables to explain and predict the costs associated with hospital admissions. This reinforces the importance of considering these factors when assessing and planning resource allocation and financial management in healthcare institutions.

# ✅ DATA SOURCERS

https://www.cms.gov/Research-Statistics-Data-and-Systems/Statistics-Trends-and-Reports/Medicare-Provider-Cost-Report/HospitalCostPUF

https://healthdata.gov/

