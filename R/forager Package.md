---
created: 2022-08-17T15:49:59-04:00
updated: 2022-08-17T15:49:59-04:00
---
# Front Office and Productivity

## Point of Service Cash Collected
 - Description: Sum of all payments (Cash, Checks and Credit Card) posted within 7 days of date of service.
 - Business Application:
	 - Measure the front-office collection efforts
	 - Collecting patient balances at the time of service will reduce billing costs
 - Calculation: Sum of payments from any source of any type within 7 days of date of service.
 - Event Date: Entry/Post Date

## Patient Visit Count
- Description: Count of unique encounters between patient, provider and date of service. Sum of all Patient Encounters. This KPI is a claim level measure, meaning when sliced by a charge level dimension, such as CPT code, the results may be skewed.
- Example/Calculation:
	- A patient who saw a physician on one day or twice in one day is equal to one Patient Visit Count.
	- A patient who saw a physician twice on two separate days of service is two Patient Visit Counts.


## Patients Seen Count
Description: The number of patients seen in a time slice (e.g. month) is the number of unique patients seen in
that time slice (e.g. month).
o Example: If a patient is seen (produces an encounter) multiple times within the time period selected,
the patient is only counted once.

 Business Application:
o Measure the productivity of the practice
o Track trends over time and seasonality
 Calculation: Distinct count of patients seen in the selected time frame.
 Event Date=DOS
o Drivers: Number of Patients Seen (Total)

## New Patients Seen Count
Description: The number of new patients seen in a time slice (e.g. month) is the number of new unique
patients seen in that time slice (e.g. month).
o Example: If a new patient is seen (produces an encounter) multiple times within the time period
selected, the patient is only counted once.

 Business Application:
o Measure the productivity of the practice
o Track trends over time and seasonality
 Calculation: Distinct Count of New Patients seen in the selected time frame.
 Event Date=DOS
o Drivers: Number of Patients Seen (Total)

## New Patient Percentage
Description: The number of new patients seen divided by total number of patients seen.
o Example: (CPT Codes: 92002, 92004, 99201-99205, 99241-99245, 99251-99255, 99324-99328, 99341-
99345, 99381-99387), to the total number of patients seen in a given period.

 Business Application:
o Identify the growth rate of new patients into the practice
o Measure the productivity of the practice
o Track trends over time and seasonality
 Calculation: [Number of New Patients] / [Number of Patients Seen]
 Event Date=DOS
 Drivers: Number of Patients Seen (Total)

## Visits Per Days Worked

## Work RVU Unit

## RVU Work Units Per Days Worked

## RVU Work Units Per Patient

## RVU Work Units Per Procedure

## RVU Work Units Per Procedure

# Charge Capture and Billing

## Number of Claims

