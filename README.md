
# Global-Coffee-Health-Analysis



The objective of this analysis is to investigate patterns between coffee consumption, caffeine intake, sleep, stress, heart rate and other lifestyle/health factors, while also identifying differences across age groups, occupations and countries.

The dashboard was designed to answer questions such as:

Who consumes the most coffee?
Which occupations have the highest coffee consumption?
How does caffeine intake vary across groups?
What sleep-quality patterns exist among coffee consumers?
How are sleep hours associated with stress levels?
Which age groups show higher recorded heart rates?
Which countries show relatively high coffee intake?





<img width="1855" height="631" alt="Coffe Health Dashboard" src="https://github.com/user-attachments/assets/627a2dd0-d9f8-47e3-9466-8f80bf9ac643" />







Dataset Structure
The dataset contains the following major variables:



<img width="987" height="579" alt="structure 1" src="https://github.com/user-attachments/assets/e82f59f2-ed11-4bab-bd64-d4d2b3503613" />
<img width="979" height="559" alt="structure 2" src="https://github.com/user-attachments/assets/b1b0e232-c6ec-4156-9327-9866da31c0f2" />





PRE-ANALYSIS BOARD
Dependent and Independent Variables
There isn’t one universally correct dependent variable for this dataset because the appropriate variable depends on the research question.

For the overall coffee-health investigation, I recommend defining the variables this way:



Dependent Variables
These are the health/well-being outcomes we want to understand:

Sleep_Quality
Stress_Level
Heart_Rate
Health_Issues



Independent Variables
These are variables that may be associated with the outcomes:

Coffee_Intake
Caffeine_mg
Age
Gender
Sleep_Hours
BMI
Physical_Activity_Hours
Occupation
Smoking
Alcohol_Consumption
Country





Pre-Analysis Questions


Coffee Consumption
Which occupation has the highest coffee consumption?

Which countries have the highest coffee intake?

Does coffee consumption vary by age?

Does coffee consumption differ between males and females?



Caffeine and Health

Does higher caffeine intake correspond with differences in sleep quality?

Is caffeine intake associated with heart rate?

Are high caffeine consumers concentrated in particular occupations?



Sleep

How does sleep quality vary across the population?

Is fewer sleep hours associated with higher stress levels?

Which stress category has the greatest recorded sleep duration?



Lifestyle

Is physical activity associated with sleep quality?

Do smoking and alcohol consumption appear alongside different health patterns?

Does BMI differ across coffee-consumption groups?



Demographics

Which age groups have the highest recorded heart rates?

Are particular occupations associated with higher coffee consumption?

Are there notable country-level differences in coffee intake?





Pre-Analysis Hypotheses

You can also include hypotheses before presenting the dashboard findings.



Hypothesis 1

Higher caffeine consumption may be associated with differences in sleep quality.



Hypothesis 2

Higher stress levels may be associated with shorter sleep duration.



Hypothesis 3

Coffee consumption may vary considerably across occupations.



Hypothesis 4

Caffeine intake may show an association with recorded heart rate.



Hypothesis 5

Coffee-consumption patterns may differ between countries and demographic groups.






IN-ANALYSIS BOARD

This is where you explain what the dashboard revealed.



Youngest Coffee Lovers

The dashboard identifies 18 years as the youngest age represented among the coffee-consuming groups.

The “Youngest Coffee Lovers” visual shows age 18 with the largest displayed aggregate value, followed by ages 32, 34, 35 and 37.



Coffee Lovers by Occupation

The Coffee Lovers by Occupation visual shows:






<img width="1090" height="414" alt="occupation" src="https://github.com/user-attachments/assets/3a66d6b6-6d15-42c5-8037-d664124d390d" />






Sleep Quality

The dashboard categorizes sleep quality into:

Good

Fair

Excellent

Poor


The displayed aggregate values are approximately:





<img width="1094" height="355" alt="sleep" src="https://github.com/user-attachments/assets/ccbe2b75-8278-4883-ae81-2c7f821d8890" />





Caffeine Consumption

The dashboard’s caffeine visualization shows the following aggregated values:






<img width="1069" height="398" alt="caffeine" src="https://github.com/user-attachments/assets/580d6818-0184-4aff-af72-2b88a79d8a1a" />






Ages With High Heart Rate

The dashboard highlights:





<img width="923" height="485" alt="age-rate" src="https://github.com/user-attachments/assets/97937e09-dc29-44ec-8e6d-1881cebd762c" />






Country-Level Coffee Consumption

The dashboard identifies countries with high coffee-intake values, with Canada prominently highlighted and China also appearing among the displayed countries.






POST- ANALYSIS BOARD


Observation Board


1. Coffee consumption differs by occupation;
Office participants have the highest aggregated coffee-intake value in the dashboard.

This suggests that occupation is worth investigating as a potential factor associated with coffee consumption.


2. Caffeine follows a similar occupational pattern;
Office participants also have the highest displayed aggregate caffeine value.

This indicates a relationship between the dataset’s coffee-consumption and caffeine variables.


3. Sleep and stress show a visible pattern;
The dashboard shows substantially more total sleep hours among participants classified as having Low stress than those classified as having High stress.

However, group sizes must be considered before interpreting this as a per-person relationship.


4. Sleep quality varies substantially;
Good sleep quality is a major category in the dataset, while Fair, Excellent and Poor sleep quality are also represented.

This creates an opportunity to examine whether coffee and caffeine intake differ between sleep-quality categories.


5. Age 18 is prominent in several dashboard analyses;
Age 18 appears in the youngest-coffee-lovers analysis and also has the largest displayed aggregate heart-rate value.

This makes the age group particularly interesting for further investigation, but the result should be validated using averages and participant counts.


6. Aggregation is an important analytical issue;
The dashboard contains several SUM-based visuals.

This is appropriate for measuring overall volume but not always appropriate for comparing individual health outcomes.

For example:

Total heart rate ≠ average heart rate

and

Total sleep hours ≠ average sleep hours.

This is one of the most important technical considerations when interpreting the dashboard.





Post-Analysis Recommendation


1. Replace selected SUM metrics with averages
For health-related comparisons, use:

Average Coffee Intake

Average Caffeine mg

Average Sleep Hours

Average Heart Rate

Average BMI

This will make comparisons between groups more meaningful.




2. Add participant counts
Every major group comparison should include:

Number of Participants

For example:

Office — Average Coffee Intake: X | Participants: Y

This allows users to understand whether a high total is caused by higher consumption or simply a larger group.



3. Create a Coffee Intake vs Sleep Quality analysis
A useful visual would be:

Average Caffeine mg by Sleep Quality

with categories:


Excellent

Good

Fair

Poor

This would directly address one of the project’s main health questions.



4. Analyze caffeine against heart rate
Create a scatter plot:


Caffeine mg → Heart Rate

Add a trendline where appropriate.

This would help determine whether the dataset shows an association between caffeine exposure and heart rate.



5. Analyze stress and sleep using averages
Replace the current total sleep-hour comparison with:


Average Sleep Hours by Stress Level

This would make the relationship easier to interpret.



6. Control for lifestyle factors
Coffee and health outcomes may also be associated with:


Physical activity

Smoking

Alcohol consumption

BMI

Age

Occupation

Therefore, these variables should be considered before attributing differences in health outcomes to coffee consumption.



7. Improve the country analysis
Use:

Average Coffee Intake by Country

rather than only total intake.

A map can then display the average consumption while a separate KPI shows the number of participants represented by each country.





TECHNICAL LIMITATIONS
Several limitations should be acknowledged.


1. Observational data
The dataset can identify associations but cannot establish that coffee or caffeine caused a health outcome.


2. Synthetic dataset
The dataset is identified as synthetic_coffee_health_10000, meaning it should not be treated as a representative clinical population.


3. Aggregate dashboard measures
Several dashboard values appear to use SUM rather than averages.


4. Unequal group sizes
Differences between occupations, countries and age groups may partly reflect different numbers of participants.


5. Potential confounding
Age, occupation, physical activity, smoking, alcohol consumption and BMI may influence health outcomes independently of coffee consumption.


6. Health interpretation
The dashboard should be treated as a data-analysis project rather than a medical assessment.





CONCLUSION
The Global Coffee Health Analysis provides a multidimensional view of coffee consumption and its relationship with demographic, lifestyle and health-related variables.

The dashboard shows noticeable differences in coffee consumption across occupations, countries and age groups. Office participants have the highest displayed aggregate coffee and caffeine values, while Canada is highlighted among the countries with high coffee intake. The analysis also reveals a substantial difference in total sleep hours across stress categories and highlights several age groups with high aggregated heart-rate values.

However, the most important technical conclusion is that aggregate totals should not be interpreted as individual-level health outcomes. Differences in group size can substantially affect SUM-based visualizations.

For a stronger analytical model, the next stage should focus on average coffee/caffeine intake, average sleep hours, average heart rate and participant counts, followed by relationship analyses such as caffeine versus heart rate and coffee intake versus sleep quality.

Overall, the project demonstrates how demographic, behavioral and health variables can be combined in Power BI/Excel to identify patterns and generate data-driven questions. The findings provide a foundation for deeper statistical analysis while emphasizing the distinction between association and causation.





REFERENCE

kaggle.com




