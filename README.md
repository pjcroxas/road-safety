# Road Safety: Comprehensive Analysis of DRIVERs Road Crash Data

## Overview
---

**DRIVERs** is the central database for road crashes across the Philippines. Various agencies, such as the PNP-Highway Patrol Group, LGUs from Metro Manila, Metro Cebu, and Metro Davao, as well as the Department of Health (DOH), contribute to this database. It is used by decision-makers across sectors such as transportation, urban planning, and road safety. The primary goal of the database is to monitor road accidents and assess the effectiveness of existing public policies in reducing casualties and mortality rates.

## Executive Summary
---

## Project Summary
---

A. The goal of this project is to:

1. Identify the  underlying cause of an accident
2. Evaluate the data collection methodology
3. Recommend policy to lower the accidents

B. The Project is divided into the following topics:

1. Data Quality Inspection
2. Data Analysis
3. Statistical Analysis
4. Recommendations

C. Data Structure

## I. Data Quality Inspection
---
![image](https://github.com/user-attachments/assets/ea67af8f-701d-4d45-b68e-3e9ed9983f09)


## II. Exploratory Data Analysis (EDA)
---
![image](https://github.com/user-attachments/assets/0f539bc2-cb83-44c9-9399-d067c79b0b03)

![image](https://github.com/user-attachments/assets/ec86676b-f065-4f7b-aac1-665f7b094ed3)

![image](https://github.com/user-attachments/assets/ba8b6e0e-f25d-4a7a-acc6-7a75d814c85e)


1. **Accident Trend**
    1. For the annual comparison, 2018 recorded the highest number of accidents, with two peaks (`march` and `october`). With accidents centered in `ber` months.
        1. accidents occurrences in March significantly decreases to 2020, however it increased by five times in 2021.
        2. The number of accidents in October decreased significantly to 2020. Though there is `zero` records in 2021, there is no data to support that the accidents are totally diminished.
    2. Daily Average Accident per Hour
        1. High accident rates usually occurs in the morning. It has two peaks: 7 AM and 12 AM.
        2. For 7 AM, Thursday recorded the highest number of accidents which has approx. of 31 incidents. While at midnight, Monday recorded an approx. of 32 incidents.
        3. For weekdays, accidents are low in the afternoon and evening (between 1 pm to 9 pm).
        4. For weekends, the recorded average accidents didn’t exceed 22 incidents.
        5. Sunday always recorded the lowest average accidents per hour. It only spiked at 10 pm.


![image](https://github.com/user-attachments/assets/509e7151-fd7a-46ab-a0d7-52e15163d0fc)

2.  Severity
    1. Records for `Fatal/Injury`, and `Property/Injury`  involves one vehicle. 
    2. For `fatal` 45.5% involves two or more vehicles, while 54.5% involves one vehicle.
    3. For `injury` majority are single vehicle with 88.3% of total records.
    4. For `Injury/Property`, `Injury/Property Damage` , `Property`, and `Property Damage`, the majority of these involves two or more vehicles, with percentages 88.9%, 69.6%, 85.3%, 91.8% respectively.


![image](https://github.com/user-attachments/assets/84f1aca9-5cda-42aa-b755-e27118dd02c4)

![image](https://github.com/user-attachments/assets/bb288dc1-f083-48b3-a7f6-5f5a3c4f9ca9)


3. Accident prone area:
- Majority of the recorded incidents are `Property` or `Property Damage`.
    - `Taguig City`, and `Muntinlupa` having both `100%` of recorded incidents are `Property Damage`
- From 2018 to 2020, `QC` , `Makati`, and `Mandaluyong` exceeds `4000` casualties. These cities in Metro Manila are business districts.
    - For QC, `69.2%` are `injury` (approximately 3180 casualties), while `30.8%` are `property related` (approximately 1420 casualties).
    - For Makati `40%` are fatal (approx. 1400 incidents), and `60%` (approx. 2700 casualties) are property related and damage.
    - For Mandaluyong, property damage is majority.
    - QC, and Pasig are cities that records `fatal` incidents. With Pasig having `14.3%` of fatal road crash.
- `Cebu City` the only city outside Metro Manila, recorded a `66.7%` of injury or property.



![image](https://github.com/user-attachments/assets/b7542d82-4785-42ef-b617-03bcea0ba318)

![image](https://github.com/user-attachments/assets/cf38e5fc-088a-4bb7-8e41-0dd7ea667325)

4.  Accident prone roads
    1. Accident prone areas are major road.
    2. From 2018 to 2020, EDSA has been the top rank in road crashes with over 10,000 recorded incidents.
        1. Majority of the incidents in EDSA are `property` related, with `75%` (approx. 7420 casualties).
        2. `Injuries`  recorded in EDSA are `25%` (approx. 3180 casualties)
    3. `EDSA` and `Commonwealth Ave.` are roads that recorded injury-related incidents, with Commonwealth having recorded a `52.7%` (approx. 1160 casualties).
    4. There is no fatalities recorded on major highways.



![image](https://github.com/user-attachments/assets/4cba3ec7-f0fd-4cda-a0ea-f60ec9d23665)

![image](https://github.com/user-attachments/assets/93f63993-1de6-434d-ac03-9990d1012fca)

5. Weather Situation
    1. `Partly-cloudy-day` , `clear-day`, `rain` makes up the total `80%` of accidents.
    2. The majority of the casualties based on weather are `injury` and `property`.
    3. `clear-night`, `clear-day`and `partly-cloudy` recorded fatal casualties.


![image](https://github.com/user-attachments/assets/f7a53064-414b-4bf7-9df7-c18755d6b4c8)

![image](https://github.com/user-attachments/assets/f61551d4-0f99-4fa4-ad99-1f2a37535950)


6. Cause
    - The main cause of road crashes is `Human error`, with a total record of 60,000 casualties from 2018 to 2020.
        - Majority of `Human error` results to `property damage` with 61.7% (approx. 31,700) casualties .
        - For `injury or property` , 14.8% (approx. 8800) casualties.
    - For `vehicle defect`, 20% are fatal (approx. 90 casualties), while 40% suffers from injuries (approx. 180).
    - For `Road Defect` , all incidents results to property damage.


![image](https://github.com/user-attachments/assets/b3cc6694-bcc0-4181-9d82-b9999f4f9b8a)

![image](https://github.com/user-attachments/assets/7146e2db-660c-4c57-bef6-72729e50d2f8)

7. Vehicle type
    - The `80%` of the accident involves, `car`, `motorcycle`, `SUV`, `van`, `bus`.
        - Most of the severities for these 6 types of vehicles resulted to `property damage`
        - Recorded `fatalities` involves `car`, `motorcycle`, and `van`
            - The highest number of accidents involves `car` , with 1% (approx, 183) casualties.
            - For motorcycles, 4.1% (approx. 389) casualties, which is higher than cars.
            - For van, 5.7% (approx 345) casualties.
        - `Injury`  were recorded on all 6 vehicle types.
            - For motorcycles, the recorded injuries is 22.7 (approx. 1446 casualties)
            - For cars, 11.3% (approx. 2060 casualties).
            - For buses, 3% (approx. 163. casualties)
            - For SUVs, 5% (approx. 468 casualties)
            - For taxi, 8% (approx. 271 casualties
            - For van, 9.7% (approx. 586 casualties)

## Recommendations
