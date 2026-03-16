This repository (repo), contains the "2022 Vessel Profit Snapshots" site produced by the NEFSC Social Sciences Branch. 

Who worked on this project: The project team consists of Social Sciences Branch staff members [Greg Ardini](https://www.fisheries.noaa.gov/contact/greg-ardini), 
[Samantha Werner](https://www.fisheries.noaa.gov/contact/samantha-werner), and [Elizabeth Conley](https://www.fisheries.noaa.gov/contact/elizabeth-conley).

When this project was created: This project commenced following implementation of the Greater Atlantic Region Commercial Fishing Business Cost Survey for 2022. 
The project repo was finalized in March 2026.

What the project does: The website housed in this repo first provides background on the Greater Atlantic Region Commercial Fishing Business Cost Survey, fielded by the Social Sciences Branch of the Northeast Fisheries Science Center. 
Next, the metrics presented on the site are discussed along with the protocol for filtering survey responses for use on the site. 
Methods for calculating the metrics are then discussed, followed by fleet revenue and cost summaries. 
Finally, operating profit, total profit, and profit margins are presented by both primary gear and fishery. 
The site focuses on the 2022 calendar year- the most recent year for which cost information is available within the Northeast region.

Why the project is useful: Vessel-level profits have not previously been calculated for commercial fishing fleets in the Northeast region.
The information provided in this site can be helpful to fishery managers and stakeholders in understanding how gross revenues translate to profits.

How users can get started with the project: The website found in this repo provides a fair amount of detail on the Greater Atlantic Region Commercial Fishing Business Cost Survey.
Additional information can be found on the [Cost Survey Landing Page](https://www.fisheries.noaa.gov/new-england-mid-atlantic/commercial-fishing/commercial-fishing-business-cost-survey).
Cost distributions are available on the [Cost Data Visualization Tool](https://apps-nefsc.fisheries.noaa.gov/cost-data/). The repo contents are summarized below to help users navigate the various repo folders.

Where users can get help with the project: For questions on the contents of this repo, please reach out to Greg Ardini.

Who maintains and contributes to the project: This repo is maintained by Greg Ardini with contributions by Samantha Werner and Elizabeth Conley.


Repo contents:

The full code to generate the site is available in the index.Rmd file. For smaller segments of code, see the intro_methods_1, revenue_cost_2, profit_3, and discussion_4 Rmds.

The following folders are available in this repo:

scripts_to_generate_input_files: SAS scripts are listed in sequential order. 

Retrieve_revenue: Generates vessel-level commercial, for-hire, and total revenue. 
Vessels are grouped into primary gear and fishery based on the largest source of revenue.

Retrieve_survey_cost: Generates vessel-level costs using data collected in 2022 Commercial Fishing Business Cost Survey.

Retrieve_supplies_water: Generates vessel-level estimates of costs not collected in the 2022 Commercial Fishing Business Cost Survey. 
These costs (crew supplies and water) are estimated from at-sea observer data.

Retrieve_depreciation: Generates vessel-level depreciation costs using estimated vessel market values. 
A hedonic model is used to estimate market value as a function of various vessel characteristics such as age, horsepower, length, and tonnage.

Filter_observations: Filters responses from the 2022 Commercial Fishing Business Cost Survey to determine if adequate information was provided to calculate vessel profits. 

Final_combine: Merges datasets generated in scripts #1-4 and retains observations based on script #5. All .csv files that are read in to the RBookdown code are generated.

input_files: csv files produced from the SAS script, "6_final_combine"

docs: figures for the site are contained within the SSB_Profit_Profiles_files/figure-html sub-folder.

references: Includes links to all papers referenced in the site.


*This repo was initially generated from a bookdown template available here: https://github.com/jtr13/bookdown-template.*

**This repository is a scientific product and is not official communication of the National Oceanic and Atmospheric Administration, or the United States Department of Commerce. 
All NOAA GitHub project code is provided on an ‘as is’ basis and the user assumes responsibility for its use. 
Any claims against the Department of Commerce or Department of Commerce bureaus stemming from the use of this GitHub project will be governed by all applicable Federal law. 
Any reference to specific commercial products, processes, or services by service mark, trademark, manufacturer, or otherwise, does not constitute or imply their endorsement, recommendation or favoring by the Department of Commerce. 
The Department of Commerce seal and logo, or the seal and logo of a DOC bureau, shall not be used in any manner to imply endorsement of any commercial product or activity by DOC or the United States Government.
