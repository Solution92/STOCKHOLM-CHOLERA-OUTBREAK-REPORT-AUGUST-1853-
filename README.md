# STOCKHOLM-CHOLERA-OUTBREAK-REPORT-AUGUST-1853

## Table of Content
- [Project Overview](#project-overview)
- [Data Source](#data-source)
- [Tools Used](#tools-used)
- [Data Cleaning and Preparation](#data-cleaning-and-preparation)
- [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-eda)
- [Data Analysis](#data-analysis)
- [The Dashboard](#the-dashboard)
- [Result and Findings](#result-and-findings)
- [Recommendation](#recommendation)
- [Limitations](#limitations)
- [Reference](#reference)


### Project Overview

The Stockholm Cholera Outbreak of August 1853 was a historical event during which cholera, a waterborne disease, spread throughout the city. Cholera is caused by the bacterium Vibrio cholerae and leads to severe diarrhea and dehydration. This outbreak was a significant public health concern because it led to the death of about 3,000 people.

The foregoing brought about the necessity of this project to analyze and answer a few questions.

### Data Source

The dataset was provided in a CSV file format by the client which I am not permitted to disclose.

### Tools Used

Excel and Power BI.

### Data Cleaning and Preparation

The Dataset used in this Analysis may be limited in several ways because it was collected by manual writing in a church environment.

![Screenshot_143](https://github.com/Solution92/STOCKHOLM-CHOLERA-OUTBREAK-REPORT-AUGUST-1853-/assets/144762124/9ce5defc-eac6-47ab-8d5b-3e1b6eee3101)
Raw File — Swedish language

![Screenshot_144](https://github.com/Solution92/STOCKHOLM-CHOLERA-OUTBREAK-REPORT-AUGUST-1853-/assets/144762124/ab5c1b45-6383-4326-8066-3cb36a80db51)
After translation

The dataset has only 8 columns and 249 active rows with a lot of unwanted values and irrelevant and unprintable characters. The Column names after translation are ‘Date of death’, ‘Name’, ‘Profession’, ‘Sex’, ‘Age’, ‘Assembly’, ‘Archive Ref’, as well as ‘Page’.

The Dataset has gone through several processes of standardizing before creating the dashboard.

From the “TRIM” function to the “CLEAN”, Replacement of unwanted values, Removing of Errors, and so on.

I created several other Columns like “Month Name”, “Day Name”, and a conditional Column named “Age Categories”, using

Ages 1–11 as Children,

Ages 12–19 as Teenagers,

Ages 20–30 as Young Adult,

Ages 31–40 as Adult,

Ages 41–50 as Senior and

Ages 51 and Above as Aged

This Transformation process was successfully completed using the Power query editor before loading the Dataset to Power BI Desktop for further insights and Visualization.

### Exploratory Data Analysis (EDA)

The following Key Performance Indicators (KPIs) were calculated using the appropriate formula.
- Total No. of Death
- Count of Male
- Count of Female
- MAX AGE
- Total Death by Day
- Gender Analysis: Count of Men/Women’s Death
- Total Death by Month
- Death by Age Categories Analysis
- Death by Profession Analysis

### Data Analysis
~~~
Total No. of Death = COUNTROWS(‘Cholera Outbreak’) = 239

Count of Male = Count of Male = COUNTROWS(FILTER(‘Cholera Outbreak’,’Cholera Outbreak’[Sex]=”MAN”)) = 112

Count of Female = COUNTROWS(FILTER(‘Cholera Outbreak’,’Cholera Outbreak’[Sex]=”WOMAN”)) = 127

MAX AGE = MAX AGE = MAX(‘Cholera Outbreak -Age’[Age]) = 86
~~~

### The Dashboard

![Screenshot_145](https://github.com/Solution92/STOCKHOLM-CHOLERA-OUTBREAK-REPORT-AUGUST-1853-/assets/144762124/b9022042-9949-4fab-9c36-e7a2b2981b4d)

### Result and Findings

Below are my findings from the table 
- At 44, Thursday had the highest Count of Name_of_death and was 100.00% higher than Sunday, which had the lowest Count of Name_of_death at 22.  Thursday accounted for 18.41% of Count of Name_of_death.  Across all 7 Day Name, Count of Name_of_death ranged from 22 to 44.  
- Meanwhile, Count of Name_of_death for Woman (127) was higher than MAN (112).  Woman accounted for 53.14% of Count of Name_of_death.  
- At 175, September had the highest Count of Name_of_death and was 1,490.91% higher than November, which had the lowest Count of Name_of_death at 11.  September had the highest Count of Name_of_death at 175, followed by October, August, and November.  September accounted for 73.22% of Count of Name_of_death.  Across all 4 Month Name, Count of Name_of_death ranged from 11 to 175.  
- In the same vein, at 55, Children had the highest Count of Name_of_death and was 587.50% higher than Teenager, which had the lowest Count of Name_of_death at 8.  Children accounted for 23.01% of Count of Name_of_death.  Across all 6 Age Categories, Count of Name_of_death ranged from 8 to 55.  
- Finally, Count of Name_of_death was highest for Mamsell at 10, followed by Boy child and Worker.  Mamsell accounted for 4.18% of Count of Name_of_death.  Across all 148 Profession, Count of Name_of_death ranged from 1 to 10.  

### Recommendation

- From the findings above, Thursdays had the highest count of deaths, suggesting a potential pattern or trend that may be further investigated. 
- Secondly, the higher count of deaths among women compared to men may warrant closer examination to understand the underlying factors. 
- The concentration of deaths in September is noteworthy, and it may be beneficial to explore potential seasonal or environmental influences during that month. 
- Furthermore, the higher count of deaths among children suggests a need for targeted interventions or investigations into factors affecting this age group. 
- Finally, the profession with the highest count of deaths, such as Mamsell, may require specific attention for further analysis and understanding of potential occupational risks.

### Limitations

- The Dataset used in this Analysis may be limited in several ways because it was collected by manual writing in a church environment.
- Temporal and Historical Context: The dataset is limited to the year 1853, which might not be representative of contemporary mortality patterns or reflect changes in societal, medical, or environmental factors over time.
- Categorical and Limited Variables: The dataset provides a narrow view by categorizing professions, ages, and other variables in a simplified manner. This lack of granularity can hinder a more detailed analysis of specific risk factors or correlations.
- Potential Biases and Underrepresentation: The recording process and cultural biases of the time may lead to underreported or misclassified information. Certain groups or causes of death may be disproportionately represented or neglected, limiting the dataset's reliability.
- Small Sample Size: The dataset may have a relatively small sample size for comprehensive statistical analyses, potentially limiting the generalizability of findings to broader populations or contexts.

### Reference

Kaggle is a goodd place for such dataset.


#data #visualization #powerbi #cholera #stockholm #sweden #1853 #outbreak #excel #analysis #report #death #pandemic #quantun





















