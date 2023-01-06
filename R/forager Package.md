---
created: 2022-08-17T15:49:59-04:00
updated: 2022-09-24T20:12:50-04:00
---


```cardlink
url: https://github.com/andrewallenbruce/forager
title: "GitHub - andrewallenbruce/forager: Healthcare Revenue Cycle Analysis Suite"
description: "Healthcare Revenue Cycle Analysis Suite. Contribute to andrewallenbruce/forager development by creating an account on GitHub."
host: github.com
favicon: https://github.githubassets.com/favicons/favicon.svg
image: https://repository-images.githubusercontent.com/528716264/afaf256b-531d-45db-a3e9-de19eb285061
```


## Front Office and Productivity

## Point of Service Cash Collected
 - Description: Sum of all payments (Cash, Checks and Credit Card) posted within 7 days of date of service.
 - Business Application:
	 - Measure the front-office collection efforts
	 - Collecting patient balances at the time of service will reduce billing costs
 - Calculation: Sum of payments from any source of any type within 7 days of date of service.
 - Event Date: Entry/Post Date

## Patient Visit Count
- Description: Count of unique encounters between patient, provider and date of service. Sum of all Patient Encounters. This [[Key Performance Indicator|KPI]] is a claim level measure, meaning when sliced by a charge level dimension, such as [[Current Procedural Terminology|CPT]] code, the results may be skewed.
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
o Example: ([[Current Procedural Terminology|CPT]] Codes: 92002, 92004, 99201-99205, 99241-99245, 99251-99255, 99324-99328, 99341-
99345, 99381-99387), to the total number of patients seen in a given period.

 Business Application:
o Identify the growth rate of new patients into the practice
o Measure the productivity of the practice
o Track trends over time and seasonality
 Calculation: [Number of New Patients] / [Number of Patients Seen]
 Event Date=DOS
 Drivers: Number of Patients Seen (Total)

## Visits Per Days Worked

## Work [[Relative Value Unit (RVU)|RVU]] Unit

## [[Relative Value Unit (RVU)|RVU]] Work Units Per Days Worked

## [[Relative Value Unit (RVU)|RVU]] Work Units Per Patient

## [[Relative Value Unit (RVU)|RVU]] Work Units Per Procedure

## [[Relative Value Unit (RVU)|RVU]] Work Units Per Procedure

# Charge Capture and Billing

## Number of Claims

