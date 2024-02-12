# Infographic-Analysis-Criminal-Behavior-Patterns-and-Trends-in-Iowa

## Background of the problem
The United States of America is known for having one of the highest crime rates in the world. Iowa, a Midwestern state in the United States, has a population of approximately 3.2 million people. Like many other states in the US, Iowa faces challenges related to crime and incarceration. While the state has a lower crime rate compared to many other states, it still faces issues related to public safety and criminal justice. In this project we choose the two datasets, Iowa Prison Admissions and Offenders Released from Iowa Prisons to analyze the data and visualize the the functioning of the criminal justice system, including patterns in arrests, convictions, and sentencing in Iowa State. The criminal justice system in the state of Iowa is an essential aspect of the state’s efforts to maintain public safety and uphold the law. To better understand the functioning of the system, data on the number of offenders admitted and released from Iowa prisons over the last ten years can provide valuable insights into the patterns and trends of incarceration in the state. It can also identify areas where policies and interventions could be implemented to improve the effectiveness and fairness of the criminal justice system.

## Research Questions
Are there any temporal variation (increase/decrease) in types of offenses over the years?
What are the trends in crime rates in different jurisdictions or counties over time?
How does the severity and frequency of crimes vary by demographic factors such as age, gender and race?
How does age relate to the types of crimes committed by offenders?
What is the ratio of Race & Ethnicity and Gender of Offenders?
What are the average sentence length in the prisons of Iowa by different types of offense?

## Data Description
The initial datasets are collected from Iowa Data portal (data.iowa.gov). For addressing the research questions, two datasets are extracted from the source. One dataset provides information regarding offenders admitted to Penitentiaries and Correctional Facilities in Iowa during the last 10 year. The other provides information regarding the release of individuals from prisons in Iowa with specific location of occurrence in the last 10 years. Since our research questions seek to observe geographic pattern of crime, the two datasets will be merged together in order to obtain the location details of crime. The prison admission dataset contains 16 variables and 49706 observations while the release from prison dataset contains 18 variables and 55900 observations.

## Variables of interest in two datasets are:

### Prison Admission Data
Record ID
Offender Number //
Fiscal Year Admitted
Sex
Race & Ethnicity
Supervising Institution
Offense Type
Offense Subtype
Age at Admission
Months Served

### Prison Release Data
Record ID
Jurisdiction

## Data Pre-Processing
For analyzing the research questions, the initial datasets are manipulated and manual transformation are done. Both data_admit and data_released were joined together to make a comprehensive dataset for addressing the research questions. Necessary variables were also created for data analysis. There are a number of variables in both datasets and some would be common after joining. To avoid redundancy the datasets were cut smaller with only the varibales of interests. For the purpose of analysis, some observations are merged together and some are given more intuitive names. For the purpose of analysis and visualization, the character variables are transformed into factor variables. To analyze some research questions, a few variables were created which contains the total number of offense per year and percentage of different offenses per year Offense Count, Yearly_total_offense would represent the total number of offense occurred per year.
