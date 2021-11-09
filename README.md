# Predicting-NYC-Illegal-Conversions

The goal of this project was to label buildings in New York City that are at high risk of an illegal conversion. An illegal conversion occurs when an existing residential or commercial building is altered or modified to create an additional room, space, or unit without first getting approval from the Department of Buildings (DOB). Illegal conversions therefore often do not complying with Building and Fire Code. Many deaths are caused by illegal conversions because the illegally converted room or unit is often located in a cellar or attic that lack a second egress to escape. Hurricane Ida caused eleven deaths in basement apartments, at least five of the apartments were illegally converted:
https://www.independent.co.uk/climate-change/news/new-york-apartment-flood-ida-b1914113.html

# Data
311 illegal conversion complaints routed to the DOB, DOB previous class one violations, DOB job filings, HPD multiple dwelling buildings, HPD multiple dwelling owners (contact list) and PLUTO.

# Model
Outcome variable: DOB vacate order on an illegal conversion complaint. A vacate typically occurs when the apartment has an inadequate or blocked egress, occupancy contrary to what is allowed by the law, or other hazardous conditions.

Independent variables: Independent variables included measures for building characteristics, previous bad behavior and location of the building. Variables include building classification, year built, building area, high or low rise, flag if multiple dwelling building, median income (based on location of building), whether building had a previous job filing (it was thought that a building is more likely to be an illegal conversion if there was no history of receiving a job filing),  text key word dummy variables based on the complaint notes (basement, attic, cellar, occupancy, FDNY), community board. 

# Results
The independent variables most correlated with a vacate issued on an illegal conversion complaint include building classification (1-2 family homes and walk up apartments), building area (<3000 square feet), location in the outer borough of Queens, year built between 1916 and 1937 and if basement or cellar occurred in the complaint notes. Previous class 1 violations and no history of job filings were only slightly correlated with a vacate order. 
