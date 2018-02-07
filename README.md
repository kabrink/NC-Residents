# NC-Residents

**Tableau**: https://public.tableau.com/profile/kimberly.brink#!/vizhome/DataRobot-Dashboard/Dashboard1?publish=yes

### Dataset: Raleigh, NC - 2016 Resident Survey 
- https://opendurham.nc.gov/explore/dataset/2016-with-county-and-city/
- 735 residents completed the survey 
- 192 survey items 
- Survey assessed citizen satisfaction with the delivery of government services

### Problem
- Determine government services that citizens are not satisfied with 
- Pinpoint problem areas to recommend that the NC government focus on improving

### What I learned
1. In general, residents are satisfied with government services that they receive (residents mostly report that they are satisfied or very satisfied with the services provided) 
2. Public transportation, parking, and availability of government information are potential services in need of improvement (these services were ranked most poorly across residents)
3. In general, each district is equally satisfied with its services
   - Note that District 1 was ranked more poorly than the top performing districts (1, 2, and outlying areas); if this trend continues, District 1 may require more attention from the NC government
4. Dissatisfaction with public transportation and parking may be linked to geographical regions
   - Dissatisfaction with public transportation appears higher outside of the county center
   - Dissatisfaction with parking appears higher near the county center

### What I did
1. ***Selected a dataset*** that most closely resembles one type of DataRobot’s HR data (i.e., survey measures of satisfaction)
2. ***Reduced data*** into meaningful categories of services using data-driven techniques
3. ***Extracted 8 categories*** of government services
4. ***Visualized satisfaction*** for each of those categories and whether satisfaction differed by geographical location 
5. ***Analyzed differences*** in ratings of satisfaction 

### How I did it
1. ***Reduced data (R)*** 
   - Using Exploratory Factor Analysis (EFA), I reduced a dataset of 192 variables into 8 categories of government services. Unlike other forms of dimension reduction, EFA can identify meaningful and descriptive categories of data within a dataset. 
2. ***Extracted categories (R)***
   - After identifying 8 categories using EFA, I created aggregate measures of satisfaction for these categories.  
3. ***Visualized satisfaction (Tableau)*** 
   - I created a plot of satisfaction by government service to identify any problem areas (i.e., which services show substantially less satisfaction) (See “1. Satisfaction” in dashboard)
   - I created a plot of satisfaction by district to identify whether any specific districts were performing more poorly than any other district (See “3. Satisfaction by District” in dashboard)
   - I plotted satisfaction by geographical location to see whether any specific geographical area was performing poorly in a certain government service (See “2. Satisfaction - Durham, NC” in dashboard)
4. ***Analyzed differences (R)***
   - Using ANOVA and post-hoc tests, I analyzed whether there were any categories or districts that had significantly lower ratings of satisfaction
