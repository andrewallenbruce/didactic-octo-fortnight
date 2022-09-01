# Basic measures of healthcare utilization, cost and price
The earliest measures of healthcare utilization and cost were simple and ‘high-level’. These measures were limited by the availability and quality of ‘secondary’ data sources. 

Secondary source refers to the generation of data from transactions unrelated to the purpose of any specific retrospective analysis. 

This is opposed to a ‘primary’ data source, where the data is generated for the specific purpose of an analysis. For payers, this secondary data source has been the billing claims submitted by providers for payment. The data was typically collected and stored after the payment had been ‘adjudicated’ and payment made to the provider. 

[[Adjudication]] is the processing of bills for payment, and involves determining the correct amount to be paid, accounting for discounts and patient out-of-pocket responsibilities.  These are referred to as ‘paid’ or ‘adjudicated’ claims.  

For providers, the secondary data has been generated from their own billing and accounting systems.  Initially focused on inpatient hospital services, measures such as number of discharges by type and average number of days per discharge, referred to as ‘average length of stay (ALOS)’, and case-mix adjusted cost per discharge and per patient day, provided hospitals with basic information about patterns and trends. 

An important note on defining the terms ‘cost’ and ‘price’ We normally think of ‘price’ as the amount we pay for a single unit of a product or service. For example, the price of a new television might be $850.  However, even in this simple example, there is some ambiguity in the definition of price. Suppose that there is a sale that discounts the price by 15%. You would now pay $722.50. Is this the price? Perhaps we define this as the ‘discounted price’. 

A similar situation exists in defining price for healthcare services. In this case, the base price is labeled the ‘charge’ for the service, and the discounted price is described by one of several alternative terms including, ‘[[allowed amount]]’, ‘paid amount’ or simply ‘payment’. It is important to be clear about the term used for this amount when analyzing costs.  

Another important concept is ‘net payment’.  We define price from the perspective of the entity actually purchasing the service, which in most cases is a commercial or government insurer or a large self-insured employer. We often refer to this entity as the ‘payer’. Most health insurance coverage includes provisions for the patient to pay a portion of the price, including a [[deductible]], copayment or coinsurance. 

The ‘cost’ to the payer is, therefore, the ‘paid amount’ less the total of the patient’s payments, defined as the patient’s ‘out-of-pocket’ amount. The result is referred to as the payer’s ‘net payment’.  The concept of ‘cost’ is obviously related to ‘price’.  

Continuing our simple example, we might refer to the $722.50 as the ‘cost’ of the television.  Therefore, in some cases the two concepts are equivalent. However, from another perspective we might want to refer to the price paid by the merchandizer as their ‘cost’ to differentiate from the ‘price’ paid by you, the consumer.

You can see that the terms used in defining variables and in labeling results can be confusing. For example, the price of an office visit to the patient should be distinguished from the cost to the physician of providing that service. This may seem trivial but can result in confusion when comparing results prepared from these two perspectives. 

To further complicate terminology, let’s consider that we have limited the use of the term price to the amount paid for a single unit of service or product.  We often refer to the total of all payments made for a collection of units as the ‘cost of care’.  

For example, a payer may calculate the total cost for a group of members as the sum of all payments for services provided to those members. We will dig deeper into measurements based on this total cost later in this chapter.

## Measuring cost and utilization from the payer perspective
It should be obvious that a payer is interested in what services it is purchasing and the price payed for each of these services. Does the price vary across multiple alternative providers? Is the use of an expensive procedure increasing?  Has the price of a specific medication increased since last year?  

There are dozens of relevant questions to be answered by ‘descriptive’ analytics. First, we need to start by understanding a few basic concepts. These measures often refer to a population or subpopulation / subset / cohort of ‘members’ or ‘patients’. It is best not to refer to this type of group as a ‘sample’, since this implies ‘randomization’ in selecting group members, a ‘random sample’. These sub-populations analyzed here are usually defined by a single characteristic, (e.g., location, health plan) and are not random selections. The purpose of this initial analysis is usually to identify variation in a measure between two or more of these groups. 

For example, we may want to identify any difference between Region A and Region B in the average ‘cost per member per month’. In testing this difference the ‘null hypothesis’ is that both are actually random samples from a larger population. The probability that this hypothesis is true, and, therefore that there is no difference between the two groups, is measured using a statistical test of the difference between two sample means. 

A significant difference in the means requires rejection of this hypothesis and acceptance that there is a non-random difference between the two groups. These measures must be ‘standardized’ to reflect relevant differences in the group characteristics that might explain the difference in cost per member. Some methods of standardization are discussed in a later chapter. 

For example, if the two groups differ in the distribution of age (e.g., younger vs. older), a higher average cost for one group might be simply explained by this age difference, and not an actually a difference in the cost characteristics of the two locations.

We refer to this as ‘controlling‘ for differences in these characteristics. This prevents us from ‘comparing apples to oranges.’ Most measures of member or patient utilization and cost are calculated as a rate. 

The denominator of many of the basic measures is ‘member month’.  Firstly, note that both numerator and denominator are ‘counts’ and must be limited to a specified period of time, (e.g., year). Of course, the same time-period must be applied for both. Secondly, a member month must be sourced from an enrollment or eligibility file and is defined as a month of service coverage for an eligible member. For example, if one-year (i.e., twelve continuous months) is selected as the analysis period, the number of member months is the sum of the months of eligibility of each member enrolled for all or a portion of that year. A member that became eligible in March and continued for the remainder of the year would add ten member months to the total, as would a member enrolled in January and dis-enrolled  in November. For example, the number of ‘admissions per 1,000 member months’ is a basic measure of the use of hospital care. A related measure is the ‘number of days in a hospital per 1,000 member months’.  

**Two important lessons:**
1) selecting 1,000 member months, rather than per single member month, avoids dealing with small fractions,
2) a third measure, the average length of stay, can be calculated as the ratio of these two measures. 

It is important to note the difference between the concepts of ‘member’ and ‘patient’. 

A member is an individual who is eligible to receive services as enrolled in a health plan. A member may or may not have received any services during the analysis period. 

A patient is a member that has received at least one service during the analysis period. By definition, a patient is also counted as a member. A patient can be described by a specific diagnosis or service (e.g., received emergency room care for a diabetes-related condition).  It is also important to note that there is a slight difference between payers and hospitals in the methods used to calculate hospitalization-based measures.

These calculations require a count of hospitalizations for either the denominator or numerator of a measure. From the payer perspective the unit is often referred to as an ‘admission’, and from the hospital perspective a ‘discharge’. The difference is in the date used to assign the hospitalization to an analysis period (e.g., a calendar year). 

Admissions are counted in the time-period that includes the ‘admission date’ (i.e., the first date), while discharges are counted in the time-period that includes the ‘discharge date’ (i.e., the last date). 

Why is it important to recognize this difference? For payers, it is important to match the hospitalization to the date of a member’s enrollment, since this is the method of computing the eligible members for the analysis period. The term of a member’s benefit coverage is determined on the first date of their current plan enrollment. 

For the provider, hospitalizations are only counted when the patient is discharged and all documentation is completed. Payment methods based on hospitalizations count discharges within the analysis period.  It should be obvious that measures such as ‘length of stay’ and ‘cost per case’ cannot be calculated until the discharge is recorded. Payers deal with this by waiting for the collection of data from the discharge to become available before calculating these measures. This difference in perspective can result in some confusion when reconciling hospitalization counts between payer and hospital sources.  

## Measuring cost and utilization from the provider perspective
It should be obvious that a provider is interested in the utilization of resources used in delivering its services to patients, and in the relationship between the cost of these resources and the payments received for providing the service.  The average length of stay (ALOS) is a useful measure of resource use for a hospitalization, since the longer the stay, the higher is the resource consumption, (e.g., nursing services, facility overhead, supplies). However, it is also likely that resource use is more intense during the earlier days of the stay. The hospital’s financial staff are responsible for this type of cost accounting, and we will not discuss these methods in this document. However, we do know that hospitals compare their ALOS to benchmarks in order to identify opportunities to reduce resource use and to increase patient throughput.  They can also apply methods to estimate the cost based on department-level (e.g., radiology, intensive care, emergency room) ‘cost-to-charge ratios’. These ratios are reported to [[Medicare]] and are estimates of the ratio of total costs in a department to the total charges for services provided by that department. These include indirect and other allocated costs. This ratio is applied to the charges for each of that department’s services to estimate cost for that service.  For example, the cost of an imaging service is estimated as the charge for that service multiplied by this ratio.  

There are dozens of relevant questions to be answered by analytics. We need to start with a few basic concepts. As discussed previously, the primary unit of analysis for hospitals is the discharge. The primary method of classifying a discharge is a Diagnosis Related Group (DRG). This classification model is maintained by the Centers for Medicare and Medicaid ([[CMS]]) and is used to determine the Medicare or Medicaid  payment rate for each discharge. Each DRG is assigned a weight and the mean of these weights for all of a hospital’s discharges is referred to as its ‘case-mix index (CMI)’. To calculate Medicare payments to a hospital this CMI is multiplied by a base rate common to all similar hospitals. Of course, the actual payment calculation is more complicated than this, but this is the general idea and demonstrates the use of the CMI. 

More detail on ‘standardization’ methods using DRG are covered in a later chapter. The primary units for other hospital services and for ambulatory services provided in a physician office are ‘visit’ or ‘procedure’. For example, we count emergency department and physician office visits, and count specific procedure-types for imaging departments. It is important that you understand the grouping of these procedures into higher-level categories. For example, the category “MRI” includes many different specific procedures, while the category “Imaging” includes MRI, as well as many other types of procedure, such as CT. These aggregations are discussed in a later chapter.