The project focuses on examination of child welfare metrics, particularly child abuse rates and the effectiveness of Child Protective Services (CPS) intake and referral processes. This approach aims to unravel the complexities surrounding child welfare, offering insights into state-specific and national trends.

**Data Sets:** There are several key datasets namely, Iowa Child Abuse Occurrences, National Child Abuse Data, CPS Intakes, Screened-In CPS Intakes, and Recurrence Rates of Child Abuse. These handle characteristics of child welfare, from abuse occurrences to CPS processing outcomes.

**Research Questions:**

**1.	How do the types and rates of child abuse in Iowa compare to national averages, and what might these differences or similarities suggest about state-specific factors influencing child welfare?**
This aspect investigates how Iowa's child abuse types and rates compare to national figures. The analysis will explore whether state-specific factors such as demographic or policy differences contribute to the observed rates and could be crucial for tailoring interventions.

Required Columns: Iowadata.csv:  Year, Neglect Type(String), Occurrences(int)

For National Data(MaltreatmentTypes.csv): State(String), Victims(Int), Types of Neglects(Medical,Physical etc)(String).


**2.	What is the effectiveness of child protective services (CPS) intake and referral processes in every state compared to national average, particularly regarding outcomes for screened-in cases?**
The study will evaluate the operational efficacy of CPS intake and referral mechanisms across states.

ScreenedIn.csv:

State(String), Screened-In Referrals(Int),Screened-Out Referrals(int), Total Referrals(int)

**3.	Investigate the frequency of repeated abuse cases for each state relative to national data to evaluate the effectiveness of interventions?**
An examination of the frequency of repeated abuse cases provides insight into the effectiveness of interventions. High recurrence rates may signal gaps in support and monitoring, prompting a revaluation of current strategies.

Required Columns: State(String)	Year	Emotional Abuse (%)	Medical Neglect (%)	Neglect (%)	Physical Abuse (%)	Sexual Abuse (%)	Trafficking (%)	Other (%)	Missing Data (%)

**4.	How do referral sources impact the likelihood of CPS intakes being screened in for further action?"**
By analyzing how different referral sources affect the likelihood of CPS intakes being screened for further action, this inquiry seeks to uncover potential biases or efficiencies within the referral process.

CPS_Intakes.csv

Required Columns: Intake_Year	County(String)	REFERENT_TYPE(String)	DECISION(String)	Age_Group(Int)	child_count(Int)

**Models and Algorithms:**

For Analysis of Child Abuse Types and Rates:

•	**Descriptive Statistical Analysis**: We will use descriptive statistics to summarize the data, including mean, median, and standard deviation.

For CPS Intake and Referral Process Effectiveness:

•	**Logistic Regression**: This could be used to model the probability of cases being screened in versus screened out.

•	**Random Forests**: This algorithm can provide insight into the importance of different factors influencing the screening decision.

For the Impact of Referral Sources:

•	**Classification Models**: Logistic Regression and Random Forest could again be employed here to predict the likelihood of CPS intakes being screened in for further action based on the referral source and other covariates.

•	**Decision Trees**: These models could provide additional insights, offering a clear visualization of decision paths and handling complex interactions between features.
Few Model Comparison Metrics like Accuracy, Precision, Recall, F1-Score  could be used to evaluate model performances.

**Conclusion:**
The ultimate goal is to distill actionable insights from these analyses, offering evidence-based recommendations for enhancing child welfare systems. 




