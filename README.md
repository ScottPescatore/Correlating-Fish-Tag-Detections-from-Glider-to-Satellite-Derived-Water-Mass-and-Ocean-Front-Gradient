# Correlating Fish Tag Detections from Slocum Glider Missions to Satellite Derived Water Mass and Ocean Front Gradient
#### Code for Scott Pescatore's Thesis in the Masters of Operational Oceanography Program at Rutgers University
#
#
#
## Satellite Data is pulled from Thredds but can be accessed via ERDDAP
## 1-Day Aggregate is used in final analysis but compared to 3-Day Aggregate
#### Thredds: http://basin.ceoe.udel.edu/thredds/catalog/catalog.html
#### ERDDAP: https://basin.ceoe.udel.edu/erddap/griddap/index.html?page=1&itemsPerPage=1000
#
## Glider Mission Data is pulled from ERDDAP via Rutgers Glider Deployments Page
#### Glider Deployment Website: https://marine.rutgers.edu/cool/data/gliders/deployments/?type=deployments&filter=project_name&val=ECO-PAM 
#### (Filtered by project"ECO-PAM" which has 9 of the 10 missions used)
#### Final Mission is from RU28 Sep. 6th -  Oct. 11th, 2022 - Project: NJDEP
#### File paths should still work to each glider mission
#
## Tag Detection Data is in the form of CSV files with Qualified Tag Detections returned from Mid-Atlantic Telemetry Observation System (MATOS). Each CSV file contains all detections from all missions for the Project ECO-PAM each year from 2020 - 2022. The final CSV file contains all detections from a different project (NJDEP) for the ear of 2022.
#### Data Available Upon Request
#
## Tag Biometric Data was Collected by Contacting Tag Owners, Using the Contact and Tag Owner Information Provided with the Qualified Detection Data from MATOS
#### Data Available Upon Request
#
#
#
## Thesiscode1
##### This is my first iteration in correlating fish tag detections to water masses. I was able to grab the water masses with this code and make some basic histograms to explore the data. 
##### I then run the same code with 3-day aggregate satellite data to compare the results
#
#
#
##Thesiscode2
##### This was from when I was struggling to get the code in Thesiscode1 to work. It contains diagnostic images as well as explores the different datasets.
#
#
#
## Thesiscode5
##### This code creates visual representations of Glider paths and detections as well as showing detections over-layed on the water mass product. (The date I chose has the most unique tags detected in a single day that also has satellite coverage)
#
#
#
## Thesiscode4
##### Starting to get some better figures and incorporates the score of the strongest water gradient within 1-km and 5-km and also starts to incorporate biometric data on the tags (species)
#
#
#
## Thesiscode6
##### Finally the final code that incorporates everything and producing final figures. In addition to last iteration, I got the score of the closest water gradient to the detection above a threshhold of 1.5 and the distance to the gradient. I then divide the score by the distance to get an index score that relates to the strength of the correlation between the fish and ocean front. I also classify each mission as Stratified or Mixed by looking at their data. (Later: Stratification will be determined by using glider density, temperature, and salinity at time of the detection instead of entire mission/ More Figures will be generated in near future)  
