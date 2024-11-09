# IBM-DataScienceCapstone-SpaceX-project
## Introduction
![image](https://github.com/user-attachments/assets/ff7b246b-c87a-40ac-b872-2ca0553a5a7d)
### Background
SpaceX advertises its Falcon 9 launches at $62 million per mission, a substantial savings compared to other providers who charge upwards of $165 million per launch. Much of this cost efficiency comes from SpaceX’s ability to reuse the rocket’s first stage. Accurately predicting whether this first stage will land successfully allows for more precise launch cost estimations, which is essential for companies, like SpaceY, that seek to competitively bid against SpaceX. Data for this analysis is gathered from available APIs and preprocessed to ensure quality and consistency. By investigating both successful and unsuccessful launch events, the project will identify key factors influencing landing outcomes, supporting more cost-effective and strategically planned space mission.

### Project Objectives
Analyze the impact of key factors such as payload mass, launch site, number of flights, and orbit type on landing success.
Examine trends in launch success rates over time to assess improvements.
Identify the most effective model for predicting successful landings through classification analysis.
## Executive Summary
This project explores the variables that influence a Falcon 9 rocket’s first-stage landing outcome. The methodology includes data collection from SpaceX’s API and web scraping, data wrangling to prepare variables for analysis, exploratory analysis with SQL and visualization tools, and model building to predict landing success.

### Methodology
#### Data Collection
API data: Retrieved launch details such as flight number, payload mass, orbit type, and launch site from the SpaceX API.
Web scraping: Supplemented data with historical launch records from Wikipedia.
#### Data Wrangling
Processed the data to handle missing values and create a binary classification target variable (1 for success, 0 for failure).
#### Exploratory Data Analysis (EDA)
Visualizations and SQL queries were used to explore relationships between payload mass, launch site, orbit type, and success rates.
Created maps with Folium to visualize the geographical distribution of launch sites and proximity to coasts, supporting safe recovery zones.
#### Predictive Modeling
Built multiple classification models (Logistic Regression, SVM, Decision Tree, K-Nearest Neighbor) to predict landing success, with the Decision Tree showing the best performance.
## Key Findings
### Exploratory Data Analysis
Improved Success Over Time: Landing success has significantly improved since 2013, highlighting advancements in SpaceX’s recovery technology.
Launch Site and Orbit Insights: KSC LC-39A showed the highest success rate, while orbits such as ES-L1, GEO, HEO, and SSO achieved a 100% success rate.
Mapping Analysis: Coastal sites near the equator offer ideal launch locations, benefiting from Earth’s rotational speed and reducing fuel costs.
### Predictive Model Performance
The Decision Tree classifier slightly outperformed other models, accurately predicting landing outcomes and offering practical insights for SpaceY’s mission planning.
### Visualization & Analytics
Most launch sites are close to the coast, minimizing risks and optimizing launch efficiency.
The equatorial launch locations provide a natural rotational boost, saving fuel and reducing mission costs.
## Conclusion
#### Improved Landing Success Over Time
Success rates showed a clear upward trend from 2013 to 2020, driven by advancements in SpaceX’s landing technology and reliability
#### Strategic Launch Site Utilization
KSC LC-39A had the highest success rate, highlighting its strategic importance. Coastal launch sites near the equator, such as Cape Canaveral, provide safe recovery zones over the ocean and benefit from Earth’s rotation, optimizing launch efficiency
#### Orbit and Mission Trends
Orbits like ES-L1, GEO, HEO, and SSO achieved a 100% success rate, showing reliability for specific mission types. Other orbits, like SO, faced greater challenges, impacting mission success variability
#### Map-Based Insights on Launch Sites
Interactive map analysis revealed that launch sites are strategically located near coastlines but away from populated areas, minimizing risks and optimizing logistics. Color-coded markers on the map illustrated success and failure rates at each site, allowing a quick visual assessment of site-specific performance over time
#### Predictive Model Performance
The Decision Tree classifier was the top-performing model, accurately predicting outcomes and enabling data-driven decisions for future missions.
