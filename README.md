# Road Safety: Comprehensive Analysis of DRIVERs Road Crash Data
**DRIVERs** is the central database for road crashes across the Philippines. Various agencies, such as the `PNP-Highway Patrol Group`, `LGUs` from `Metro Manila`, `Metro Cebu`, and `Metro Davao`, as well as the `Department of Health (DOH)`, contribute to this database. It is used by decision-makers across sectors such as transportation, urban planning, and road safety. The primary goal of the database is to monitor road accidents and assess the effectiveness of existing public policies in reducing casualties and mortality rates.

## Executive Summary

**Trend (Daily Average Accidents per Hour):**
- On weekdays, the majority of accidents occur in the morning, peaking around 7 AM (between 6 AM and 9 AM), and again at midnight (12 AM). In the afternoon, road crashes tend to decrease. On weekends, accidents do not exceed 28 casualties throughout the day, except for a spike at 10 AM on Sundays.

**Accident Severity:**
- Majority accidents result in property damage, followed by incidents involving injury.

**Accident-Prone Cities:**
- Key accident-prone cities like Quezon City and Mandaluyong mostly report property damage and injuries. In contrast, Makati and Pasig recorded fatalities, with 40% and 14.3% casualty rates, respectively.

**Accident-Prone Roads:**
- EDSA ranks highest in road crashes, with most incidents leading to property damage and injuries. Fatalities are rare on major roads and highways, occurring primarily on smaller streets and avenues.

**Weather Conditions:**
- Fatalities are recorded during both clear (partly cloudy) and rainy conditions. Injuries occur across all six weather conditions.

**Root Cause:**
- Human error is the leading cause of accidents, accounting for 586 casualties.

**Vehicle Type:**
- Most incidents involve cars, motorcycles, vans, taxis, and SUVs. Motorcycles account for the highest number of fatalities (389 casualties), followed by cars (183 casualties).

## Project Summary

A. The goal of this analysis is to:

1. Identify the underlying causes of a road crash
2. Evaluate the data collection methodology
3. Recommend policy to help reduce the road crash

B. The Project is divided into the following topics:

1. Data Quality Inspection
2. Exploratory Data Analysis
4. Recommendations

C. Data Structure

## I. Data Quality Inspection
![image](https://github.com/user-attachments/assets/ea67af8f-701d-4d45-b68e-3e9ed9983f09)
 - The majority of the missing data suggests that certain fields are not set as required. Features like severity, injury, age, damage, gender, and defect should be prioritized and marked as mandatory fields.
 - Inconsistencies in categorical data, such as region, city, and road, indicate that the data are being entered as free-text strings instead of using dropdowns or predefined selection options.
 - Supplemental data, such as descriptions for the main cause of accidents, should be provided near the relevant fields to support accurate input.
 - Fields like the date of report, email of the encoder, and other similar details should be automatically captured by the system to reduce the encoder’s workload.
 - Finally, the collection or extraction of personal information, such as name, license number, engine number, and address, should be minimized to protect privacy.

## II. Exploratory Data Analysis (EDA)
![image](https://github.com/user-attachments/assets/0f539bc2-cb83-44c9-9399-d067c79b0b03)

![image](https://github.com/user-attachments/assets/ec86676b-f065-4f7b-aac1-665f7b094ed3)

![image](https://github.com/user-attachments/assets/ba8b6e0e-f25d-4a7a-acc6-7a75d814c85e)
1. **Accident Trend**
   - For the annual comparison, 2018 recorded the highest number of accidents, with two peaks (`march` and `october`). With accidents centered in `ber` months.
     - accidents occurrences in March significantly decreases to 2020, however it increased by five times in 2021.
     - The number of accidents in October decreased significantly to 2020. Though there is `zero` records in 2021, there is no data to support that the accidents are totally diminished.
   - Daily Average Accident per Hour
     - High accident rates usually occurs in the morning. It has two peaks: 7 AM and 12 AM.
     - For 7 AM, Thursday recorded the highest number of accidents which has approx. of 31 incidents. While at midnight, Monday recorded an approx. of 32 incidents.
     - For weekdays, accidents are low in the afternoon and evening (between 1 pm to 9 pm).
     - For weekends, the recorded average accidents didn’t exceed 22 incidents.
     - Sunday always recorded the lowest average accidents per hour. It only spiked at 10 pm.

---
![image](https://github.com/user-attachments/assets/d26cca54-8bfe-44b5-9b38-31949b3d0e62)
2. **Severity**
   - Records for `Fatal/Injury`, and `Property/Injury`  involves one vehicle.
   - For `fatal` 45.5% involves two or more vehicles, while 54.5% involves one vehicle.
   - For `injury` majority are single vehicle with 88.3% of total records.
   - For `Injury/Property`, `Injury/Property Damage` , `Property`, and `Property Damage`, the majority of these involves two or more vehicles, with percentages 88.9%, 69.6%, 85.3%, 91.8% respectively.

![image](https://github.com/user-attachments/assets/cc644df6-436a-4350-90dd-d5714c5f499d)
![image](https://github.com/user-attachments/assets/0ec10da3-fe28-4f39-8d41-22b3f1276c1f)

3. **Accident prone area**
   - Majority of the recorded incidents are `Property` or `Property Damage`.
     - `Taguig City`, and `Muntinlupa` having both `100%` of recorded incidents are `Property Damage`
   - From 2018 to 2020, `QC` , `Makati`, and `Mandaluyong` exceeds `4000` casualties. These cities in Metro Manila are business districts.
     - For QC, `69.2%` are `injury` (approximately 3180 casualties), while `30.8%` are `property related` (approximately 1420 casualties).
     - For Makati `40%` are fatal (approx. 1400 incidents), and `60%` (approx. 2700 casualties) are property related and damage.
     - For Mandaluyong, property damage is majority.
     - QC, and Pasig are cities that records `fatal` incidents. With Pasig having `14.3%` of fatal road crash.
   - `Cebu City` the only city outside Metro Manila, recorded a `66.7%` of injury or property.

---
![image](https://github.com/user-attachments/assets/4e209029-6488-4b4a-b87c-f16c43339d0a)
![image](https://github.com/user-attachments/assets/dc349108-2225-4a2b-ba03-e66e64cc8df1)
4. **Accident prone roads**
   - Accident prone areas are major road.
   - From 2018 to 2020, EDSA has been the top rank in road crashes with over 10,000 recorded incidents.
     - Majority of the incidents in EDSA are `property` related, with `75%` (approx. 7420 casualties).
     - `Injuries`  recorded in EDSA are `25%` (approx. 3180 casualties)
   - `EDSA` and `Commonwealth Ave.` are roads that recorded injury-related incidents, with Commonwealth having recorded a `52.7%` (approx. 1160 casualties).
   - There is no fatalities recorded on major highways.

---
![image](https://github.com/user-attachments/assets/6c021815-e7e8-4ee3-9632-aeb9ecf69d0a)
![image](https://github.com/user-attachments/assets/4878e484-b541-49cc-abd7-80d64c80cc5f)
5. **Weather Situation**
   - `Partly-cloudy-day` , `clear-day`, `rain` makes up the total `80%` of accidents.
   - The majority of the casualties based on weather are `injury` and `property`.
   - `clear-night`, `clear-day`and `partly-cloudy` recorded fatal casualties.

---
![image](https://github.com/user-attachments/assets/23fea4f8-d923-4755-b440-344cab5b0f4d)
![image](https://github.com/user-attachments/assets/169f6bb6-1b34-47a1-98a8-b6249e8b4860)
6. **Cause**
   - The main cause of road crashes is `Human error`, with a total record of 60,000 casualties from 2018 to 2020.
     - Majority of `Human error` results to `property damage` with 61.7% (approx. 31,700) casualties .
     - For `injury or property` , 14.8% (approx. 8800) casualties.
   - For `vehicle defect`, 20% are fatal (approx. 90 casualties), while 40% suffers from injuries (approx. 180).
   - For `Road Defect` , all incidents results to property damage.

---
![image](https://github.com/user-attachments/assets/ca9396d4-a0ab-4f86-ae11-df180e335b67)
![image](https://github.com/user-attachments/assets/2d72bf99-d330-42e6-80a6-5da501ea4434)
7. **Vehicle type**
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

1. **Time-Specific Interventions**
    - **Peak Hour Safety Campaigns:**
        - **Weekday mornings (6 AM - 9 AM)**: Implement stricter enforcement of traffic rules and launch targeted road safety campaigns during these hours to mitigate the high volume of accidents.
        - **Midnight Accidents**: Strengthen patrols and consider placing checkpoints or speed cameras around midnight when accidents spike. Implement stricter speed limits in areas prone to nighttime crashes.
    - **Weekend Monitoring:**
        - Focus resources on **Sunday mornings (10 AM)** when accidents peak, by deploying traffic enforcers or utilizing technology such as AI-based traffic monitoring systems in accident-prone areas.
2. **City-Specific Safety Programs**
    - **For Quezon City and Mandaluyong**:
        - Expand accident prevention programs focusing on property damage and injury reduction. These could include better road signage, improved road lighting, and more stringent monitoring of vehicle speed and lane discipline.
    - **For Makati and Pasig**:
        - Prioritize efforts to reduce fatal crashes. This may include:
            - **Targeted interventions in high-fatality areas**, such as improved road lighting, stricter enforcement of helmet laws for motorcycles, and pedestrian safety enhancements like speed bumps, barriers, and better crosswalk visibility.
            - Public safety campaigns specifically tailored to these cities that emphasize the risks of reckless driving and speeding.
3. **High-Risk Roads:**
    - **EDSA**: Introduce additional safety measures on EDSA by:
        - Expanding surveillance through traffic cameras and real-time incident reporting apps.
        - Enhancing driver education and awareness campaigns, emphasizing safe driving practices during high-traffic hours to minimize property damage and injury-related incidents.
    - **Small Streets and Avenues**: Conduct safety audits to identify problematic roads where fatalities occur. Improve signage, lighting, and pedestrian safety features in these areas. Enforce lower speed limits in smaller streets and avenues to reduce fatal crashes.
4. **Weather Condition Adaptation:**
    - Equip traffic and enforcement systems with weather condition alerts to adjust enforcement efforts during:
        - **Rainy Conditions**: Enforce reduced speed limits, ensure proper road drainage systems, and promote the use of hazard lights.
        - **Clear Conditions**: Continue to monitor and address speeding and reckless driving.
5. **Human Error Reduction Initiatives:**
    - **Driver Education Programs**:
        - Establish periodic **driver refresher courses** focusing on common human errors that lead to accidents. These could include:
            - Defensive driving techniques
            - Safe overtaking and merging practices
            - Safe speed management and hazard anticipation
        - Leverage **technology** such as mobile apps for drivers that provide alerts and real-time guidance on road conditions and rules.
    - **Stricter Penalties for Human Error**: Increase penalties for human-error-related offenses such as distracted driving, DUI, speeding, and reckless driving. Implement **"zero tolerance"** rules for repeat offenders.
6. **Vehicle-Specific Measures**
    - **Motorcycle Safety**:
        - Focus on reducing fatalities by implementing stricter helmet laws and safety gear enforcement.
        - Launch public safety campaigns aimed at motorcycle drivers emphasizing defensive driving, lane discipline, and adherence to speed limits.
        - Provide **dedicated motorcycle lanes** where feasible to minimize accidents involving cars and motorcycles.
    - **Car and SUV Regulation**:
        - Encourage **mandatory installation of advanced safety features** in vehicles such as anti-lock braking systems (ABS), airbags, and vehicle stability control systems.
        - Promote safe driving practices for all vehicle types through public awareness campaigns, highlighting the dangers of speeding, distracted driving, and tailgating.
7. **Accident Response & Post-Crash Care**
    - **Improve Emergency Response Times**: In collaboration with local governments, set up additional emergency response stations along major roads and in high-risk areas, such as accident-prone streets and avenues.
    - **Post-Crash Care**: Increase the number of trained first responders and equip ambulances with life-saving tools to address injuries promptly, reducing the likelihood of fatalities.
8. **Data-Driven Monitoring & Evaluation**
    - **Accident Tracking Systems**:
        - Develop a centralized, data-driven road traffic accident tracking system that allows for real-time data collection and analysis of accidents. Use this data to inform future safety initiatives and road infrastructure planning.
    - **Periodic Policy Review**:
        - Conduct regular evaluations of accident data to assess the effectiveness of the implemented measures. Adjust strategies as necessary to ensure continuous improvement in road safety outcomes.

These recommendations aim to target the root causes of accidents while addressing the specific risks posed by different vehicle types, time frames, cities, and roads. By focusing on both prevention and responsive measures, the overall goal is to reduce casualties, particularly fatalities, and property damage.
