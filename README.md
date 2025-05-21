# Tax-Commission
The New York City Tax Commission Reduced Values Unevenly

METHODOLOGY

The goal of this analysis was to compare the proportion of property tax reductions each borough received from the New York City Tax Commission, by how much each borough paid in property taxes.

The analysis of this data depended on the Sandeep Junnarkar's function to analyze the entire tax-roll of New York City. I downloaded the publicly available tax-roll for all tax classes from the city's Department of Finance page (https://www.nyc.gov/site/finance/property/property-assessments.page)   

Using Sandeep's function, the data was broken down into chunks so it could be accessed. 

Actual taxes paid per parcel depended on multiplying its total assessed value minus exemptions, by the property's tax rate. The city posts only four classes of tax rates, so I created a new column called taxed_amt that ran this calculation on each row.

When I compared a sample of ten to actual tax bills, the data was within 7 percent of the actual tax bills. The actual tax bills could be based on a more recent assessment, or include additional exemptions. This could be a shortcoming of the analysis. 

I summed the total taxed amounts per borough, summed the total reductions per borough, and combined them onto a data set together with a column dividing the total reductions by the total taxes. This gave me the proportion of tax dollars that get reduced per borough. 

The results showed that Manhattan property owners had 20 percent of property taxes reduced, the Bronx had six percent, Brooklyn 11 percent, Queens 10 percent, and Staten Island six percent.


