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

## Description of Dataset:

Data Obtained From: https://catalog.data.gov/dataset/crime-data-from-2020-to-present

Data Set: Crime Data From 2020 to Present

Data Set Description: Represents crime in the City of Los Angeles from 2020 to now.

### Data:
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


## Research Questions:

### Research Question #1: 
### What types of crimes are most commonly reported in different areas, and during which time of the year do they tend to occur most frequently?

Understanding the prevalent types of crimes in various areas and identifying the peak times of the year for these occurrences is crucial for the Los Angeles Police Department. This information aids in strategic officer stationing, ensuring a more targeted and effective law enforcement approach. For instance, if the Central area of Los Angeles experiences a higher crime rate compared to the Hollywood area, allocating more officers to the central region becomes a priority. Additionally, analyzing this data unveils patterns indicating the months with elevated overall crime rates in specific areas.



### Research Question #2: 
### What is the average age of the victims of each crime, and how does the frequency of crime differ based on gender?

Understanding the average age and typical gender of a victim within a crime is crucial for the Los Angeles Police Department in determining what attributes offenders look for. This information can be used to help aid the community in being more vigilante if they fall within one of these categories. 


## Dataset Manipulations:

### Question #1:

  Filter the results from all crimes to crimes with 1,500 or more instances.


### Question #2: 

  The difference in crime frequency between genders was calculated by subtracting the number of victims of one gender from the number of victims of the other gender for each crime type. This calculation was stored in a calculated field named ``[GenderDiff]``.




## Analysis and Results:
Analyze and visualize the results of your analysis and describe the implications of your analysis.
Please provide any citations if required as well as supporting visualizations and analysis
generated from Tableau.

### Research Question #1: 
### What types of crimes are most commonly reported in different areas, and during which time of the year do they tend to occur most frequently?

Understanding the prevalent types of crimes in various areas and identifying the peak times of the year for these occurrences is crucial for the Los Angeles Police Department. This information aids in strategic officer stationing, ensuring a more targeted and effective law enforcement approach. For instance, if the Central area of Los Angeles experiences a higher crime rate compared to the Hollywood area, allocating more officers to the central region becomes a priority. Additionally, analyzing this data unveils patterns indicating the months with elevated overall crime rates in specific areas.



### Research Question #2: 
### What is the average age of the victims of each crime, and how does the frequency of crime differ based on gender?

Understanding the average age and typical gender of a victim within a crime is crucial for the Los Angeles Police Department in determining what attributes offenders look for. This information can be used to help aid the community in being more vigilante if they fall within one of these categories. 

## Tableau Packaged Workbook
Save or Export your project as a Tableau packaged workbook file and provide it as part of the
github repository
