# Education_and_Taxes
Analyzing IRS data to determine if areas with greater educational (early learning through college) opportunities correlate with electronic filings with focus on Indiana. 

## Datasets used: 

Public Schools (early learning - grade 12): https://www.kaggle.com/carlosaguayo/usa-public-schools

IRS: https://www.irs.gov/statistics/soi-tax-stats-individual-income-tax-statistics-zip-code-data-soi

College/University: https://www.registrar.iastate.edu/sites/default/files/uploads/codebook/bystate.pdf

## Transformation: 

Cleaned data sets to focus strictly on Indiana and for the year 2018 with the exception of public school set, which is defined as being 2014-2015 school year. Census API was used to find population data to compare with tax filings reported by the IRS. College/University had to be transformed from pdf to excel to be reorganized and cleaned up. Google Geocode was used to obtain the zip code for the college/university as this was not originally included by getting the latitude and longitude of each city. St Mary-of-the-Woods, North Manchester University, and Ancilla College showed up as NaN when obtaining Lat and Lng coordinates. To not loose these colleges as part of the data set, the data was exported to a new CSV file and these coordinates were entered manually to finish obtaining zip code for all college/universities. All cleaned data was exported to a new, cleaned csv file: Indiana_k12.csv, _____, ____. 

### Languages Used: 
<li>pandas
<li>matplotlib
<li>sqlalchemy
<li>json

## Analysis: 
In Indiana, there are ____ zip codes total per the IRS, 517 unique zip codes that has PK-12 schools, ____ unique zip codes that have colleges or universities, and ___ that has both grade level and college/university level schools.




## Drawbacks:

Data for taxes and census is for 2018. The public school data is for 2014 only; however, it is assumed there has been no school closings or openings within that time period. It is also unknown how many people did not file taxes for reasons such as malicious intent or incapability.  

## Contributors:

<li> Andy: https://github.com/andyob715
<li> Jake: https://github.com/JakeRose689
<li> Stacey: https://github.com/staceyj118
