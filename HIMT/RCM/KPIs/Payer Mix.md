---
tags: definition, him, kpi, metrics, rcm, analytics, data
author: Yuval Lirov, Max Reiboldt, Nate Moore
alias: Payer mix, Payer Mix Ratio
related:
created: 2021-12-27T12:07:41-05:00
updated: 2022-08-05T23:57:45-04:00
---
# Payer Mix
The percentage of revenue coming from each type of contracted payer such as government-based insurance, commercial insurance, and self-paying individuals for a facility or provider.^[ISBN 9781584266464 - Principles of Healthcare Reimbursement]

## Monitoring Payer Mix
Because payers will pay for services at different rates, a shift in your patient population to a payer who generally pays less can have a substantial impact on your practice revenues. Monitor on a regular basis the percentage of services associated with each of your payers and verify a good payer mix that represents a strong revenue stream for the practice. Having a well-balanced mix decreases the control any one payer will have on your practice.^[Practice Management Study Guide - AAPC - Google Books]

## Reviewing Payer Mix
This begins by looking at payers as a regular initiative of the practice’s management. Payer mix should be considered in light of developing a marketing strategy to derive a different payer mix. Marketing manifests itself in various ways for medical practices in the current payer market, including marketing strictly to third-party payers and, in some instances, marketing directly to business/industry or the patient.^[ISBN 9781603592963 - Financial Management of the Medical Practice (Practice Success)]

## Payer Mix Ratio
As alluded to earlier, obtaining a detailed understanding of a practice’s payer mix is essential to achieving a comprehensive analysis of the entity’s broader financial stability, as well as being critical to ongoing financial management on behalf of the practice’s leadership. A typical payer mix ratio is based on net charges for a payer, divided by total net charges for the practice:

### $$\frac {\textrm{Net Charges for Payer A}}{\textrm{Total Net Charges}}=\textrm{Payer Mix Ratio}$$

For instance, if a practice’s [[Medicare]] charges represent $355,000 of $1,200,000 in total net charges, the practice’s [[Medicare]] payer mix would be calculated as follows:

### $$\frac {$350,000}{$1,200,000}=\textrm{29\%}$$

This says that the practice’s payer mix is composed of 29% Medicare coverage. While knowing the Medicare payer mix is certainly important, knowing how the remaining 71% of the practice’s payer mix is allocated makes that ratio even more relevant and actionable. 

As such, it is beneficial for practices to maintain a payer mix report on their dashboard to follow the payer mix among all of the practice’s payers on a monthly basis, as well as tracking the fluctuations of their payer mix on a rolling basis. 

The following table and chart are examples of reports that should be broken down even further to show monthly performance, day-to-day variation in payer mix (which is also relevant when analyzing [[Accounts Receivable]] by payer.) Further, these reports can show payer mix by provider, to determine payer concentration for each provider as well as AR by payer.


| Payer           | 2017 | 2018 | 2019 | 2020 | 2021 |
| --------------- | ---- | ---- | ---- | ---- | ---- |
| Medicare        | 24%  | 23%  | 28%  | 31%  | 26%  |
| Medicaid        | 17%  | 22%  | 24%  | 19%  | 25%  |
| ABC Ins Co      | 25%  | 24%  | 21%  | 19%  | 21%  |
| XYZ Health Plan | 34%  | 31%  | 27%  | 31%  | 28%  |
| TOTAL           | 100% | 100% | 100% | 100% | 100% |


```chart
type: bar
labels: [2017,2018,2019,2020,2021]
series:
- title: Medicare
data: [24,23,28,31,26]
- title: Medicaid
data: [17,22,24,19,25]
- title: ABC Ins
data: [25,24,21,19,21]
- title: XYZ Plan
data: [34,31,27,31,28]
tension: 0
width: 95%
labelColors: false
fill: true
beginAtZero: false
```


## Payer Mix Report Example
The following is an example of a simple bar chart comparing payer mix by payer groups. Payer groups are maintained like procedure categories. For example, the payer group [[Medicare]] might contain traditional Medicare, Railroad Medicare, or Medicare Advantage plans. It is helpful to understand changes in payer mix over time. The practice’s largest payer is almost four percentage points larger year-to-date compared to the prior year. If this is a better payer for the practice, that could be wonderful news. If this payer has higher deductibles to collect and more denials to appeal, the increase may not be such good news. The filters in the dashboard can help management understand whether this change in payer mix is especially relevant for a certain location, procedure group, or department in the practice. p273 ^[ISBN 9781568295442 - Even Better Data, Better Decisions (Advanced Business Intelligence for Medical Practice)]

```chart
type: bar
labels: [YTD,PYTD]
series:
  - title: Group A
    data: [7.4,5.0]
  - title: Group B
    data: [3.7,3.3]
  - title: Group C
    data: [1.9,1.5]
  - title: Group D
    data: [4.2,6.3]
  - title: Group E
    data: [48.3,44.5]
tension: 0
width: 95%
labelColors: false
fill: true
beginAtZero: false
```

## Relationship to Provider Compensation
The practice’s payer mix is often used in determining an appropriate compensation plan. For example, in hospital employment, a poor payer mix composed of a high level of [[Medicaid]] and self-pay patients may indicate that a collections-type model is not as viable. Thus, the focus would turn to wRVUs or some other metric. In private practice, the payer mix of various physicians is compared to determine whether they all have similar payer mixes. If this is not the case, it may indicate that some equilibrium is needed within the model to shift some of the payer risk to the practice as a whole instead of a single physician incurring the poor payer mix. If the model is the individual productivity-based model, a poor payer mix is detrimental to a physician. ^[ISBN 9781603592963 - Financial Management of the Medical Practice (Practice Success)]

### Payer Mix by Work RVU
Comparing payer mix by receipts to payer mix work [[Relative Value Unit (RVU)]] can be very instructive. A payer who represents more work (as measured by work [[Relative Value Unit (RVU)]]) but is a lower percentage of receipts is not a good payer relative to the other payers in the practice. If that payer’s business is growing, the practice has reason to be concerned about working harder for less. p274 ^[ISBN 9781568295442 - Even Better Data, Better Decisions (Advanced Business Intelligence for Medical Practice)]

### Receipts Per Work RVU
The idea of working harder for less is captured in the practice’s receipts per work RVU measure. The chief executive officer uses the metric to compare procedures and payers across providers. A relatively new addition to the dashboard is a series of charts like the following line chart that trend receipts per wRVU over time. The dashboard includes several similar charts that analyze groups of five procedure categories.

Since receipts per work RVU is such an important metric for this practice, the dashboard also includes similar charts trending receipts and work RVUs separately for each procedure category. Charting receipts and work RVUs separately makes it easier to explain differences in the measure over time. In this case, the practice does not match the month receipts were collected to the month that the work RVUs were rendered.

```chartsview
#-----------------#
#- chart type    -#
#-----------------#
type: TinyLine

#-----------------#
#- chart data    -#
#-----------------#
data: [264, 417, 438, 887, 309, 397, 550, 575, 563, 430, 525, 592, 492, 467, 513, 546, 983, 340, 539, 243, 226, 192]

#-----------------#
#- chart options -#
#-----------------#
options:
  height: 100
  autoFit: false
  smooth: false
  tooltip: false
  annotations:
    - type: "line"
      start: ["min", "mean"]
      end: ["max", "mean"]
      style:
        stroke: "rgba(0, 0, 0, 0.45)"
      text:
        content: "Average"
        offsetY: -1
        style:
          textAlign: "left"
          fontSize: 12
          fill: "rgba(44, 53, 66, 0.45)"
          textBaseline: "bottom"
    - type: "line"
      start: ["min", 800]
      end: ["max", 800]
      style:
        stroke: "rgba(200, 0, 0, 0.55)"
      text:
        content: "Target"
        offsetY: -1
        style:
          textAlign: "left"
          fontSize: 12
          fill: "rgba(44, 53, 66, 0.45)"
          textBaseline: "bottom"
```

Other practices match charges and receipts in the same month and trend that data. Consider an example of a service rendered in April. The practice may receive a copayment in April, a primary insurance payment in May, and a secondary insurance payment in June. It will likely take several months to record most of the revenues against April charges. This lag in payments received against charges introduces a delay before the trend matching charges and receipts is available for the month. Though matching charges against receipts does have a lag, the advantage is that the receipts are measured against the charges that generated the receipts.^[ISBN 9781568295442 - Even Better Data, Better Decisions (Advanced Business Intelligence for Medical Practice)]

### Compensation Per wRVU Ratio
This ratio is often referred to as the *conversion factor* and is a key variable in wRVU productivity models. It is also used to gauge the appropriateness of a physician’s compensation in relation to benchmark data. For example, in private practice, assessing the compensation per wRVU ratio would indicate whether the physician was receiving a proper level of compensation at the respective level of productivity. If this is not the case, it would indicate that changes are likely necessary within the practice to realize more compensation for the same level of productivity. This would involve cost reductions, negotiating better payer contracts, etc. In a hospital employment setting, a higher conversion factor could indicate that a model may not be deemed to be within fair market value limitations. This is because it could be assumed that, for the physician’s level of productivity, he or she was receiving too much compensation.^[ISBN 9781603592963 - Financial Management of the Medical Practice (Practice Success)]

### Compensation to Collections
This ratio is similar to the above but it replaces wRVUs with collections. This ratio is very important in private practice, as it allows the practice to understand how much of each dollar received in collections gets taken home as cash compensation. A high compensation to collections ratio would indicate that the practice is good at managing its overhead. This ratio is also used in hospital employment settings, but to a lesser degree in terms of determining appropriate compensation (unless the model used is a percentage of collections model.) This places much more focus on wRVU-related metrics.^[ISBN 9781603592963 - Financial Management of the Medical Practice (Practice Success)]

## Payer Mix by Allowed Charges
Practices can look at the percentage of their charges and allowed amounts per payer to determine their payer mix. If practices bill the same [[Fee schedule]] to all payers, they can monitor whether payers have gained or lost market share. If practices already know their preferred or less desirable contracts, recognizing shifts in the market will alert business managers to take necessary actions. It can also be helpful to look at payer mix by provider or specialty.

Another way to look at payer mix is to compare the billed charges to the allowed amount by payer:

| Primary Insurance | % of Billed Charges | % of Allowed Charges |
| ----------------- | ------------------- | -------------------- |
| Payer 1           | 15.1%               | 16.4%                |
| Payer 2           | 39.9%               | 42.2%                |
| Payer 3           | 5.2%                | 5.4%                 |
| Payer 4           | 1.1%                | 0.9%                 |
| Payer 5           | 14.9%               | 12.7%                |
| Payer 6           | 23.8%               | 22.2%                |
| Total             | 100.0%              | 100.0%               |

Payers like Payer 1 and 2 have a higher percentage of allowed charges than billed charges, indicating favorable contracts as compared to other payers. Payer 5, on the other hand, represents 14.9% of billed charges but only 12.7% of the allowed amounts, indicating a less favorable contract.

This analysis compares allowed amounts, not actual collections. It might be that a payer has a different demographic (more or less compliant patients, for example) or has sold high-[[Deductible]] plans to patients unable to meet that obligation. Tracking bad debt and collections [[Adjustments]] by the patients’ primary insurance can identify these payers.

Payer mix can also be evaluated over time to track and understand changes. For example, practices may have seen an increase in self-pay patients. To smooth out month-to-month fluctuations in the data, this payer mix uses a three-month moving average to compare last year’s payer mix to the current year. A similar analysis could be done by provider, facility, specialty, and other fields in the reimbursement dataset. The table below shows the percentage of allowed charges in the current-year column and compares that payer mix to the prior year’s payer mix. This data might also be displayed differently showing a five-year trend with a sparkline.^[ISBN 9781568294322 - Better Data, Better Decisions: Using Business Intelligence in the Medical Practice]


| Payer   | Current Year | Prior Year |
| ------- | ------------ | ---------- |
| Payer 1 | 16.4%        | 15.9%      |
| Payer 2 | 42.4%        | 39.5%      |
| Payer 3 | 5.4%         | 7.9%       |
| Payer 4 | 0.9%         | 0.8%       |
| Payer 5 | 12.7%        | 12.8%      |
| Payer 6 | 22.2%        | 23.1%      |

## Percentage of Medicare Reimbursement Charted against RVU Volume
Another part of a practice’s contracting strategy may be to use Medicare reimbursement as a baseline and then compare reimbursement as a percentage of Medicare:

![](https://i.imgur.com/7IDC7TN.png)
The red diagonal line represents the desired minimum average payment per RVU based on contracted rates as a percentage of Medicare (plotted on the y-axis) and the volume of RVUs for that payer as measured in RVUs (plotted on the x-axis). The red line is essentially the practice’s contracting strategy, which is to offer the best rates (lowest percentage of Medicare rates) to the payers purchasing the highest volume amount of services (as measured in RVUs) from the practice. 

Notice how Payers B and C both purchase a little less than 6,000 RVUs from this practice. Both payers are below the red line, especially Payer C. According to the pricing policy, payers who purchase 6,000 RVUs per year from the practice should pay about 135% of Medicare rates, but Payer C is only paying about 113%. Payer E is on the line, so their reimbursement rates are in lone with the volume of services purchased from the practice. Payers A and D are above the pricing policy line and are good contracts for the practice.

This model can be adjusted to take into account many reimbursement models, such as pay for performance, [[Capitation]], withholds, and bonuses. Another benchmark to chart on the y-axis might be the survey data regarding average payment per RVU from MGMA-ACMPE for the specialty, practice size, and region. Those reimbursement percentages can then be compared to RVU volume to analyze reimbursement by payer in context with the volume of patients per payer.^[ISBN 9781568294322 - Better Data, Better Decisions: Using Business Intelligence in the Medical Practice]



[ISBN 9781584266464 - Principles of Healthcare Reimbursement]: https://isbnsearch.org/isbn/9781584266464
[Practice Management Study Guide - AAPC - Google Books]: https://books.google.com/books/about/Practice_Management_Study_Guide.html?id=7uQWEAAAQBAJ
[ISBN 9781603592963 - Financial Management of the Medical Practice (Practice Success)]: https://isbnsearch.org/isbn/9781603592963
