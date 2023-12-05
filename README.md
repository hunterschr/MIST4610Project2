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

Graph 1:
  From a blank sheet, The Crime Code Description was inserted for our Columns, as a dimension. The Count of Crime Code measure was inserted as our rows in descending order, Bar Chart was selected, and results were filtered from all crimes to only those with 1500 or more instances, in order to display the most frequent criminal activities. Then, ‘Area name’ was inserted as a dimension as well, and we filtered our data down to only crimes reported in the ‘Central’ LA area to reduce the scope to just our target location. From this point, the Crime Code was added as a color marker in discrete dimension form, and the Crime Code Description was added in dimension form as a detail marker for the different column names to make the data more visually appealing and descriptive. This chart clearly represents the Count, of the most frequent crimes, above a certain threshold of 1500 reports, for only the ‘Central’ LA area, in descending order. 

Graph 2:
  From a blank sheet, ‘MONTH(Date Occ)’ is inserted as a discrete dimension for our columns in order to sequentialize our results by the different months of the year and reveal seasonal trends in criminal activity. The discrete Count of Crime Code measure is then inserted as our rows and filtered to only include values above 200 reports, so as to remain focused on our most frequent crimes. We then filter the results again by ‘YEAR(Date Occ)” discrete dimension and select ‘All’ in order to display results from every year that we have data. The results are filtered again by ‘Area Name’ to only include data from the ‘Central’ LA area. The results are filtered again by the Crime Code Description as a dimension to produce the individual trend lines for our chart. Finally, the Crime Code Description dimension is used as a color marker to make the graph more visually appealing. The resulting discrete lines chart clearly displays the average Count of crimes reported, per month, in the ‘Central’ LA area, across 4 years, for only those crimes which have above 200 reports in a month. 



### Question #2: 

  The main data manipulations for question 2 were within the *Difference in Crime Occurence between Genders* graph. The difference in crime frequency between genders was calculated by subtracting the number of victims of one gender from the number of victims of the other gender for each crime type. This calculation is stored in a calculated field named ``[GenderDiff]`` which is shown beneath the total number of occurences of each crime for each gender. 
  
  The only data manipulation used in the *List of Crimes with Average Age of Different Genders* graph was converting the victims' ages into averages instead of a sums.




## Analysis and Results:
Analyze and visualize the results of your analysis and describe the implications of your analysis.
Please provide any citations if required as well as supporting visualizations and analysis
generated from Tableau.

### Question #1: 

Understanding the average age of each crime and the frequency of the crime changes based on gender is a great question for this kind of data. It allows you to look at it and compare the data in Tableau and figure out how Los Angeles is from a crime rate perspective. This can also be something used in the police department because this gives information about each gender and the amount of cases that occurred throughout the year and gives information in numbers and is organized based on a bar graph from least to greatest. I believe this is a great way to look at information like this because it gives every crime that occurred, the gender, the place and any other details that need to be specified.


For example, one can see that for the Central region of LA, burglary from vehicles is the most common crime and for Hollywood, simple assault battery is most prevalent. The most common crime, interestingly, for all of LA is stolen bikes. This data can help the city and the police track crime and also take precaution to address and mitigate these crimes.

<img width="958" alt="Screenshot 2023-12-05 at 10 33 37 AM" src="https://github.com/hunterschr/MIST4610Project2/assets/148081356/b7d742a6-4577-4719-b64a-234ff0b29e5b">



 In conclusion to this question, this information can be something that helps many people and allows them to learn a lot based on the tables. This is something can can benefit the police department and it will help them keep everything organized.

### Question #2: 

Understanding the average age of victims for various crimes and the disparities in crime frequency based on gender reveals important insights with wide-ranging effects. Firstly, this data allows for targeted prevention strategies. By identifying the average age groups affected by specific crimes, specific initiatives can be designed, such as educational programs for youth or teens to prevent crimes like resisting arrest or pandering. Additionally, recognizing gender-based differences in crime frequency helps in resource allocation, allowing support services and protection measures towards the more vulnerable gender for certain crimes, like support for females affected by credit card fraud or males when it unfortunately comes to lynchings. (See below for comparisons)

![image](https://github.com/hunterschr/MIST4610Project2/assets/148078185/a66d8ae9-53f7-42db-b3b9-0cead1e38bf9)

![image](https://github.com/hunterschr/MIST4610Project2/assets/148078185/342e7c19-7f4b-4b0b-9a4f-7c28dd6c523f)


For example, simple assault battery is a very prevalent crime in the data. Though both females and males have committed this crime over 30,000 times each, males have committed it about 4,000 more times. The victims of this crime, male and female, are on average about 40 years old. Data like this is shown for each crime, which allows for preventive action to be taken.

<img width="989" alt="Screenshot 2023-12-05 at 10 35 57 AM" src="https://github.com/hunterschr/MIST4610Project2/assets/148081356/d205ab3c-9bbf-4c10-8934-4055333f1b80">



Furthermore, these findings inform policy making and law enforcement strategies. Policymakers can create more effective policies concerning the needs of specific demographic groups impacted by different crimes, while law enforcement agencies can change their approaches based on victim demographics, adjusting patrolling or investigative efforts accordingly. This data also emphasizes social awareness and education, creating campaigns that educate communities about safety measures, legal rights, and available resources for specific demographics. Overall, these insights highlight the need for a targeted approach to crime prevention and victim support, considering the diverse demographic characteristics of crime victims.

## Completed Tableau Workbook
[Team Name: 29704 3](https://drive.google.com/file/d/1ahjPNhCLhfTBLJsfvPv9hkGLXPYOUFab/view?usp=share_link)
