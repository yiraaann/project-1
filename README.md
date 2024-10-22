# Project-1 | Chicago Infrastructure: Deficits & Disparities

## Team Members
- Michelle Moody: Project report, graffiti & pothole analysis, final Jupyter notebook
- Wayne Mitchell: EDA, clean all csv files, statistical tests, linreg figures
- Yiran Zhang: CSV pulls, vacancy analysis, repo clean, README, slide deck
- Deidra Lebron: Crime graphic, pothole research

## Introduction
This project came about from a mutual interest in the City of Chicago's crime reports. Our team wanted to take a deeper look at the possible variables associated with crime in our city and their connections to other factors of interest such as infrastructure, locations, ward spending, etc. We sought to answer the question, "Do areas with a higher concentration of infrastructure issues also report higher crime rates?"

## Executive Summary
Infrastructure issues, such as unrepaired potholes, malfunctioning streetlights, and neglected or littered vacant lots, often reflect deeper problems of neglect and underinvestment in a community. These visible signs of disrepair can create environments that feel less secure and welcoming, potentially weakening community bonds and affecting economic activity. Such conditions may also signal to residents and outsiders that an area receives less attention and maintenance, which can influence crime rates. The "Broken Windows Theory" in policing suggests that visible signs of neglect, like poor infrastructure, can give the impression of disorder, leading to minor offenses that may escalate into more serious criminal activity. The concept implies that addressing minor issues or managing infrastructure concerns in a particular ward might help prevent a rise in crime.

The datasets that we examined looked at crime trends over the past five years, coupled with data on infrastructure service requests.  We understand that the trends could possibly be influenced by the effects of COVID-19, as the pandemic significantly altered social behavior and patterns. During lockdowns and periods of restricted movement, certain types of crime, such as burglaries and street crimes, saw a decline due to fewer people being out and about. Conversely, other crimes, like domestic violence, may have increased as people were confined to their homes. Additionally, changes in economic conditions, such as job losses and business closures, could have impacted crime rates, leading to variations that are atypical when compared to pre-pandemic years. Therefore, any analysis of crime during this period should take into account the unique conditions and disruptions caused by the pandemic.

## Project Objectives
- What does it do? Our project takes a close look at the correlation between crimes reported in Chicago and 3 types of infrastructure service requests (graffiti, potholes, vacant buildings/lots) on a ward-by-ward basis.
- Who is the audience? Our broad audience consists of community activists, alderpersons, concerned community members, potential homebuyers, and real estate industry actors.
- What problem does it solve? Our project seeks to bring awareness to the reported infrastructure issues within the city and their correlation with reported crimes. This type of analysis can inform more targeted and effective spending priorities for bringing down crime rates while investing in neighborhood infrastructure: a win-win for the city's residents and decisionmakers.

## Data Sources
- Chicago Crime Database (January 1, 2019 - October 10, 2024) [https://data.cityofchicago.org/Public-Safety/Crimes-2001-to-Present/ijzp-q8t2/]
- Chicago 311 Service Call Database (January 1, 2019 - October 10, 2024) [https://data.cityofchicago.org/Service-Requests/311-Service-Requests/v6vf-nfxy/]
- Geoapify API [https://www.geoapify.com/places-api/]
- City of Chicago Ward Spending [https://www.wardwisechicago.org]

## Instructions
- set timeline boundaries for both the Crime and the Chicago 311 databases
- filter the full 311 database for service requests of interest (using keywords such as "streetlight," "rat," or "pothole")
- export the data in csv format according to timeline and subject matter for ease of use
- clean the data by eliminating unnecessary columns. minimum columns needed: "WARD" "SR_TYPE" "CREATED_DATE" "LATITUDE" "LONGITUDE"
- make sure os, pathlib, numpy, pandas, hvplot.pandas, matplotlib.pyplot, scipy.stats, requests, time, gc, and your geoapify key are all imported
- further clean the data by analyzing which rows of "null" values to drop
- merge the data into a single dataframe using pd.merge
- determine number of service requests per ward, number of crimes per ward
- sort each list descending by highest number of crimes or service requests and plot in bar graph or other meaningful visual
- compare, ward by ward, crime with service request type of choice to determine linear regression values

## Happy Analyzing!
