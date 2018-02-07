# NC-Residents

![alt text](https://github.com/kabrink/NC-Residents/blob/master/Screenshot%20Tableau%20Dashboard.png)

**Tableau**: https://public.tableau.com/shared/68B33QZBX?:display_count=yes

## Executive Summary
- Explored data on citizen satisfaction with North Carolina government services
- The NC government should consider improvements to public transportation, parking, and availability of government information to improve citizen satisfaction
- The survey should be updated to include questions that address citizens’ largest concerns: public schools, police protection, city streets, traffic flow, and bike facilities.

## Process

### Dataset: Raleigh, NC - 2016 Resident Survey 
- https://opendurham.nc.gov/explore/dataset/2016-with-county-and-city/
- 735 citzens completed the survey 
- 192 survey items 
- Survey assessed citizen satisfaction with the delivery of government services

### Problem
- Pinpoint problems with government services to recommend improvements to the NC government
- Determine if survey design appropriately addresses the topics that citizens are most concerned about

### What I learned
#### Potential Issues with Government Services:
1. In general, citizens are satisfied with government services that they receive (residents mostly report that they are satisfied or very satisfied with the services provided) 
2. Public transportation, parking, and availability of government information are potential services in need of improvement (these services were ranked most poorly across citizens)
3. In general, each district is equally satisfied with its services
   - Note that District 1 was ranked more poorly than the top performing districts (1, 2, and outlying areas); if this trend continues, District 1 may require more attention from the NC government
4. Dissatisfaction with public transportation and parking may be linked to geographical regions
   - Dissatisfaction with public transportation appears higher outside of the county center
   - Dissatisfaction with parking appears higher near the county center
   
#### Survey Design:
1. Citizens’ top 5 concerns were
   - Quality of Public Schools 
   - Quality of Police/Sheriff Protection
   - Maintenance of City Streets 
   - Traffic Flow 
   - Quality of Bike Facilities
2. Satisfaction with 4 out of 5 of these issues could not be measured by the survey (there were not enough questions on these topics). Future surveys should include more questions to measure citizens’ concerns and satisfaction on issues that matter to them.

### What I did
1. ***Selected a dataset*** that most closely resembles one type of DataRobot’s HR data (i.e., survey measures of satisfaction)
2. ***Summarized variables*** of interest
3. ***Reduced data*** into meaningful categories of services using data-driven techniques
4. ***Extracted 8 categories*** of government services
5. ***Visualized satisfaction*** for each of those categories and whether satisfaction differed by geographical location 
6. ***Analyzed differences*** in ratings of satisfaction 

### How I did it
1. ***Summarized variables (R)***
   - I examined variables that measured citizen reported top concerns (“What do you think should receive the MOST EMPHASIS from City and County leaders over the next two years?”) 
2. ***Reduced data (R)*** 
   - Using Exploratory Factor Analysis (EFA), I reduced a dataset of 192 variables into 8 categories of government services. Unlike other forms of dimension reduction, EFA can identify meaningful and descriptive categories of data within a dataset. 
3. ***Extracted categories (R)***
   - After identifying 8 categories using EFA, I created aggregate measures of satisfaction for these categories.  
4. ***Visualized satisfaction (Tableau)*** 
   - I created a plot of satisfaction by government service to identify any problem areas (i.e., which services show substantially less satisfaction) (See “1. Satisfaction” in dashboard)
   - I created a plot of satisfaction by district to identify whether any specific districts were performing more poorly than any other district (See “3. Satisfaction by District” in dashboard)
   - I plotted satisfaction by geographical location to see whether any specific geographical area was performing poorly in a certain government service (See “2. Satisfaction - Durham, NC” in dashboard)
5. ***Analyzed differences (R)***
   - Using ANOVA and post-hoc tests, I analyzed whether there were any categories or districts that had significantly lower ratings of satisfaction
