# Medical Appointments No-Shows
## Project Overview
This project investigated a dataset of appoinment records for Brasil public hospitals and included information on their ability to show up for doctor's appointment.
The analysis explored factors affecting patients' ability to show up for appointment.
This project was completed as part of Udacity's Data Analyst Nanodegree certification and the original problem description and data set can be found here: https://www.kaggle.com/joniarroba/noshowappointments/home
## Project Analysis Scope
Data gathering
Data wrangling
Exploratory Data Analysis
Conclusion
## Project Tools
Python, libraries: numpy, pandas, matplotlib, seaborn
## Findings
From the 'no_show" plot, we observe that the patients who attended their scheduled appointment were far more than those that did not.

It was observed from the plot between "Scholarship" and "no_show" that majority of people who made it to the appointment were not enrolled in the welfare program. Several factors could be responsible among which could be a clash in timimg between welfare meetings and appointment date or little emphasis on the need to make the doctor's appointment by the welfare program officials. This will require further investigation for confirmation.

Surprisingly, people who did not receive sms notification attended more appointments than those who received. One would expect that sms notification would motivate patients to make their appointments but this was not the case. In terms of cost for the hospital, it could mean that they need to channel their focus elsewhere and cut down on the costs incurred semding sms to patients as this is not effective.

Across both genders, the people who attended appointments were more than those who did not.

The plot between "illness incidence" and "no_show" revealed that as the reported cases of illnesses increased, the number of patients who attended their appointments declined. This could be as a result of constraints caused by the illnesses making it it difficult for patients to leave their homes unassissted.

The age distribution is right-skewed with most patients around 0 years of age. The large number of patients in the 0 years age bracket could imply that the appointments were pediatric appointments for nursing mothers.

From the logistic regression, SMS_received and illness_incidence corroborated the relationship shown in the visualization plot. Both variables have negative coefficients showing an inverse relationship with the dependent variable. Using their odd ratios, the odd ratio of 0.55 indicates that for every sms notification sent, the odds of a patient showing up for an appointment decreases by 0.55. Furthermore, a value of 0.99 indicates that for every additional illness experience, the odds of showing up for an appointment declines by 0.99. In addition, even though the dataset has more female paients, the logistic regression reports that the odds of showing up for an appointment increases by 1.00 and an increase in age by one year increases the odds of showing up for an appointment by 1.00. Finally, contrary to what the plot between scholarship and no_show displays, the logistic regression reported that joining the welfare program increases the odds of showing up for an appointment by 0.83.

The p-values show that the effect of ALL the predictors on the dependent variable is highly significant.
