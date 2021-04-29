## Introduction

I was tasked with creating a capstone project that included: the compilation of data, analyzing the data, and providing actionable insights. In this project, I was tasked with exploring Tennessee's high school graduation requirements with median household income and  personal bankruptcy filings. When going through the data set I wanted to highlight trends to support an increase to Tennessee's graduation requirement for Personal Finance and target areas in which this could be done. For this project I used Excel and Python for data analysis and PowerPoint for data visualization.

Data Sources:  
[Bankruptcy Data](https://www.uscourts.gov/report-name/bankruptcy-filings)  
[Income Data](https://www.census.gov/)
[Schools Data](https://k-12.education.tn.gov/sde/)  
[Donate Here](https://www.donorschoose.org/donors/search.html?state=TN&cityName=Memphis&countyName=Shelbycounty&centerLat=35.1495&centerLng=-90.0490&includeNearbyLocations=true&gradeType=4)  
[More Classes Here](https://www.ramseysolutions.com/)  

## Proposal

[Proposal Document](data/Proposal.pdf)

## Table Of Contents

* [Introduction](#introduction)
* [Proposal](#proposal)
* [Table of Contents](#table-of-contents)
* [Data Question](#data-question)
* [Deliverables](#deliverables)
* [Tools Used](#tools-used)
* [Parameters](#parameters)

## Data Question

What areas in Tennessee should be targeted for adding additional financial literacy courses to its high school curriculum?

## Deliverables

* Top 3 Counties to target
* 10 High Schools to start with

## Challenges/ Rewards

Just like every good war we can't foget to skip over the battles, because they too are important. The challenges with this project came before the war, in cleaning the data. I ran into issues with the different data sources in first cleaning up my key column to merge the data sets on just the county name. It required a lot of string manipulation, creation of columns, and deletion of columns. The next problem came with webscrapping google maps api to geocode the addresses for the schools to be able to visually show location of the different schools in my geospatial environment. I made the address column by concatenating columns together to format the addresses in a format google maps could recognize. I was able to define a function to grab the longitude and latitude locations of each school, however some address that ended in Pike or were on streets called "Hwy" were not recognized, so additionally I had to manipulate my function and search and find those errors to manually adjust those addresses and obtain their geocode. The last problem I ran into came far down the road in to the project when I realized that data form Hamblen County was missing. I then discovered that there was an error with the actual data from the site in which the site had Hablen County spelled as "Hamblem". This was easy to correct, but a pain to see. Despite all of the challenges I faced over the data cleaning process I think it was rewarding to go through the experience becuase nothing is more real than spending more time cleaning than you though, using a plethra of different languages when walling in others, or having "fat finger data". Those battles added an extra layer of fun to this project war. 

## Tools Used

* Python  
  * geospatial environment
* Excel
* PowerPoint

## Parameters

Limited Analysis to Public and Private High Schools  
Excluded Home Schools, Homebound Schools, and Public Charter Schools  
