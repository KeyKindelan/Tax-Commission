# Tax-Commission
The New York City Tax Commission Reduced Values Unevenly

METHODOLOGY

The goal of this analysis was to compare the proportion of property tax reductions each borough received from the New York City Tax Commission, by how much each borough paid in property taxes.

The analysis of this data depended on the Sandeep Junnarkar's function to analyze the entire tax-roll of New York City. I downloaded the publicly available tax-roll for all tax classes from the city's Department of Finance page (https://www.nyc.gov/site/finance/property/property-assessments.page)   

Using Sandeep's function, the data was broken down into chunks so it could be accessed. 

Actual taxes paid per parcel depended on multiplying its total assessed value minus exemptions, by the property's tax rate. The city posts only four classes of tax rates, so I created a new column called taxed_amt that ran this calculation on each row.

When I compared a sample of ten to actual tax bills, the data was within $134.03. The actual tax bills could be based on a more recent assessment, or include additional exemptions. For the goal of this project, I felt this data was close enough. *

I summed the total taxed amounts per borough, summed the total reductions per borough, and combined them onto a data set together with a column dividing the total reductions by the total taxes. This gave me the proportion of tax dollars that get reduced per borough. 

The results showed that Manhattan property owners had 20 percent of property taxes reduced, the Bronx had six percent, Brooklyn 11 percent, Queens 10 percent, and Staten Island six percent.**



* I compared a sample of ten to actual tax bills, searching by the borough, block and lot. The sample changed when I re-ran it in the final notebook. Here are the initial results:

PARID		        Boro	Block	Lot	  MyResult	TaxBill		  Difference	  Comments
	
4067971435	    4	    6797	1435	$2966.63	$3,080.00	  113.37
4088830064	    4	    8883	64	  $8117.36	$8,117.36	  0		
2039442088	    2	    3944	2088	$1291.25	$1,223.28	  67.97		
3015160055	    3	    1516	55	  0		      0		        0		           Parkland
2039435135	    2	    3943	5135	$595.38		$595.40		  .02		
3072691081	    3	    7269	1081	$527.983	$553.72		  27.73
4726140011 176  4	    72614	11	  $5753.15  $1,140,663.20xxxx		       Verizon Utility - likely includes more lots 
4004081021	    4	    408	  1021	$454.50		$454.52		  .02
3044151476	    3	    4415	1476	$3377.50	$3,301.52	  75.98		
2039443001	    2	    3944	3001	$1544.25	$1,678.28	  -134.03		

The final_df taxed_amt estimates were within seven percent of the actual tax bill. The difference could be based on a more recent assessment, or include additional exemptions. For the goal of this project, I felt this data was close enough.

**
BORO  taxed_amt      REDUCTION      BoroReduction_Per_TaxedAmt  Boro Name	    Tax Commissioner  Expiration
			  
1	    1.668625e+10	  3.443159e+09	0.206347			              Manhattan	     Gary Bristol		  1/6/2030	
2	    2.835643e+09	  1.751189e+08	0.061756			              Bronx		       Vacant			      NA
3	    5.142249e+09	  5.754786e+08	0.111912			              Brooklyn	     Kirk P. Tzanides	1/6/2016	
4	    4.699267e+09	  4.760045e+08	0.101293			              Queens		     Vacant           NA 
5	    1.175646e+09	  7.138677e+07	0.060721			              Staten Island  Bennett Minko		1/6/2026

