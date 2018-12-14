# H1-B-Processing-Likelihood of LCA Applications

This project works to build a model that can predict the likelihood of a LCA application being accepted based on all the parameters that the USCIS accepts as part of the application

## Pre-requisites to an H1-B Application

• Before filing H1B application, organizations have to file an LCA (Labor Condition Application)

• LCA is required to prove an immigrant worker is required for job – candidates can be rejected at this phase

• No lottery, LCA decisions are completely human centric and determined by immigration officer

• Since the LCA process is manually determined and is not subject to a lottery, it is completely objective

## Data and Variables Considered

“H-1B_Disclosure_Data” is available for the years 2011-2018 in the USCIS website, documenting all the applications submitted for the LCA procedure in the given period.
Combining these datasets, a cumulative database consisting of *3 million rows* with 34 variables was created.

13 variables were selected from these that would aide in the analysis and model
creation. 

Cleaning the data to remove rows with missing values (N/A) resulted in a total of 1.6 million rows.

The 13 variables specifically used for this analysis are-

* **'CASE_STATUS'** - Status associated with the last significant event or decision. Valid values
include “Certified”, “Certified-Withdrawn”, “Denied”, and, “Withdrawn”

* **'VISA_CLASS'** - Indicates the type of temporary application submitted for processing. R = H-1B; A = E-3 Australian; C = H-1B1 Chile; S = H-1B1 Singapore. Also referred to as “Program” in
prior years.

* **'EMPLOYER_NAME'** - Employer’s name

* **'JOB_TITLE'** - Job Title

* **'SOC_CODE'** - The Standard Occupational Classification (SOC) code which classifies workers by
occupational groups

* **'SOC_NAME'** - Title of the SOC occupational group

* **'FULL_TIME_POSITION'**- Y = Full time; N = Part time position

* **'PREVAILING_WAGE'**- The present wage rate on offer

* **'PW_UNIT_OF_PAY'** - The unit of pay for the wage. Yearly or Hourly.

* **'H1B_DEPENDENT'** - Y’ if dependents exist, ‘N’ otherwise.

* **'WILLFUL_VIOLATOR'** - Whether employers who have committed either a willful failure or a misrepresentation of a material fact when hiring foreign workers

* **'WORKSITE_STATE'** - Location (state) associated with the present position.

* **'YEAR'** - Year at which the LCA was filed
