# Education_and_Taxes
Analyzing IRS data to determine if areas with greater educational (early learning through college) opportunities correlate with electronic filings with focus on Indiana. 

## Datasets used: 

Public Schools (early learning - grade 12): https://www.kaggle.com/carlosaguayo/usa-public-schools

IRS: https://www.irs.gov/statistics/soi-tax-stats-individual-income-tax-statistics-zip-code-data-soi

College/University: https://www.registrar.iastate.edu/sites/default/files/uploads/codebook/bystate.pdf

Census Data: https://www.census.gov/data/developers/data-sets.html & GitHub - datamade/census: A Python wrapper for the US Census API.

## Transformation: 

Cleaned data sets to focus strictly on Indiana and for the year 2018 with the exception of public school set, which is defined as being 2014-2015 school year. Census API was used to find population data to compare with tax filings reported by the IRS. College/University had to be transformed from pdf to excel to be reorganized and cleaned up. Google Geocode was used to obtain the zip code for the college/university as this was not originally included by getting the latitude and longitude of each city. Data for 2018 taxes in Indiana were downloaded and cleaned using Pandas.  

### Languages Used: 
<li>pandas
<li>matplotlib
<li>sqlalchemy
<li>json
<li>scipy.stats

## Analysis: 
In Indiana, there are 674 zip codes with available IRS data, 517 unique zip codes that have PK-12 schools, 53 unique zip codes that have colleges or universities, and 47 that have both grade level and college/university level schools. 

There were 6,211,130 total tax returns filed: 5,706,720 electronically and 260,120 paper (computer prepared). Out of all the returns, 3,007,160 were submitted by paid preparers and 108,070 by volunteers. Direct deposits were received on 4,205,260 of the returns. Returns accounted for a total of 11,866,510 persons, 3,783,260 of which were dependents.




## Drawbacks:

<li>Some people do not file taxes, which could not be accounted
<li>Data for taxes and census is from 2018
<li>Data from public schools was 2014 – it is assumed not significant changes
<li>Data from colleges/universities was a recent list, exact year unknown

## Contributors:

<li> Andy: https://github.com/andyob715
<li> Jake: https://github.com/JakeRose689
<li> Stacey: https://github.com/staceyj118
