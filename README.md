#  <span style="color:tan"> **Module 7 Project**  </span>


# Meet the Pyrates:

# 🦜 🏴‍☠️ ☠️ 💰 💰 💰 💰 💰 ☠️ 🏴‍☠️ 🦜

●	Rahma Ali, UofM

●	Paul Brichta, UofM

●	Chris Gruenhagen, UofM

●	Jason McHone, UofM

November 2022

# PyWear, the newest name in Disc Golf apparel

## Abstract
Our project is to gather data on Disc Golf for a fictional clothing company "PyWear". Pywear is a startup athleisure clothing brand that specializes in clothing tailored to meet the needs & aesthetic of Disc Golf players.  PyWear has a limited advertising budget so they need to narrow down their area of focus geographically. The marketing team understands the target customer very well so our focus is solely to find the best target market for their initial advertising campaign. In order to provide this area of focus we will review Disc Golf course locations across the US combined with the median household income where Disc Golf Courses are located. We will look for correlations between the median income and/or population & Disc Golf courses as we narrow our review. 

|Table of Contents|
|-----------------|
|Title Page|1|
|Abstract|2|
|Introduction|3|
|Methodology|4|
|Results|5|
|Summary & Conclusion|6|
|References |7|
|Acknowledgements|7|

---

## Introduction
PyWear needs assistance in determining the best geographic region in which to deploy their marketing strategy. They have created a clothing assortment tailored to the needs of Disc Golf players & they have researched the potential customer, but they have a limited marketing budget so they have to limit the target advertising market. We have been asked to help make that determination. We have agreed that we should concentrate on areas of higher participation in Disc Golf as well as areas with good median income. Given the limited selling information we have to limit our focus to demographic data. 
It is also important to PyWear that we provide an area of the country with a higher level of affinity for Disc Golf as they are planning to expand and identifying a focus region will help to maximize efficiencies in marketing, logistics and assortment building. 

## Methodology
In this study, over 7000 Disc Golf locations in the United States were plotted to determine the areas of the country that had the highest number of Disc Golf courses.
This data was analyzed to determine the best region of the country to narrow the focus of our research. We chose the Midwest because it had several states within the top 10 states for Disc Golf Courses & they had the highest % of total Disc Golf courses within the US. 
Once narrowed we incorporated the median income & population density of the zip codes where these courses are located to identify the top states within the region to focus our advertising dollars. 
We narrowed our search using median income & number of Disc Golf courses. 
To help confirm we ran a regression analysis comparing population density & median household income against the number of Disc Golf courses. We found an increasing correlation between these metrics when comparing at the national, regional and state levels. 

## Results
Once the 7000+ Disc Golf locations in the United States were plotted it appeared that the Midwest was likely the strongest region for us to focus our attention. It had a high number of Disc Golf locations per state. Also, it was a geographically tight area of the country, allowing for the potential of future growth. 
When we then reviewed the top states in the midwest for median income & population density we found that Minnesota was in the top 3 for both lists. This is where we decided to narrow our focus, but we needed additional information to confirm that we made the right decision. 
In order to increase our confidence in Minnesota we performed regression analysis on the US, Region and then Minnesota. The confidence level increased as we narrowed down leading us to believe that we had made the right decision for PyWear. 
We then focused on the counties in Minnesota that had the largest number of courses and that led us to suggest that PyWear should start their advertising campaign in the Minneapolis/St-Paul metropolitan area. 

## Summary & Conclusions
Minnesota is our suggested area of focus for marketing spend because:

A. Total course count is one of highest in the US at 339

B. Variables of Interest are more correlated in MN compared to US 

|Population Density vs. Courses|R-value|
|------------------------------|------|
|US|0.335|
|Midwest|0.591|
|Minnesota|0.569|

|Income vs. Courses|R-value|
|------------------------------|------|
|US|0.264|
|Midwest|0.346|
|Minnesota|0.429| 

C. Within Minnesota - Focus on Minneapolis-St Paul Metro Area


## References & Acknowledgments
Data was sourced from the following:

|Resource files|Contents|Source|
|--------------|--------|------|
|DiscGolf.csv|Disc Golf course data|https://www.kaggle.com/datasets/lanekatris/pdga-united-states-disc-golf-courses|
|postcode_level_averages.csv|average income by zip code|https://www.kaggle.com/datasets/hamishgunasekara/average-income-per-zip-code-usa-2018|
|2010_and_2014_county_population_density.csv|Population density by county|https://odn.data.socrata.com/dataset/2010-and-2014-county-population-density/mmzq-86sd|
|Unemployment.csv|median household income by county|https://www.ers.usda.gov/data-products/county-level-data-sets/|
|FIPS_CODES.csv|County IDs for choropleth map|https://transition.fcc.gov/oet/info/maps/census/fips/fips.txt|

Additional information regarding Data Acquisition and Data Preparation is available in the README.md in the DataPrep directory.

We would like to thank the following mentors for their help throughout the data collection, analysis and presentation process:

Nick Sneed – Data Analysis Instructor

Ian Mac Moore – Teaching Assistant

Jonathan Fludd – Teaching Assistant

Shane Taylor - Teaching Assistant
