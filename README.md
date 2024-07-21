# Factors That Minimize Injuries in Car Crashes in Montgomery County, MD
## by Koty Potts, Jack Runge, and Nicole Henderson

### Introduction
This project aims to analyze public crash report data in Montgomery County, MD from January 1 2015 to December 31 2023.
The goal of our analysis was to uncover insights into various factors that influence the severity of injuries sustained 
in car crashes and to propose recommendations for enhancing road safety.

The factors that we studied were:
1. Environmental factors, including speed limit and date of crash
2. Driver conditions, including alcohol and driver at-fault
3. Vehicle conditions, including vehicle make and year

#### Data Source
From data.gov, a csv that holds records of around 170,000 accidents in Montgomery County, MD from 2015 to 2023. <br/>
[https://catalog.data.gov/dataset/crash-reporting-drivers-data](https://catalog.data.gov/dataset/crash-reporting-drivers-data) <br/>
![Project1ListColumns](https://github.com/user-attachments/assets/e78a5e3c-5a45-4b59-8959-b9f161157f7d) <br/>
![Project_1_columns](https://github.com/user-attachments/assets/13ac12ac-4227-4001-906b-30b398a7fb4e)

### Results
1. Most injuries occurred between 35 and 40 mph.<br/>
![SpeedLimit_Injuries](https://github.com/user-attachments/assets/16d58f74-73ba-485e-96a1-c820067586fb) <br/>
A chi square test indicates that there is a strong relationship between 35mph and total injury

2. A sharp increase in average injury severity occurs at higher speeds, 60mph being the most dangerous speed <br/>
![SpeedLimit_AvgInjurySeverity](https://github.com/user-attachments/assets/db5db578-d0a6-467b-a00c-4c768a4c9f54) <br/>

3. Total number of injuries tend to spike towards the end of the year <br/>
![TotalInjuries_Date](https://github.com/user-attachments/assets/5fb55d80-01c9-4859-9b61-33af0c05cbc1) <br/>

4. April and May have the highest average injury severity <br/>
![Month_InjurySeverity](https://github.com/user-attachments/assets/2ec379ac-5778-40a1-b9d0-df30d648edbc) <br/>

5. Percentage of accidents involving drugs and/or alcohol increases for accidents with serious injury <br/>
![PercentageAlcohol_All](https://github.com/user-attachments/assets/9d0e2a35-133e-48c7-a7a4-6033794f6e43)![PercentageAlcohol_SeriousInjury](https://github.com/user-attachments/assets/51df7089-b610-4787-9afb-08eb23228b03) <br/>
A chi square test indicates there is a relationship between alcohol and accidents resulting in serious injury

6. There is a relationship between the severity of the injury and the driver being at fault <br/>
![Driver-at-fault_InjurySeverity](https://github.com/user-attachments/assets/c504c03b-3845-4bb8-a032-2f2949b164d7) <br/>
A chi square test indicates there exists a relationship between driver being at fault and the severity of the injury

7. The 2 vehicle makes most commonly involed in accidents were Hondas and Toyotas <br/>
![VehicleMake_TotalSeriousFatalInjury](https://github.com/user-attachments/assets/db2f8108-8477-43ef-a431-375e2d6c3cdb) <br/>
A chi square test indicates that the relationship between driving a honda and toyota and injury severity was significant <br/>
    * Note: these also happen to be the most commonly driven cars, so it makes sense they would be involved in accidents more often

8. The 2 vehicle years most commonly involved in accidents were made in 2015 and 2014 <br/>
![VehicleYear_TotalSeriousFatalInjuries](https://github.com/user-attachments/assets/ef2325cf-8cb5-438b-a2d7-fc11b91a35a2) <br/>

### Limitations
* Data is only for Montgomery County, MD from 2015 to 2023
* Data is almost exclusively categorical, limiting the conclusions we can draw
* Data is reliant on the Automated Crash Reporting System of the Maryland State Police and includes human and mechanical errors

### Recommendations
1. Be more cautious when driving speed limits ranging from 25-45 mph
2. You are more likely to sustain serious injury for higher speed limits (especially 60 mph) and during Spring (April and May)
3. Be more cautious when driving towards the end of the year
4. Avoid any involvement with alcohol while driving
5. More research into why hondas and toyotas are most commonly involved in serious/fatal injury accidents needs to be done to determine whether that is due to its commonality on the road or due to extra risk
6. More research into why vehicles made in 2015 and 2014 are most commonly involved in serious/fatal injury accidents needs to be done to determine whether that is due to its commonality on the road or due to extra risk

### Proposal
https://docs.google.com/document/d/1aMJkBt-g-v69772nm9E2gI6Gbtyg9z6pSmKsPukXDuI/edit#heading=h.lntg56ljm653

### Presentation
https://docs.google.com/presentation/d/1OisqXRcGrlmLbNGo6381t5GdPO-3SRTnFC6CQ-_tK8Q/edit?usp=sharing

### Resources Used
https://pandas.pydata.org/docs/reference/api/pandas.to_datetime.html
https://stackoverflow.com/questions/26763344/convert-pandas-column-to-datetime
https://pandas.pydata.org/docs/user_guide/options.html
https://catalog.data.gov/dataset/crash-reporting-drivers-data
https://stackoverflow.com/questions/37625334/convert-month-int-to-month-name-in-pandas

### Navigation through Repository
In the main folder of repository, you'll find the analysis of the data separated based on the different questions we wanted to ask. <br/>
There will be a notebook analyzing the environmental conditions affecting injury severity, driver conditions affecting injury severity, and vehicle conditions affecting injury severity. <br/>
Inside the resources folder, you'll find the original dataset under Crash_Reporting_-_Drivers_Data.csv. You'll also find output figures under the Images folder.

