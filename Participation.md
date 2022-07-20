### Participation guidance

**How to participate**

To participate in the challenge, one team member must register on the predict.cdc.gov website and, after logging in, register specifically for the 2020 WNV Forecasting Challenge. The forecast submissions are connected to this account. Only one set of forecasts is allowed per account and only one account per set of forecasts (i.e. the same account must be used for all submissions).

Full participation requires:

1.	Electronic submission of forecasts for all included counties by the initial deadline (details below and [Evaluation](Evaluation.md) page).

2.	Submission of a model description document by email (See below).


### Forecast submission

**Forecast format**

Forecasts should be made in csv files matching the format in this [template](WNV_forecasting_template.csv). Each csv should contain forecasts for all counties (n= 3,108). For internal record keeping, teams may find it useful to include the forecast due date or submission date in the file name. Due to county name and FIPS code changes, some counties may not appear exactly the same in this template as they do in the historical data. Only forecasts for counties that exist in 2020 are required. See the **Data** page for more information.

The forecast file includes a set of lines for each forecast representing binned probabilities for the range of outcomes. Each bin is defined by an inclusive minimum and a non-inclusive maximum, for example, the bin defined by `bin_start_incl` = 1 case and `bin_end_notincl` = 6 cases is assigned the probability that the number of cases is greater than or equal to 1 and less than 6 (i.e. 1, 2, 3, 4, or 5 cases are reported, 1 <= x < 6). The following set of bins are used for each forecast: 0 <= x < 1, 1 <= x < 6, 6 <= x < 11, ..., 46 <= x < 51, 51 <= x < 101, 101 <= 151, 151 <= 201, 201 <= 1000. Each of these bins should have a probability between 0 and 1.0 (inclusive) and the sum of the probabilities assigned to each set of bins for one county should be 1.0. The forecast file also includes a line for each forecast representing the point prediction i.e. the most likely outcome for the specific target. A value for point prediction is required for submission; however, the point prediction will not be evaluated for this challenge. 

Each row in the submission file represents a single bin and includes the following columns:

**location**: “State” and “County” as written in the data files with a hyphen: “State-County”. For example, “California-San Diego” or “Texas-Harris”. Do not include the word “County” and include spaces between words within the county or state name. The easiest way is to accomplish this is by matching the template available above to the input data. 

**target**: “Total WNV neuroinvasive disease cases”

**type**: “Bin” or “Point”. “Bin” specifies that the prediction is for a bin covering a range of possible outcomes. “Point” specifies the total predicted cases but will not be evaluated. 

**unit**: “cases“

**bin_start_incl**: The inclusive lower bound for the bin, e.g. 0, 1, 6, 11, …, 151, 201.  

**bin_end_notincl**: The non-inclusive upper bound for the bin, e.g. 1, 6, 11, 16, …, 201, 1000.

**value**: A probability for the number neuroinvasive disease cases in the bin defined by `bin_start_incl` and `bin_end_notincl`. This probability should be greater than or equal to 0 and less than or equal to 1.0 for all bins per county. Value for ‘point’ predictions can be zero or any positive integer and must be present but will not be evaluated for this challenge. 

[Download Template](WNV_forecasting_template.csv)

**Submission process**

Registered participants will have access to a **Submit** page. The individual csv files can be uploaded on that page any time before the specific deadlines. The submission format will be automatically validated when the forecast is uploaded. Forecasts will be made for all of 2020 and initial forecasts will be due on April 30. Updated forecasts may be submitted by May 31, June 30, and July 31, 2020. Updated forecasts may use newly acquired data or updated methods, but are not required. Forecasts may be submitted and updated at any time prior to the due date. Successful submission can be checked by click on the “Open JSON” link (the JSON format is a format used by the server).


**Model description**

The initial forecast submission should be accompanied by a completed [Model description form](WNV_forecast_model_submission_form.docx) submitted by email to the organizers (<vbd-predict@cdc.gov>). If updates are made to the model for subsequent forecasts, an updated model description should be provided to the organizers.

[Download Model description form](WNV_forecast_model_submission_form.docx) 
