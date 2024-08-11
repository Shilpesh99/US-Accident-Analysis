# US-Accident-Analysis
## Problem Statement
Investigate the patterns and trends in accident occurrences across the United States from 2016 to 2023 to address the problem of increasing accident rates and their causes. Focus on city-specific accident rates, seasonal and time-of-day variations, and the impact of weather conditions. The goal is to identify key factors contributing to high accident frequencies and trends, including geographic and temporal patterns, to inform safety measures and traffic management strategies. The planning process will involve data collection, analysis, and the development of actionable insights to enhance road safety.

## Dataset
Dataset : US Accidents (2016 - 2023) by Sobhan Moosavi, *August,24*<br>
Dataset Link : https://www.kaggle.com/datasets/sobhanmoosavi/us-accidents <br>
This is a countrywide car accident dataset that covers 49 states of the USA. The accident data were collected from *February 2016 to March 2023*, using multiple APIs that provide streaming traffic incident (or event) data. The dataset currently contains approximately *7.7 million* accident records.

## Data Preprocessing
`import pandas as pd`

![image](https://github.com/user-attachments/assets/1fb3465c-dc6a-4695-a0ad-f8a360320de8) <br>
![image](https://github.com/user-attachments/assets/b37ee6e2-64e5-4d89-a94e-025ddc59ff3c)

## Exploratory Data Analysis
![image](https://github.com/user-attachments/assets/63515b94-6851-429f-ba38-0cb46ca63c81)
From the above graph we can see that Miami has the highest number of accidents in US.

![image](https://github.com/user-attachments/assets/129f7a99-804a-4173-b5c6-3e1b87503544)
From the above graph we can see that most the cities in US have very less number of accidents.

![image](https://github.com/user-attachments/assets/6a7ec7d0-f87d-4a17-b085-1260e7736339)
From the above graph we can see that a higher percentage of accident occurs between 6am to 10pm and 3pm to 6pm.

![image](https://github.com/user-attachments/assets/643af6d5-5b27-4aa0-a11c-0d25a15cd115)
From the above graph we can see that most accidents occurs on weekdays and less on weekends. 

![image](https://github.com/user-attachments/assets/61742deb-4e0b-481e-afd7-458505dc9911)
From the above graph we can see that most of the accidents occurs in December.

![image](https://github.com/user-attachments/assets/e56749c1-980d-4da2-ac8c-1b8453d3fd1f)
From the above graph we can see that most accidents occurs on the East side of the US.

![image](https://github.com/user-attachments/assets/c943a0be-5088-4822-9d4f-eced53a1a995)
From the above graph we can see that most accident occurs in California, Florida and Texas.

![image](https://github.com/user-attachments/assets/1674f41b-2f34-45f2-9d4e-75ba40d390c2)
From the above graph we can see that most accidents occurs in Fair, Mostly Cloudy, Cloudy, Clear and Partly Cloudy Weather Condition.

![image](https://github.com/user-attachments/assets/bb27b720-6537-4f63-a594-ccda8ee839bd)
From the above graph we can see that most of the accidents occur in Cooler Areas or in Winter Season.

![image](https://github.com/user-attachments/assets/60d6a7c2-6b38-4968-b272-cafcc12e603d)
From the above graph we can see that the number of accidents are increasing year over year.

## Recommended Solution
Implement Targeted Traffic Management: <br>
Focus on high-accident areas, especially in cities like Miami and California. Enhance traffic control measures during peak hours (6 AM to 10 AM) and weekdays to manage congestion.
Conduct Safety

Campaigns and Outreach: <br>
Launch targeted safety campaigns to educate drivers about the risks of accidents, particularly in high-accident areas, during peak times, and in cooler or winter conditions.

Upgrade Infrastructure: <br>
Improve road infrastructure in high-accident cities and regions, including better signage, lighting, and road conditions. Prioritize upgrades in the Eastern United States and in areas with high accident frequencies.

Introduce Weather-Responsive Safety Measures: <br>
Develop and enforce specific safety protocols for fair weather conditions, as well as for cooler and winter conditions. Adjust road maintenance and safety measures accordingly.

Investigate and Address Data Anomalies: <br>
Examine the over 1,000 cities with only one reported accident to ensure data accuracy and completeness. Use findings to improve data collection and address any discrepancies or gaps.
