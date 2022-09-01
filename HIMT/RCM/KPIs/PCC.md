---
tags: definition, him, kpi, metrics, rcm, analytics, data
author: Yuval Lirov
alias: Percentage of Clean Claims
related:
---
# Percentage of Clean Claims (PCC)
*What Can [[Clean claim|Clean Claims]] Tell Us About* [[Payer-Provider Conflict]]?

Dr. Payne shook his head in disbelief: the practice reimbursements had shrunk, instead of climbed, in response to the recent hiring of the new internist. The new doctor had clearly added to the total number of patients seen, yet overall payments did not reflect the added charges. Perhaps the new claims weren’t created, submitted or paid? Dr. Payne remembered noticing the growing pile of rejected and denied claims accumulating on his desk - he never had the time to review them. How many of these claims were clean? How many required manual review and correction?

He began analyzing the numbers. His billing software show 58% clean claims. In other words, almost half of the claims required manual correction. Who could be causing such a high level of problems - the practice, the billing service, or the payer? He instinctively felt that the billing service was negligent about the data entry process and kept introducing massive errors. But their service manager was quick to explain their rigorous QA process for data entry. What else could cause such a high level of manual work in a seemingly streamlined process?

Trying to discover a pattern, he looked for a root cause dimension, drilling into 99213 - the most frequent [[Current Procedural Terminology|CPT]] code for his practice. The software showed 3,135 claims for the 99213 code and these had an above average 62 PCC.

Having isolated the most frequent CPT code, he thought about other dimensions that influence PCC, hypothesizing that if all doctors in his practice had the same coding skills, and assuming uniform distribution of errors, there should be no PCC variance across the practice. However, after checking the software again, his suspicions were confirmed. Different doctors maintained slightly different coding skills:

| Provider      | Dr. Ted | Dr. Lori | Dr. Inn | Dr. Payne |
| ------------- | ------- | -------- | ------- | --------- |
| Claims        | 1,554   | 865      | 194     | 516       |
| PCC for 99213 | 63%     | 62%      | 61%     | 60%       |

- - -

Next, Dr. Payne switched his attention to PCC distribution across the financial classes, hypothesizing that if all payers used the same rules to deny claims, then there should be no difference in the average PCC for different payers, subject to a uniform distribution of errors over a large sample of submitted and paid claims. Yet the numbers showed a significant (30%) variation of PCC for 99213:

| Payer         | UHC | Horizon | Oxford | Aetna | Medicare | Cigna |
| ------------- | --- | ------- | ------ | ----- | -------- | ----- |
| PCC for 99213 | 82% | 73%     | 64%    | 59%   | 59%      | 51%   |

```chart
type: bar
labels: [UHC,Horizon,Oxford,Aetna,Medicare,Cigna]
series:
          - title: Clean Claim Distribution by Payers (%)
            data: [82,73,64,59,59,51]
tension: 0
width: 100%
labelColors: true
fill: true
beginAtZero: false
```

This confirmed his conclusion that different payers used different rules to deny and underpay claims. He recalled an article about PacifiCare, a California insurance company, being fined after an internal [[Audit]] revealed that 30% of their [[Health Maintenance Organization|HMO]] claims were wrongly denied and 29% of their disputes with doctors were handled incorrectly. His findings roughly matched the PacifiCare audit - the insurance companies were failing anywhere between 18% - 49% of his claims, and each insurance company showed a different failure rate, depending on their system for failing submitted claims.

- - -

Finally, Dr. Payne thought about his billing service operation. Did his billing service systematically work to discover failed claims and improve its response to such discoveries? Was there a pattern in the PCC, perhaps an occasional drop that might reflect a response to various payers’ initiatives? Conversely, was there any evidence of a systematic improvement effort? To answer his question, he output a chart of the distribution of a single [[Current Procedural Terminology|CPT]] code’s [[Clean claim]] percentage over the course of an entire year. He hypothesized that PCC should level out between occasional drops and climbs, hopefully settling at a slightly higher level after each time. He was looking for overall improvement through the year and the data and chart confirmed his expectations:

## Percentage Clean Claim Distribution

| Jan | Feb | Mar | Apr | May | Jun | Jul | Aug | Sep | Oct | Nov | Dec |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 46  | 39  | 52  | 55  | 63  | 67  | 72  | 69  | 72  | 68  | 74  | 73  |

```chart
type: line
labels: [Jan,Feb,Mar,Apr,May,Jun,Jul,Aug,Sept,Oct,Nov,Dec]
series:
  - title: Percentage of Clean Claims
    data: [46,39,52,55,63,67,72,69,72,68,74,73]
tension: 0
width: 100%
labelColors: false
fill: true
beginAtZero: false
```
---
In summary, he concluded that PCC must be a time-dependent function, which drops and climbs depending on four factors. Specifically, PCC goes down in response to:

1. Continuous *payer* initiatives to impede billing - rejecting, losing, delaying, and underpaying claims.
2. The *practice* missing or incorrectly submitting demographics and coding information.
3. The *billing service* entering erroneous or inconsistent data.

PCC improves in response to a concerted effort by both the practice and billing service to discover, correct, and avoid demographic, coding, and data entry problems. Large-scale medical billing networks create the necessary volumes and resulting economies of scale that enable the payment analyses to discover systemic claims processing problems.