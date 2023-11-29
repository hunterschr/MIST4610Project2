# Team 3 Mist 4610 Group Project 2 

## Team Name:
29704 3

## Team Members:
#### 1. Hunter Schramm [@hunterschr](https://github.com/hunterschr)
#### 2. Will Hensley  [@Willhens15](https://github.com/willhens15)
#### 3. Shweta Sainathan [@ShwetaSainathan](https://github.com/ShwetaSainathan)
#### 4. Aidan Davies [@aidan.davies@uga.edu](https://github.com/AidanDavies117)
#### 5. Lauren Prisock [@laurenPrisock](https://github.com/laurenPrisock)
#### 6. Sohum Rane [@srane05](https://github.com/srane05)

## Describing your dataset and what data it contains:
Where was it obtained, what are the dimensions of it (rows and columns), what are the various
columns, data types, etc. Describe it in sufficient detail so that an uninformed reader would
understand the dataset.

Data Obtained From: https://catalog.data.gov/dataset/crime-data-from-2020-to-present
Data Set: Crime Data From 2020 to Present
Data Set Description: Represents crime in the City of Los Angeles from 2020 to now.

Data:
| Column Name  | Data Type | Description |
| ------------- | ------------- | ------------ |
| Dr No | NUMBER | Primary Key, unique identifier for each instance of a crime |
| Date Rptd | DATETIME | the date that the crime was reported to the Los Angeles Polic Department |
| Date Occ | DATETIME | the date that the crime actually took place | 
| Time Occ | NUMBER | this gives the time (in 24-hour military time) that the crime occurred |
| Area | NUMBER | gives the location of the crime in the form of a number that is unique to an area of Los Angeles (similar to a zip code)|
| Area Name | TEXT | gives the name of the unique area where the crime occurred |
| Rpt Dist No | NUMBER | a 3-4 digit code that represents a sub-area within an area of Los Angeles, gives a more precise location of the crime |
| Crm Cd | NUMBER | indicates the crime committed| 
| Crm Cd Desc | TEXT | describes the crime committed, corresponds to Crm Code |
| Mocodes | TEXT | Modus operandi, activities associated with the suspect in commission of the crime |
| Vict Age | NUMBER | gives age of the victim |
| Vict Sex | TEXT | gives gender of the victim (M-male, F-female) |
|Vict Descent | TEXT | Descent Code: A - Other Asian B - Black C - Chinese D - Cambodian F - Filipino G - Guamanian H - Hispanic/Latino/Mexican I - American Indian/Alaskan Native J - Japanese K - Korean L - Laotian O - Other P - Pacific Islander S - Samoan U - Hawaiian V - Vietnamese W - White X - Unknown Z - Asian Indian |
| Premis Cd | NUMBER | gives the code that corresponds to the type of location the crime took place (vehicle, car, etc) |
| Weapon Used Cd | NUMBER | code for type of weapon used in the crime |
| Weapon Desc | TEXT | description of weapon used |
| Status | TEXT | status of the case| 
| Crm Cd 1-Crime Cd 4 | NUMBER | Indicates the crime committed. Crime Code 1 is the primary and most serious one. Crime Code 2, 3, and 4 are respectively less serious offenses. |
| Location | TEXT | gives exact street address of incident|
| Cross Street | TEXT | gives nearest street of rounded address|
| LAT | NUMBER | Latitude |
| LON | NUMBER | Longitude |


## The 2 questions the team generated and why they are interesting and important:
What are the questions, and why each question is important. Importance can be evaluated and
conveyed in a variety of ways including, social, economic, cultural and other factors. Also
indicate how they are tied to the data set or sets being used.

## The manipulations applied to the data set as part of the analysis:
Were there any manipulations or calculations that needed to be performed on the data, what were
they, describe the purpose and how they were accomplished.

## Analysis and Results:
Analyze and visualize the results of your analysis and describe the implications of your analysis.
Please provide any citations if required as well as supporting visualizations and analysis
generated from Tableau.

## Tableau Packaged Workbook
Save or Export your project as a Tableau packaged workbook file and provide it as part of the
github repository
