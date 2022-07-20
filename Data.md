### WNV surveillance data

Data consist of total annual neuroinvasive disease counts for counties in the 48 states (including the District of Columbia) within the contiguous United States from 2000–2018. The data were provided to registered participants in standardized csv files.

#### Data use

1. Access to ArboNET data is limited to team members named on the model submission form. The data provided will be treated as confidential and should not be provided to other persons. All other requests for access to ArboNET data should be directed to the CDC Arboviral Diseases Branch (<dvbid2@cdc.gov>). Comments or questions about the challenge should be directed to <vbd-predict@cdc.gov>.

2. The data are provided for the purpose of statistical reporting and analysis only, and may not be combined with other data or information for the purpose of matching records to identify individuals. Any information that could be used directly or indirectly to identify individuals will not be disclosed. If the identity of a person included in the data is discovered inadvertently, that information should not be disclosed or otherwise made public.

3. Analysis and reporting will be performed only on the variables and final data provided and should not be combined or compared to provisional data from the current or previous years.

4. Provisional data, other than that which is already publicly available, cannot be released.

5. The data provided, including any temporary or permanent files created from the ArboNET data, should be stored on a password protected computer. Copies of the data file(s) should not be made, even for back-up purposes. Hard copies of the data will be stored securely and shredded when they are no longer needed.

6. The team is responsible for obtaining Institutional Review Board (IRB) review of projects when appropriate.

7. ArboNET will be appropriately referenced in any publications or presentations that are derived from these data and a draft of the article or presentation will be provided to the CDC Arboviral Diseases Branch for review.


**Important notes about the data:**
+ In 2013, Bedford City, VA (FIPS 51515) was incorporated into Bedford County, VA (FIPS 51019). Historical data may have FIPS code 51515, while more recent data may have FIPS 51019. Only a prediction for Bedford County, VA (FIPS 51019) should be included in your forecast. Historical data for this county is reported as follows: 
	+ **fips:** 51019/51515 
	+ **county:** Bedford/Bedford City
	+ **location:** Virginia-Bedford City/Bedford

+ In 2015, Shannon County, SD (FIPS 46113) was renamed to Oglala Lakota County (FIPS 46102). Historical data may have FIPS code 46113 or the name Shannon County, while more recent data may use FIPS 46102 or the name Oglala Lakota County. Only a prediction for Oglala Lakota County, SD (FIPS 46102) should be included in your forecast. Historical data for this county is reported as follows:
	+  **fips:** 46102/46113
	+  **county:** Oglala Lakota/Shannon
	+  **location:** South Dakota-Oglala Lakota/Shannon

#### Data Dictionary

These data include annual counts of neuroinvasive West Nile virus disease cases reported to ArboNET by county. Each line represents all cases for a single county in a single year.

DESCRIPTION OF VARIABLES

**fips**

The five digit FIPS code, which includes the two-digit state code and the three-digit county code.
 
(Examples: 29099, 36005)

**county**

The name of the county where the case(s) resided, not including the word “county”.

(Examples: Jefferson, Bronx)

**state**

The name of the state that reported the cases. 

(Examples: Missouri, New York)

**location**

State and county for reported cases in the format State-County, there are no spaces between the state and hyphen, and the hyphen and county; but there are spaces between words in a state or county name, can be used to match the template or to submission file.

(Examples: Missouri-Jefferson, New York-Bronx)

**year**

The year (four-digits) the cases were reported.

(Examples: 2002, 2014)

**count**

Number of West Nile virus neuroinvasive disease cases reported.
