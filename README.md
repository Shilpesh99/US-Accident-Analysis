# US-Accident-Analysis
## Problem Statement
Investigate the patterns and trends in accident occurrences across the United States from 2016 to 2023 to address the problem of increasing accident rates and their causes. Focus on city-specific accident rates, seasonal and time-of-day variations, and the impact of weather conditions. The goal is to identify key factors contributing to high accident frequencies and trends, including geographic and temporal patterns, to inform safety measures and traffic management strategies. The planning process will involve data collection, analysis, and the development of actionable insights to enhance road safety.

## Dataset
Dataset : US Accidents (2016 - 2023) by Sobhan Moosavi <br>
Dataset Link : https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents <br>
This is a countrywide car accident dataset that covers 49 states of the USA. The accident data were collected from *February 2016 to March 2023*, using multiple APIs that provide streaming traffic incident (or event) data. The dataset currently contains approximately *7.7 million* accident records.

## Exploratory Data Analysis
*Data Preprocessing :* <br>
`import pandas as pd`

*loaading dataset* <br>
![image](https://github.com/user-attachments/assets/1fb3465c-dc6a-4695-a0ad-f8a360320de8) <br>
![image](https://github.com/user-attachments/assets/b37ee6e2-64e5-4d89-a94e-025ddc59ff3c)

*checking index for columns* <br>
`df.columns` <br>
![image](https://github.com/user-attachments/assets/1137b4b8-8503-4823-8d82-76bac6bee236)

*checking datatype of columns* <br>
`df.info()`

*generating descriptive statistics for the dataframe* <br>
`df.describe()`

*checking for columns containing numerical values* <br>
`numerics = ['int16', 'int32', 'int64', 'float16', 'float32', 'float64']` <br>
`numerics_df = df.select_dtypes(include=numerics)` <br>
`len(numerics_df.columns)`

*looking for null values* <br>
`df.isnull().sum().sort_values(ascending=False)`

*EDA :* <br>
`df.City` <br>
*looking for number of unique values of city* <br>
`uni_city = df.City.unique()` <br>
`len(uni_city)` <br>
![image](https://github.com/user-attachments/assets/ace0d1cb-a43a-4ac5-9bc0-4b08660fcee5)

*checking for number of times cities occurs* <br>
`accidents_by_city = df.City.value_counts()` <br>
`accidents_by_city` <br>
**City
Miami                           186917
Houston                         169609
Los Angeles                     156491
...
Wildrose                             1
Mc Nabb                              1
American Fork-Pleasant Grove         1
Name: count, Length: 13678, dtype: int64**
![image](https://github.com/user-attachments/assets/15123a02-a668-4ee2-953e-86723901b142)

`accidents_by_city[:20]`

*checking for New York data* <br>
`'New York' in df.City` <br>
**False** <br>
`'NY' in df.State` <br>
**False** <br>
From the above observation we can see that this dataset doesn't contain 'New York City' data, even if this is the most populated city of US.


Implement Targeted Traffic Management:

Focus on high-accident areas, especially in cities like Miami and California. Enhance traffic control measures during peak hours (6 AM to 10 AM) and weekdays to manage congestion.
Conduct Safety

Campaigns and Outreach:

Launch targeted safety campaigns to educate drivers about the risks of accidents, particularly in high-accident areas, during peak times, and in cooler or winter conditions.

Upgrade Infrastructure:

Improve road infrastructure in high-accident cities and regions, including better signage, lighting, and road conditions. Prioritize upgrades in the Eastern United States and in areas with high accident frequencies.

Introduce Weather-Responsive Safety Measures:

Develop and enforce specific safety protocols for fair weather conditions, as well as for cooler and winter conditions. Adjust road maintenance and safety measures accordingly.

Investigate and Address Data Anomalies:

Examine the over 1,000 cities with only one reported accident to ensure data accuracy and completeness. Use findings to improve data collection and address any discrepancies or gaps.
